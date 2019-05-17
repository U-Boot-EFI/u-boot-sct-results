# SCT test results

May 17th, 2019

## Boot services

| Service                             | Conformance | Function   |
| ----------------------------------- | ----------- | ---------- |
|                                     |             |            |
| **Event, Timer, and Task Priority Services**                   |
| CreateEvent                         | PASS        | FAIL       |
| CreateEventEx                       | PASS        | FAIL       |
| CloseEvent                          | N/A         | PASS       |
| SignalEvent                         | N/A         | PASS       |
| WaitForEvent                        | PASS        | PASS       |
| CheckEvent                          | PASS        | PASS       |
| SetTimer                            | PASS        | FAIL       |
| RaiseTPL                            | N/A         | PASS       |
| Restore TPL                         | N/A         | PASS       |
|                                     |             |            |
| **Memory Allocation Services**                                 |
| AllocatePages                       | PASS        | PASS       |
| FreePages                           | PASS        | PASS       |
| GetMemoryMap                        | PASS        | PASS       |
| AllocatePool                        | PASS        | PASS       |
| FreePool                            | PASS        | PASS       |
|                                     |             |            |
| **Protocol Handler Services**                                  |
| InstallProtocolInterface            | PASS        | PASS       |
| UninstallProtocolInterface          | PASS        | FAIL       |
| ReinstallProtocolInterface          | PASS        | FAIL       |
| RegisterProtocolNotify              | PASS        | PASS       |
| LocateHandle                        | PASS        | FAIL       |
| HandleProtocol                      | PASS        | PASS       |
| LocateDevicePath                    | PASS        | FAIL       |
| OpenProtocol                        | PASS        | CRASH      |
| CloseProtocol                       | PASS        | PASS       |
| OpenProtocolInformation             | PASS        | FAIL       |
| ConnectController                   | PASS        | FAIL       |
| DisconnectController                | PASS        | FAIL       |
| ProtocolsPerHandle                  | PASS        | PASS       |
| LocateHandleBuffer                  | PASS        | FAIL       |
| LocateProtocol                      | PASS        | FAIL       |
| InstallMultipleProtocolInterfaces   | PASS        | PASS       |
| UninstallMultipleProtocolInterfaces | PASS        | FAIL       |
|                                     |             |            |
| **Images Services**                                            |
| LoadImage                           | FAIL        | FAIL       |
| StartImage                          |             |            |
| UnloadImage                         |             |            |
| Exit                                |             |            |
| ExitBootServices                    |             |            |
|                                     |             |            |
| **Miscellaneous Boot Services**                                |
| SetWatchDogTimer                    | N/A         | FAIL       |
| Stall                               | N/A         | PASS       |
| CopyMem                             | N/A         | PASS       |
| SetMem                              | N/A         | PASS       |
| GetNextMonotonicCount               | FAIL        | FAIL       |
| InstallConfigurationTable           | PASS        | PASS       |
| CalculateCrc32                      | PASS        | PASS       |
|                                     |             |            |
