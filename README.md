# UEFI Self Certification Test (SCT)

## Running the SCT on the U-Boot sandbox

The SCT can be run on real hardware, on QEMU, or on the U-Boot sandbox.

For running on the sandbox execute

    make sandbox_defconfig

Then apply the following changes to file *.config*:

    CONFIG_SANDBOX_RAM_SIZE_MB=256
    # CONFIG_CONSOLE_TRUETYPE is not set
    CONFIG_SANDBOX_CRASH_RESET=y
    CONFIG_SYS_WHITE_ON_BLACK=y
    CONFIG_USE_PREBOOT=y
    CONFIG_PREBOOT="host bind 0 sct.img && load host 0:1 $kernel_addr_r Shell.efi && bootefi $kernel_addr_r"

On 32-bit systems additionally apply:

    CONFIG_HOST_32BIT=y

* The memory size is increased to work around a memory leak when running the
  SCT.

* The TrueType console does not support colored output yet and by default does
  not use a mono-spaced font.

* PREBOOT is needed to run the tests which involve resets.

On the SCT image create a script *startup.nsh* like:

    FS0:
    cls
    if exist run then
      rm run
      SCT -s uboot.seq
    else
      SCT -c
    endif
    SCT -g result.csv
    @echo "Test results are in Report\result.csv"
    @echo "DONE - SCT COMPLETED"
    reset -s

The script takes care of continuing the SCT after resets.

Start the sandbox with

    ./u-boot -l -S -T

## Test results

February 1st, 2021

The UEFI SCT test implementation has separate routines for testing if parameters
are correctly checked (conformance tests) and if a function does it jobs
(function tests).

* FAIL signifies that at least one failure was reported. It does not imply that
  the function is not working at all.
* \- signifies that the test reported no result
* N/A signifies that no test for this category is available.

### Boot services

| Service                             | Conformance | Function   |
| ----------------------------------- | ----------- | ---------- |
|                                     |             |            |
| **Event, Timer, and Task Priority Services**                   |
| CheckEvent                          | PASS        | PASS       |
| CloseEvent                          | N/A         | PASS       |
| CreateEventEx                       | PASS        | PASS       |
| CreateEvent                         | PASS        | PASS       |
| RaiseTPL                            | N/A         | PASS       |
| Restore TPL                         | N/A         | PASS       |
| SignalEvent                         | N/A         | PASS       |
| SetTimer                            | PASS        | PASS       |
| WaitForEvent                        | PASS        | PASS       |
|                                     |             |            |
| **Memory Allocation Services**                                 |
| AllocatePages                       | PASS        | PASS       |
| AllocatePool                        | PASS        | PASS       |
| FreePages                           | PASS        | PASS       |
| FreePool                            | PASS        | PASS       |
| GetMemoryMap                        | PASS        | PASS       |
|                                     |             |            |
| **Protocol Handler Services**                                  |
| CloseProtocol                       | PASS        | PASS       |
| ConnectController                   | PASS        | FAIL 1)    |
| DisconnectController                | PASS        | PASS       |
| HandleProtocol                      | PASS        | PASS       |
| InstallMultipleProtocolInterfaces   | PASS        | PASS       |
| InstallProtocolInterface            | PASS        | PASS       |
| LocateDevicePath                    | PASS        | PASS       |
| LocateHandleBuffer                  | PASS        | PASS       |
| LocateHandle                        | PASS        | PASS       |
| LocateProtocol                      | PASS        | PASS       |
| OpenProtocolInformation             | PASS        | PASS       |
| OpenProtocol                        | PASS        | PASS       |
| ProtocolsPerHandle                  | PASS        | PASS       |
| RegisterProtocolNotify              | PASS        | PASS       |
| ReinstallProtocolInterface          | PASS        | PASS       |
| UninstallMultipleProtocolInterfaces | PASS        | PASS       |
| UninstallProtocolInterface          | PASS        | PASS       |
|                                     |             |            |
| **Images Services**                                            |
| ExitBootServices                    | PASS        | N/A        |
| Exit                                | PASS        | PASS       |
| LoadImage                           | PASS        | FAIL 2)    |
| StartImage                          | PASS        | PASS       |
| UnloadImage                         | PASS        | PASS       |
|                                     |             |            |
| **Miscellaneous Boot Services**                                |
| CalculateCrc32                      | PASS        | PASS       |
| CopyMem                             | N/A         | PASS       |
| GetNextMonotonicCount               | PASS        | FAIL       |
| InstallConfigurationTable           | PASS        | PASS       |
| SetMem                              | N/A         | PASS       |
| SetWatchDogTimer                    | -           | PASS       |
| Stall                               | N/A         | PASS       |
|                                     |             |            |

