# SCT test results

September 12th, 2019

The UEFI SCT test implementation has separate routines for testing if parameters
are correctly checked (conformance tests) and if a function does it jobs
(function tests).

* FAIL signifies that at least one failure was reported. It does not imply that
  the function is not working at all.
* \- signifies that the test reported no result
* N/A signifies that no test for this category is available.

## Boot services

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
| ConnectController                   | PASS        | FAIL       |
| DisconnectController                | PASS        | FAIL       |
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
| ExitBootServices                    | -    1)     | N/A        |
| Exit                                | PASS        | PASS       |
| LoadImage                           | PASS        | FAIL       |
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

1) Variable is not persisted across boot.

## Runtime services

| Service                              | Conformance | Function   |
| ------------------------------------ | ----------- | ---------- |
|                                      |             |            |
| **Variable Services**                                           |
| AuthVar                              | FAIL        | FAIL       |
| GetNextVariableName                  | PASS        | PASS       |
| GetVariable                          | PASS        | PASS       |
| HardwareErrorRecord                  | -           | -          |
| QueryVariableInfo                    | FAIL        | -          |
| SetVariable                          | FAIL        | FAIL       |
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

## Protocols

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
| FlushEx                             | -           | -          |
| Flush                               | FAIL        | PASS       |
| GetInfo                             | PASS        | FAIL       |
| GetPosition                         | PASS        | -          |
| OpenEx                              | -           | -          |
| OpenVolume                          | N/A         | FAIL       |
| Open                                | PASS        | PASS       |
| ReadEx                              | -           | -          |
| SetInfo                             | FAIL        | FAIL       |
| SetPosition                         | PASS        | PASS       |
| WriteEx                             | -           | -          |
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
| UpdatePackageList                   | N/A         | -          |
|                                     |             |            |
| **HIIStringProtocol**               |             |            |
| GetLanguages                        | -           | -          |
| GetSecondaryLanguages               | -           | -          |
| GetString                           | -           | -          |
| NewString                           | -           | -          |
| SetString                           | -           | -          |
|                                     |             |            |
| **SimpleTextInputExProtocol**                                  |
| ReadKeyStrokeEx                     | PASS        | not tested |
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
| BltVideoBltBuffer                   | N/A         | PASS       |
| BltVideoFill                        | N/A         | PASS       |
| BltVideoToVideo                     | N/A         | PASS       |
| Blt                                 | PASS        | N/A        |
| QueryMode                           | PASS        | PASS       |
| SetMode                             | PASS        | PASS       |

## Missing protocol implementations

* EFI\_DECOMPRESS\_PROTOCOL - required for any UEFI system
* EFI\_DISK\_IO\_PROTOCOL - required if device can boot from a disk device
