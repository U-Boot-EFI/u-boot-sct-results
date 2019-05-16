# SCT test results

May 16th, 2019

## Boot services

| Service                             | Conformance   | Function   |
| ----------------------------------- | ------------- | ---------- |
|                                     |               |            |
| **Event, Timer, and Task Priority Services**                     |
| CreateEvent                         | PASS          | FAIL       |
| CreateEventEx                       | PASS          | FAIL       |
| CloseEvent                          | N/A           | PASS       |
| SignalEvent                         | N/A           | PASS       |
| WaitForEvent                        | PASS          | PASS       |
| CheckEvent                          | PASS          | PASS       |
| SetTimer                            |               |            |
| RaiseTPL                            |               |            |
| Restore TPL                         |               |            |
|                                     |               |            |
| **Memory Allocation Services**                                   |
| AllocatePages                       | PASS          | PASS       |
| FreePages                           | PASS          | PASS       |
| GetMemoryMap                        | PASS          | PASS       |
| AllocatePool                        | PASS          | PASS       |
| FreePool                            | PASS          | PASS       |
|                                     |               |            |
| **Protocol Handler Services**                                    |
| InstallProtocolInterface            | PASS          | PASS       |
| UninstallProtocolInterface          | PASS          | FAIL       |
| ReinstallProtocolInterface          |               |            |
| RegisterProtocolNotify              |               |            |
| LocateHandle                        |               |            |
| HandleProtocol                      | PASS          | PASS       |
| LocateDevicePath                    | PASS          | FAIL       |
| OpenProtocol                        |               |            |
| CloseProtocol                       |               |            |
| OpenProtocolInformation             |               |            |
| ConnectController                   |               |            |
| DisconnectController                |               |            |
| ProtocolsPerHandle                  |               |            |
| LocateHandleBuffer                  | PASS          | FAIL       |
| LocateProtocol                      | PASS          | FAIL       |
| InstallMultipleProtocolInterfaces   | PASS          | PASS       |
| UninstallMultipleProtocolInterfaces | PASS          | FAIL       |
|                                     |               |            |
| **Images Services**                                              |
| LoadImage                           |               |            |
| StartImage                          |               |            |
| UnloadImage                         |               |            |
| Exit                                |               |            |
| ExitBootServices                    |               |            |
|                                     |               |            |
| **Miscellaneous Boot Services**                                  |
| SetWatchDogTimer                    | N/A           | FAIL       |
| Stall                               | N/A           | PASS       |
| CopyMem                             | N/A           | PASS       |
| SetMem                              | N/A           | PASS       |
| GetNextMonotonicCount               | FAIL          | FAIL       |
| InstallConfigurationTable           | PASS          | PASS       |
| CalculateCrc32                      | PASS          | PASS       |
|                                     |               |            |