1) Override protocols not supported

2) Loading of HII resource file not supported.

### Runtime services

| Service                              | Conformance | Function   |
| ------------------------------------ | ----------- | ---------- |
|                                      |             |            |
| **Variable Services**                                           |
| AuthVar                              | FAIL        | FAIL       |
| GetNextVariableName                  | PASS        | PASS       |
| GetVariable                          | PASS        | PASS       |
| HardwareErrorRecord                  | -           | -          |
| QueryVariableInfo                    | FAIL        | -          |
| SetVariable                          | PASS        | PASS       |
|                                      |             |            |
| **Time Services**                                               |
| GetTime                              | PASS        | PASS       |
| GetWakeupTime                        | -           | -          |
| SetTime                              | PASS        | FAIL 1)    |
| SetWakeupTime                        | -           | -          |
|                                      |             |            |
| **Miscellaneous Runtime Services**                              |
| QueryCapsuleCapabilities             | PASS        | PASS       |
| ResetSystem                          | N/A         | PASS       |
| UpdateCapsule                        | FAIL        | N/A        |

1) Setting of daylight saving time is not fully supported, setting
   the time zone is not supported.

### Protocols

| Protocol                            | Conformance | Function   |
| ----------------------------------- | ----------- | ---------- |
|                                     |             |            |
| **LoadedImageProtocol**                                        |
| Test 1                              | N/A         | PASS       |
| Teet 2                              | N/A         | PASS       |
|                                     |             |            |
| **DevicePathProtocol**                                         |
| PathNodeConf                        | PASS        | N/A        |
|                                     |             |            |
| **DevicePathUtilitiesProtocol**                                |
| AppendDeviceNode                    | PASS        | PASS       |
| AppendDevicePathInstance            | PASS        | PASS       |
| AppendDevicePath                    | PASS        | PASS       |
| CreateDeviceNode                    | PASS        | PASS       |
| DuplicateDevicePath                 | PASS        | PASS       |
| GetDevicePathSize                   | PASS        | PASS       |
| GetNextDevicePathInstance           | PASS        | PASS       |
| IsDevicePathMultiInstance           | N/A         | PASS       |
|                                     |             |            |
| **DevicePathToTextProtocol**                                   |
| ConvertDeviceNodeToText             | PASS        | FAIL       |
| ConvertDevicePathToText             | PASS        | FAIL       |
|                                     |             |            |
| **SimpleFileSystemProtocol**                                   |
| Close                               | N/A         | PASS       |
| Delete                              | PASS        | PASS       |
| FlushEx                             | PASS        | PASS       |
| Flush                               | PASS        | PASS       |
| GetInfo                             | PASS        | PASS       |
| GetPosition                         | PASS        | -          |
| OpenEx                              | PASS        | PASS       |
| OpenVolume                          | N/A         | PASS       |
| Open                                | PASS        | PASS       |
| ReadEx                              | PASS        | PASS       |
| SetInfo                             | FAIL        | FAIL       |
| SetPosition                         | PASS        | PASS       |
| WriteEx                             | FAIL        | -          |
| Write                               | N/A         | -          |
|                                     |             |            |
| **BlockIOProtocol**                                            |
| FlushBlocks                         | -           | -          |
| MediaInfoIntegrity                  | N/A         | -          |
| ReadBlocks                          | PASS        | PASS       |
| Reset                               | N/A         | PASS       |
|                                     |             |            |
| **SimpleNetworkProtocol**                                      |
| GetStatus                           | PASS        | PASS       |
| Initialize                          | PASS        | PASS       |
| MCastIpToMac                        | PASS        | PASS       |
| NVData                              | -           | -          |
| ReceiveFilterConf                   | -           | FAIL       |
| Receive                             | PASS        | N/A        |
| Reset                               | N/A         | -          |
| Shutdown                            | PASS        | PASS       |
| Start                               | PASS        | PASS       |
| StationAddress                      | -           | -          |
| Statistics                          | -           | PASS       |
| Stop                                | PASS        | PASS       |
| Transmit                            | PASS        | N/A        |
|                                     |             |            |
| **UnicodeCollation2Protocol**                                  |
| FatToStr                            | N/A         | PASS       |
| MetaiMatch                          | N/A         | PASS       |
| StriColl                            | N/A         | PASS       |
| StrLwr                              | N/A         | PASS       |
| StrToFat                            | N/A         | PASS       |
| StrUpr                              | N/A         | PASS       |
|                                     |             |            |
| **HIIDatabaseProtocol**                                        |
| ExportPackageLists                  | FAIL        | -          |
| FindKeyboardLayouts                 | PASS        | -          |
| GetKeyboardLayout                   | PASS        | -          |
| GetPackageListHandle                | FAIL        | -          |
| ListPackageLists                    | PASS        | -          |
| NewPackageList                      | PASS        | FAIL       |
| RegisterPackageNotify               | PASS        | N/A        |
| RemovePackageList                   | PASS        | -          |
| SetKeyboardLayout                   | FAIL        | -          |
| UnregisterPackageNotify             | PASS        | N/A        |
| UpdatePackageList                   | PASS        | -          |
|                                     |             |            |
| **HIIStringProtocol**               |             |            |
| GetLanguages                        | -           | -          |
| GetSecondaryLanguages               | -           | -          |
| GetString                           | -           | -          |
| NewString                           | -           | -          |
| SetString                           | -           | -          |
|                                     |             |            |
| **SimpleTextInputExProtocol**                                  |
| ReadKeyStrokeEx                     | PASS        | -          |
| RegisterKeyNotify                   | PASS        | N/A        |
| Reset                               | N/A         | PASS       |
| SetState                            | PASS        | N/A        |
| UnregisterKeyNotify                 | PASS        | N/A        |
|                                     |             |            |
| **SimpleInputProtocol**                                        |
| Reset                               | N/A         | PASS       |
|                                     |             |            |
| **SimpleOutputProtocol**                                       |
| ClearScreen                         | N/A         | PASS       |
| EnableCursor                        | N/A         | PASS       |
| OutputString                        | N/A         | PASS       |
| QueryMode                           | PASS        | PASS       |
| Reset                               | N/A         | PASS       |
| SetAttribute                        | N/A         | PASS       |
| SetCursorPosition                   | PASS        | PASS       |
| SetMode                             | PASS        | PASS       |
| TestString                          | N/A         | PASS       |
|                                     |             |            |
| **GraphicsOutputProtocol**          |             |            |
| BltVideoBltBuffer                   | N/A         | FAIL       |
| BltVideoFill                        | N/A         | FAIL       |
| BltVideoToVideo                     | N/A         | PASS       |
| Blt                                 | PASS        | N/A        |
| QueryMode                           | PASS        | PASS       |
| SetMode                             | PASS        | PASS       |
|                                     |             |            |
| **RNGProtocolTest**                                            |
| GetInfo                             | PASS        | PASS       |
| GetRNG                              | PASS        | PASS       |
|                                     |             |            |



### Missing protocol implementations

* EFI\_DECOMPRESS\_PROTOCOL - required for any UEFI system
* EFI\_DISK\_IO\_PROTOCOL - required if device can boot from a disk device
