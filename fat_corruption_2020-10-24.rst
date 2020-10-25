Corruption of FAT file system
=============================

Running the SCT leads to corruptions of the U-Boot FAT file system

::

    $ sudo dosfsck -w -r -l -a -v -t /dev/loop0
    fsck.fat 4.1 (2017-01-24)
    Checking we can access the last sector of the filesystem
    Boot sector contents:
    System ID "mkfs.fat"
    Media byte 0xf8 (hard disk)
           512 bytes per logical sector
          2048 bytes per cluster
             4 reserved sectors
    First FAT starts at byte 2048 (sector 4)
             2 FATs, 16 bit entries
        131072 bytes per FAT (= 256 sectors)
    Root directory starts at byte 264192 (sector 516)
           512 root directory entries
    Data area starts at byte 280576 (sector 548)
         65398 data clusters (133935104 bytes)
    32 sectors/track, 64 heads
             0 hidden sectors
        262142 sectors total
    Checking file /boot.scr (BOOT.SCR)
    Checking file /startup.nsh (STARTUP.NSH)
    Orphaned long file name part "run"
      Auto-deleting.
    Checking file /Application (APPLIC~1)
    Checking file /Data (DATA)
    Checking file /Dependency (DEPEND~1)
    Checking file /Ents (ENTS)
    Checking file /Proxy (PROXY)
    Checking file /Report (REPORT)
    Checking file /SCRT
    Checking file /SCT.efi (SCT.EFI)
    Checking file /Sequence (SEQUENCE)
    Checking file /StallForKey.efi (STALLF~1.EFI)
    Checking file /Support (SUPPORT)
    Checking file /Test (TEST)
    Checking file /Shell.efi (SHELL.EFI)
    Orphaned long file name part "Sct.log"
      Auto-deleting.
    Orphaned long file name part "Sct.log"
      Auto-deleting.
    Orphaned long file name part "verbose.mode"
      Auto-deleting.
    Checking file /Overall (OVERALL)
    Checking file /Log (LOG)
    Checking file /ubootefi.var (UBOOTEFI.VAR)
    Orphaned long file name part "Sct.log"
      Auto-deleting.
    Orphaned long file name part "verbose.mode"
      Auto-deleting.
    Orphaned long file name part "Sct.log"
      Auto-deleting.
    Orphaned long file name part "verbose.mode"
      Auto-deleting.
    Orphaned long file name part "Sct.log"
      Auto-deleting.
    Orphaned long file name part "verbose.mode"
      Auto-deleting.
    Orphaned long file name part "Sct.log"
      Auto-deleting.
    Orphaned long file name part "verbose.mode"
      Auto-deleting.
    Orphaned long file name part "Sct.log"
      Auto-deleting.
    Orphaned long file name part "verbose.mode"
      Auto-deleting.
    Orphaned long file name part "Sct.log"
      Auto-deleting.
    Orphaned long file name part "verbose.mode"
      Auto-deleting.
    Orphaned long file name part "Sct.log"
      Auto-deleting.
    Orphaned long file name part "verbose.mode"
      Auto-deleting.
    Orphaned long file name part "Sct.log"
      Auto-deleting.
    Orphaned long file name part "verbose.mode"
      Auto-deleting.
    Orphaned long file name part "Sct.log"
      Auto-deleting.
    Orphaned long file name part "verbose.mode"
      Auto-deleting.
    Orphaned long file name part "Sct.log"
      Auto-deleting.
    Orphaned long file name part "verbose.mode"
      Auto-deleting.
    Orphaned long file name part "Sct.log"
      Auto-deleting.
    Orphaned long file name part "verbose.mode"
      Auto-deleting.
    Orphaned long file name part "Sct.log"
      Auto-deleting.
    Orphaned long file name part "verbose.mode"
      Auto-deleting.
    Orphaned long file name part "Sct.log"
      Auto-deleting.
    Orphaned long file name part "verbose.mode"
      Auto-deleting.
    Orphaned long file name part "Sct.log"
      Auto-deleting.
    Orphaned long file name part "verbose.mode"
      Auto-deleting.
    Orphaned long file name part "Sct.log"
      Auto-deleting.
    Orphaned long file name part "verbose.mode"
      Auto-deleting.
    Orphaned long file name part "Sct.log"
      Auto-deleting.
    Orphaned long file name part "verbose.mode"
      Auto-deleting.
    Orphaned long file name part "Sct.log"
      Auto-deleting.
    Orphaned long file name part "verbose.mode"
      Auto-deleting.
    Orphaned long file name part "Sct.log"
      Auto-deleting.
    Orphaned long file name part "verbose.mode"
      Auto-deleting.
    Orphaned long file name part "Sct.log"
      Auto-deleting.
    Orphaned long file name part "verbose.mode"
      Auto-deleting.
    Orphaned long file name part "Sct.log"
      Auto-deleting.
    Orphaned long file name part "verbose.mode"
      Auto-deleting.
    Orphaned long file name part "Sct.log"
      Auto-deleting.
    Orphaned long file name part "verbose.mode"
      Auto-deleting.
    Orphaned long file name part "Sct.log"
      Auto-deleting.
    Orphaned long file name part "verbose.mode"
      Auto-deleting.
    Orphaned long file name part "Sct.log"
      Auto-deleting.
    Orphaned long file name part "verbose.mode"
      Auto-deleting.
    Orphaned long file name part "Sct.log"
      Auto-deleting.
    Orphaned long file name part "verbose.mode"
      Auto-deleting.
    Orphaned long file name part "Sct.log"
      Auto-deleting.
    Orphaned long file name part "verbose.mode"
      Auto-deleting.
    Orphaned long file name part "Sct.log"
      Auto-deleting.
    Orphaned long file name part "verbose.mode"
      Auto-deleting.
    Orphaned long file name part "Sct.log"
      Auto-deleting.
    Orphaned long file name part "verbose.mode"
      Auto-deleting.
    Orphaned long file name part "Dir1"
      Auto-deleting.
    Orphaned long file name part "Dir2"
      Auto-deleting.
    Orphaned long file name part "File1"
      Auto-deleting.
    Orphaned long file name part "Dir1"
      Auto-deleting.
    Orphaned long file name part "Dir2"
      Auto-deleting.
    Orphaned long file name part "File1"
      Auto-deleting.
    Orphaned long file name part "BBTestDeleteBasicTestCheckpoint1_File1"
      Auto-deleting.
    Orphaned long file name part "BBTestDeleteBasicTestCheckpoint1_File1"
      Auto-deleting.
    Orphaned long file name part "BBTestDeleteBasicTestCheckpoint2_Dir1"
      Auto-deleting.
    Orphaned long file name part "BBTestDeleteBasicTestCheckpoint2_Dir1"
      Auto-deleting.
    Orphaned long file name part "BBTestDeleteBasicTestCheckpoint3_Dir1"
      Auto-deleting.
    Orphaned long file name part "BBTestDeleteBasicTestCheckpoint3_Dir1"
      Auto-deleting.
    Orphaned long file name part "BBTestFlushExConformanceTestCheckpoint1_File"
      Auto-deleting.
    Orphaned long file name part "BBTestFlushExBasicTestCheckpoint1_File"
      Auto-deleting.
    Orphaned long file name part "BBTestFlushExBasicTestCheckpoint2_File"
      Auto-deleting.
    Orphaned long file name part "BBTestFlushExBasicTestCheckpoint3_Dir"
      Auto-deleting.
    Orphaned long file name part "BBTestFlushExBasicTestCheckpoint4_Dir"
      Auto-deleting.
    Orphaned long file name part "BBTestFlushExBasicTestCheckpoint4_File"
      Auto-deleting.
    Orphaned long file name part "BBTestFlushExBasicTestCheckpoint4_File"
      Auto-deleting.
    Orphaned long file name part "BBTestFlushConformanceTestCheckpoint2_File"
      Auto-deleting.
    Orphaned long file name part "BBTestFlushBasicTestCheckpoint1_File"
      Auto-deleting.
    Orphaned long file name part "BBTestFlushBasicTestCheckpoint2_Dir"
      Auto-deleting.
    Orphaned long file name part "BBTestGetInfoConformanceTestCheckpoint1_File"
      Auto-deleting.
    Orphaned long file name part "BBTestGetInfoConformanceTestCheckpoint2_File"
      Auto-deleting.
    Orphaned long file name part "BBTestGetInfoConformanceTestCheckpoint2_Dir"
      Auto-deleting.
    Orphaned long file name part "[abc123]][()].Aa [b"
      Auto-deleting.
    Orphaned long file name part "[abc123]][()].Aa [b"
      Auto-deleting.
    Checking file /BBTestGetInfoBasicTestCheckpoint3_File_0 (BBTEST~1)
    Checking file /BBTestGetInfoBasicTestCheckpoint3_File_1 (BBTEST~1)
    Checking file /BBTestGetInfoBasicTestCheckpoint3_File_2 (BBTEST~1)
    Orphaned long file name part "Sct.log"
      Auto-deleting.
    Orphaned long file name part "verbose.mode"
      Auto-deleting.
    Orphaned long file name part "BBTestGetPositionConformanceTestCheckpoint1_Dir"
      Auto-deleting.
    Orphaned long file name part "BBTestGetPositionBasicTestCheckpoint1_File"
      Auto-deleting.
    Orphaned long file name part "BBTestGetPositionBasicTestCheckpoint1_File"
      Auto-deleting.
    Orphaned long file name part "BBTestGetPositionBasicTestCheckpoint1_ReadOnlyFile"
      Auto-deleting.
    Orphaned long file name part "BBTestGetPositionBasicTestCheckpoint1_File"
      Auto-deleting.
    Orphaned long file name part "BBTestGetPositionBasicTestCheckpoint1_File"
      Auto-deleting.
    Orphaned long file name part "BBTestGetPositionBasicTestCheckpoint1_ReadOnlyFile"
      Auto-deleting.
    Orphaned long file name part "BBTestOpenConformanceTestCheckpoint3_File"
      Auto-deleting.
    Orphaned long file name part "[abc123]][()].Aa [b"
      Auto-deleting.
    Orphaned long file name part "Sct.log"
      Auto-deleting.
    Orphaned long file name part "verbose.mode"
      Auto-deleting.
    Orphaned long file name part "BBTestOpenConformanceTestCheckpoint3_File"
      Auto-deleting.
    Orphaned long file name part "[abc123]][()].Aa [b"
      Auto-deleting.
    Orphaned long file name part "[abc123]][()].Aa [b"
      Auto-deleting.
    Orphaned long file name part "[abc123]][()].Aa [b"
      Auto-deleting.
    Orphaned long file name part "[abc123]][()].Aa [b"
      Auto-deleting.
    Orphaned long file name part "[abc123]][()].Aa [b"
      Auto-deleting.
    Orphaned long file name part "[abc123]][()].Aa [b"
      Auto-deleting.
    Orphaned long file name part "[abc123]][()].Aa [b"
      Auto-deleting.
    Orphaned long file name part "[abc123]][()].Aa [b"
      Auto-deleting.
    Orphaned long file name part "[abc123]][()].Aa [b"
      Auto-deleting.
    Orphaned long file name part "[abc123]][()].Aa [b"
      Auto-deleting.
    Orphaned long file name part "BBTestReadExConformanceTestCheckpoint1_File"
      Auto-deleting.
    Orphaned long file name part "BBTestReadExConformanceTestCheckpoint2_File"
      Auto-deleting.
    Orphaned long file name part "BBTestReadExBasicTestCheckpoint1_File"
      Auto-deleting.
    Orphaned long file name part "BBTestReadExBasicTestCheckpoint2_File"
      Auto-deleting.
    Orphaned long file name part "BBTestReadExBasicTestCheckpoint3_Dir"
      Auto-deleting.
    Orphaned long file name part "BBTestReadBasicTestCheckpoint2_Dir"
      Auto-deleting.
    Orphaned long file name part "BBTestReadBasicTestCheckpoint1_File"
      Auto-deleting.
    Orphaned long file name part "BBTestReadBasicTestCheckpoint2_Dir"
      Auto-deleting.
    Orphaned long file name part "BBTestSetInfoConformanceTestCheckpoint1_File"
      Auto-deleting.
    Orphaned long file name part "BBTestSetInfoConformanceTestCheckpoint2_File"
      Auto-deleting.
    Orphaned long file name part "BBTestSetInfoConfTestCheckpoint2_File_New"
      Auto-deleting.
    Orphaned long file name part "BBTestSetInfoConformanceTestCheckpoint2_Dir"
      Auto-deleting.
    Orphaned long file name part "BBTestSetInfoConfTestCheckpoint2_File_New"
      Auto-deleting.
    Orphaned long file name part "BBTestSetInfoConformanceTestCheckpoint3_File"
      Auto-deleting.
    Orphaned long file name part "BBTestSetInfoConformanceTestCheckpoint3_Dir"
      Auto-deleting.
    Orphaned long file name part "BBTestSetInfoConformanceTestCheckpoint4_File"
      Auto-deleting.
    Orphaned long file name part "BBTestSetInfoConformanceTestCheckpoint4_Dir"
      Auto-deleting.
    Orphaned long file name part "BBTestSetInfoConformanceTestCheckpoint6_File"
      Auto-deleting.
    Orphaned long file name part "BBTestSetInfoConformanceTestCheckpoint7_File_One"
      Auto-deleting.
    Orphaned long file name part "BBTestSetInfoConformanceTestCheckpoint7_File_Two"
      Auto-deleting.
    Orphaned long file name part "[abc123]][()].Aa [b"
      Auto-deleting.
    Orphaned long file name part "[abc123]][()].Aa [b"
      Auto-deleting.
    Orphaned long file name part "BBTestSetPositionConformanceTestCheckpoint1_Dir"
      Auto-deleting.
    Orphaned long file name part "BBTestSetPositionBasicTestCheckpoint1_File"
      Auto-deleting.
    Orphaned long file name part "BBTestSetPositionBasicTestCheckpoint1_ReadOnlyOpenFile"
      Auto-deleting.
    Orphaned long file name part "BBTestSetPositionBasicTestCheckpoint1_ReadOnlyFile"
      Auto-deleting.
    Orphaned long file name part "BBTestSetPositionBasicTestCheckpoint2_Dir"
      Auto-deleting.
    Orphaned long file name part "BBTestWriteExConformanceTestCheckpoint1_Dir"
      Auto-deleting.
    Orphaned long file name part "BBTestWriteExConformanceTestCheckpoint2_File"
      Auto-deleting.
    Orphaned long file name part "BBTestWriteExConformanceTestCheckpoint3_File"
      Auto-deleting.
    Orphaned long file name part "BBTestWriteExBasicTestCheckpoint1_File"
      Auto-deleting.
    Orphaned long file name part "BBTestWriteExBasicTestCheckpoint2_File"
      Auto-deleting.
    Orphaned long file name part "BBTestWriteExBasicTestCheckpoint3_File1"
      Auto-deleting.
    Orphaned long file name part "BBTestWriteExBasicTestCheckpoint3_File2"
      Auto-deleting.
    Orphaned long file name part "BBTestWriteExBasicTestCheckpoint3_File3"
      Auto-deleting.
    /BBTestGetInfoBasicTestCheckpoint3_File_0
      Duplicate directory entry.
      First    Size 0 bytes, date 01:00:00 Dec 31 1979
      Second   Size 0 bytes, date 01:00:00 Dec 31 1979
      Auto-renaming second.
      Renamed to FSCK0000.000
    /BBTestGetInfoBasicTestCheckpoint3_File_0
      Duplicate directory entry.
      First    Size 0 bytes, date 01:00:00 Dec 31 1979
      Second   Size 0 bytes, date 01:00:00 Dec 31 1979
      Auto-renaming second.
      Renamed to FSCK0000.001
    Checking file /Application/.
    Checking file /Application/..
    Checking file /Data/.
    Checking file /Data/..
    Checking file /Data/Category.ini (CATEGORY.INI)
    Checking file /Data/GuidFile.txt (GUIDFILE.TXT)
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "Recovery.dat"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "Recovery.dat"
      Auto-deleting.
    Orphaned long file name part "Recovery.dat"
      Auto-deleting.
    Orphaned long file name part "Recovery.dat"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "Recovery.dat"
      Auto-deleting.
    Orphaned long file name part "Recovery.dat"
      Auto-deleting.
    Orphaned long file name part "Recovery.dat"
      Auto-deleting.
    Orphaned long file name part "Recovery.dat"
      Auto-deleting.
    Orphaned long file name part "Recovery.dat"
      Auto-deleting.
    Orphaned long file name part "Recovery.dat"
      Auto-deleting.
    Orphaned long file name part "Recovery.dat"
      Auto-deleting.
    Orphaned long file name part "Recovery.dat"
      Auto-deleting.
    Orphaned long file name part "Recovery.dat"
      Auto-deleting.
    Orphaned long file name part "Recovery.dat"
      Auto-deleting.
    Orphaned long file name part "Recovery.dat"
      Auto-deleting.
    Orphaned long file name part "Recovery.dat"
      Auto-deleting.
    Orphaned long file name part "Recovery.dat"
      Auto-deleting.
    Orphaned long file name part "Recovery.dat"
      Auto-deleting.
    Orphaned long file name part "Recovery.dat"
      Auto-deleting.
    Orphaned long file name part "Recovery.dat"
      Auto-deleting.
    Orphaned long file name part "Recovery.dat"
      Auto-deleting.
    Orphaned long file name part "Recovery.dat"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "Recovery.dat"
      Auto-deleting.
    Orphaned long file name part "Recovery.dat"
      Auto-deleting.
    Orphaned long file name part "Recovery.dat"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "Recovery.dat"
      Auto-deleting.
    Orphaned long file name part "Recovery.dat"
      Auto-deleting.
    Orphaned long file name part "Recovery.dat"
      Auto-deleting.
    Orphaned long file name part "Recovery.dat"
      Auto-deleting.
    Orphaned long file name part "Recovery.dat"
      Auto-deleting.
    Orphaned long file name part "Recovery.dat"
      Auto-deleting.
    Orphaned long file name part "Recovery.dat"
      Auto-deleting.
    Orphaned long file name part "Recovery.dat"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "Recovery.dat"
      Auto-deleting.
    Orphaned long file name part "Recovery.dat"
      Auto-deleting.
    Orphaned long file name part "Recovery.dat"
      Auto-deleting.
    Orphaned long file name part "Recovery.dat"
      Auto-deleting.
    Orphaned long file name part "Recovery.dat"
      Auto-deleting.
    Orphaned long file name part "Recovery.dat"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "SkippedCase.ini"
      Auto-deleting.
    Orphaned long file name part "SkippedCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "SkippedCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "SkippedCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "SkippedCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "SkippedCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "SkippedCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "SkippedCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Checking file /Data/SkippedCase.ini (SKIPPE~1.INI)
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Orphaned long file name part "TestCase.ini"
      Auto-deleting.
    Checking file /Data/TestCase.ini (TESTCASE.INI)
    /Data  and
    /Data/GuidFile.txt
      share clusters.
      Truncating second to 210944 bytes.
    /Data/GuidFile.txt
      File size is 1330592 bytes, cluster chain length is 210944 bytes.
      Truncating file to 210944 bytes.
    Checking file /Dependency/.
    Checking file /Dependency/..
    Checking file /Dependency/EfiCompliantBBTest (EFICOM~1)
    Checking file /Dependency/ProtocolHandlerServicesBBTest (PROTOC~1)
    Checking file /Dependency/ImageServicesBBTest (IMAGES~1)
    Checking file /Dependency/DecompressBBTest (DECOMP~1)
    Checking file /Dependency/DeviceIoBBTest (DEVICE~1)
    Checking file /Dependency/EbcBBTest (EBCBBT~1)
    Checking file /Dependency/LoadedImageBBTest (LOADED~1)
    Checking file /Dependency/PciIoBBTest (PCIIOB~1)
    Checking file /Dependency/PciRootBridgeIoBBTest (PCIROO~1)
    Checking file /Dependency/PxeBaseCodeBBTest (PXEBAS~1)
    Checking file /Dependency/ConfigKeywordHandlerBBTest (CONFIG~1)
    Checking file /Dependency/EfiCompliantBBTest/.
    Checking file /Dependency/EfiCompliantBBTest/..
    Checking file /Dependency/EfiCompliantBBTest/EfiCompliant.ini (EFICOM~1.INI)
    Checking file /Dependency/ProtocolHandlerServicesBBTest/.
    Checking file /Dependency/ProtocolHandlerServicesBBTest/..
    Checking file /Dependency/ProtocolHandlerServicesBBTest/BusDriver1.efi (BUSDRI~1.EFI)
    Checking file /Dependency/ProtocolHandlerServicesBBTest/BusDriver2.efi (BUSDRI~2.EFI)
    Checking file /Dependency/ProtocolHandlerServicesBBTest/BusDriver3.efi (BUSDRI~3.EFI)
    Checking file /Dependency/ProtocolHandlerServicesBBTest/BusDriver4.efi (BUSDRI~4.EFI)
    Checking file /Dependency/ProtocolHandlerServicesBBTest/BusOverrideDriver1.efi (BUSOVE~1.EFI)
    Checking file /Dependency/ProtocolHandlerServicesBBTest/DBindingDriver1.efi (DBINDI~1.EFI)
    Checking file /Dependency/ProtocolHandlerServicesBBTest/DBindingDriver2.efi (DBINDI~2.EFI)
    Checking file /Dependency/ProtocolHandlerServicesBBTest/DBindingDriver3.efi (DBINDI~3.EFI)
    Checking file /Dependency/ProtocolHandlerServicesBBTest/DBindingDriver4.efi (DBINDI~4.EFI)
    Checking file /Dependency/ProtocolHandlerServicesBBTest/DBindingDriver5.efi (DBINDI~5.EFI)
    Checking file /Dependency/ProtocolHandlerServicesBBTest/DeviceDriver110.efi (DEVICE~1.EFI)
    Checking file /Dependency/ProtocolHandlerServicesBBTest/DeviceDriver111.efi (DEVICE~2.EFI)
    Checking file /Dependency/ProtocolHandlerServicesBBTest/DeviceDriver11.efi (DEVICE~3.EFI)
    Checking file /Dependency/ProtocolHandlerServicesBBTest/DeviceDriver12.efi (DEVICE~4.EFI)
    Checking file /Dependency/ProtocolHandlerServicesBBTest/DeviceDriver13.efi (DEVICE~5.EFI)
    Checking file /Dependency/ProtocolHandlerServicesBBTest/DeviceDriver14.efi (DEVICE~6.EFI)
    Checking file /Dependency/ProtocolHandlerServicesBBTest/DeviceDriver15.efi (DEVICE~7.EFI)
    Checking file /Dependency/ProtocolHandlerServicesBBTest/DeviceDriver18.efi (DEVICE~8.EFI)
    Checking file /Dependency/ProtocolHandlerServicesBBTest/DeviceDriver19.efi (DEVICE~9.EFI)
    Checking file /Dependency/ProtocolHandlerServicesBBTest/DeviceDriver1.efi (DEB0E0~2.EFI)
    Checking file /Dependency/ProtocolHandlerServicesBBTest/DeviceDriver2.efi (DEB0D5~2.EFI)
    Checking file /Dependency/ProtocolHandlerServicesBBTest/DeviceDriver3.efi (DEB0CA~2.EFI)
    Checking file /Dependency/ProtocolHandlerServicesBBTest/DeviceDriver4.efi (DEB0BF~2.EFI)
    Checking file /Dependency/ProtocolHandlerServicesBBTest/DeviceDriver5.efi (DEB0B4~2.EFI)
    Checking file /Dependency/ProtocolHandlerServicesBBTest/DeviceDriver6.efi (DEB0A9~2.EFI)
    Checking file /Dependency/ProtocolHandlerServicesBBTest/DeviceDriver7.efi (DEB09E~2.EFI)
    Checking file /Dependency/ProtocolHandlerServicesBBTest/PlatformOverrideDriver1.efi (PLATFO~1.EFI)
    Checking file /Dependency/ProtocolHandlerServicesBBTest/TestDriver1.efi (TESTDR~1.EFI)
    Checking file /Dependency/ProtocolHandlerServicesBBTest/TestDriver2.efi (TESTDR~2.EFI)
    Checking file /Dependency/ProtocolHandlerServicesBBTest/TestDriver3.efi (TESTDR~3.EFI)
    Checking file /Dependency/ProtocolHandlerServicesBBTest/TestDriver4.efi (TESTDR~4.EFI)
    Checking file /Dependency/ProtocolHandlerServicesBBTest/TestDriver5.efi (TESTDR~5.EFI)
    Checking file /Dependency/ImageServicesBBTest/.
    Checking file /Dependency/ImageServicesBBTest/..
    Checking file /Dependency/ImageServicesBBTest/InvalidImage1 (INVALI~1)
    Checking file /Dependency/ImageServicesBBTest/InvalidImage2 (INVALI~2)
    Checking file /Dependency/ImageServicesBBTest/InvalidImage3 (INVALI~3)
    Checking file /Dependency/ImageServicesBBTest/InvalidImage4 (INVALI~4)
    Checking file /Dependency/ImageServicesBBTest/InvalidImage5 (INVALI~5)
    Checking file /Dependency/ImageServicesBBTest/InvalidImage6 (INVALI~6)
    Checking file /Dependency/ImageServicesBBTest/InvalidImage7 (INVALI~7)
    Checking file /Dependency/ImageServicesBBTest/Application1.efi (APPLIC~1.EFI)
    Checking file /Dependency/ImageServicesBBTest/Application2.efi (APPLIC~2.EFI)
    Checking file /Dependency/ImageServicesBBTest/Application3.efi (APPLIC~3.EFI)
    Checking file /Dependency/ImageServicesBBTest/Application4.efi (APPLIC~4.EFI)
    Checking file /Dependency/ImageServicesBBTest/BootServicesDriver1.efi (BOOTSE~1.EFI)
    Checking file /Dependency/ImageServicesBBTest/BootServicesDriver2.efi (BOOTSE~2.EFI)
    Checking file /Dependency/ImageServicesBBTest/BootServicesDriver3.efi (BOOTSE~3.EFI)
    Checking file /Dependency/ImageServicesBBTest/BootServicesDriver4.efi (BOOTSE~4.EFI)
    Checking file /Dependency/ImageServicesBBTest/BootServicesDriver5.efi (BOOTSE~5.EFI)
    Checking file /Dependency/ImageServicesBBTest/BootServicesDriver6.efi (BOOTSE~6.EFI)
    Checking file /Dependency/ImageServicesBBTest/CombinationImage10.efi (COMBIN~1.EFI)
    Checking file /Dependency/ImageServicesBBTest/CombinationImage1.efi (COMBIN~2.EFI)
    Checking file /Dependency/ImageServicesBBTest/CombinationImage2.efi (COMBIN~3.EFI)
    Checking file /Dependency/ImageServicesBBTest/CombinationImage3.efi (COMBIN~4.EFI)
    Checking file /Dependency/ImageServicesBBTest/CombinationImage4.efi (COMBIN~5.EFI)
    Checking file /Dependency/ImageServicesBBTest/CombinationImage5.efi (COMBIN~6.EFI)
    Checking file /Dependency/ImageServicesBBTest/CombinationImage6.efi (COMBIN~7.EFI)
    Checking file /Dependency/ImageServicesBBTest/CombinationImage7.efi (COMBIN~8.EFI)
    Checking file /Dependency/ImageServicesBBTest/CombinationImage8.efi (COMBIN~9.EFI)
    Checking file /Dependency/ImageServicesBBTest/CombinationImage9.efi (COB0E1~2.EFI)
    Checking file /Dependency/ImageServicesBBTest/LoadFileDriver.efi (LOADFI~1.EFI)
    Checking file /Dependency/ImageServicesBBTest/RuntimeServicesDriver1.efi (RUNTIM~1.EFI)
    Checking file /Dependency/ImageServicesBBTest/RuntimeServicesDriver2.efi (RUNTIM~2.EFI)
    Checking file /Dependency/ImageServicesBBTest/RuntimeServicesDriver3.efi (RUNTIM~3.EFI)
    Checking file /Dependency/ImageServicesBBTest/RuntimeServicesDriver4.efi (RUNTIM~4.EFI)
    Checking file /Dependency/ImageServicesBBTest/RuntimeServicesDriver5.efi (RUNTIM~5.EFI)
    Checking file /Dependency/ImageServicesBBTest/RuntimeServicesDriver6.efi (RUNTIM~6.EFI)
    Checking file /Dependency/ImageServicesBBTest/ValidHiiImage1.efi (VALIDH~1.EFI)
    Checking file /Dependency/DecompressBBTest/.
    Checking file /Dependency/DecompressBBTest/..
    Checking file /Dependency/DecompressBBTest/InvalidCompressedFile1.cmp (INVALI~1.CMP)
    Checking file /Dependency/DecompressBBTest/DecompressBbTest.ini (DECOMP~1.INI)
    Checking file /Dependency/DecompressBBTest/CompressedFile1.cmp (COMPRE~1.CMP)
    Checking file /Dependency/DecompressBBTest/CompressedFile2.cmp (COMPRE~2.CMP)
    Checking file /Dependency/DecompressBBTest/UncompressedFile1.ucmp (UNCOMP~1.UCM)
    Checking file /Dependency/DecompressBBTest/UncompressedFile2.ucmp (UNCOMP~2.UCM)
    Checking file /Dependency/DeviceIoBBTest/.
    Checking file /Dependency/DeviceIoBBTest/..
    Checking file /Dependency/EbcBBTest/.
    Checking file /Dependency/EbcBBTest/..
    Checking file /Dependency/EbcBBTest/EbcDriver.efi (EBCDRI~1.EFI)
    Checking file /Dependency/LoadedImageBBTest/.
    Checking file /Dependency/LoadedImageBBTest/..
    Checking file /Dependency/LoadedImageBBTest/LoadedImageApplication1.efi (LOADED~1.EFI)
    Checking file /Dependency/LoadedImageBBTest/LoadedImageApplication2.efi (LOADED~2.EFI)
    Checking file /Dependency/LoadedImageBBTest/LoadedImageBootServicesDriver1.efi (LOADED~3.EFI)
    Checking file /Dependency/LoadedImageBBTest/LoadedImageBootServicesDriver2.efi (LOADED~4.EFI)
    Checking file /Dependency/LoadedImageBBTest/LoadedImageRuntimeServicesDriver1.efi (LOADED~5.EFI)
    Checking file /Dependency/LoadedImageBBTest/LoadedImageRuntimeServicesDriver2.efi (LOADED~6.EFI)
    Checking file /Dependency/PciIoBBTest/.
    Checking file /Dependency/PciIoBBTest/..
    Checking file /Dependency/PciIoBBTest/MakeConfigWritable.efi (MAKECO~1.EFI)
    Checking file /Dependency/PciIoBBTest/PciIoBBTest.ini (PCIIOB~1.INI)
    Checking file /Dependency/PciRootBridgeIoBBTest/.
    Checking file /Dependency/PciRootBridgeIoBBTest/..
    Checking file /Dependency/PciRootBridgeIoBBTest/PciRootBridgeIoBbTest.ini (PCIROO~1.INI)
    Checking file /Dependency/PxeBaseCodeBBTest/.
    Checking file /Dependency/PxeBaseCodeBBTest/..
    Checking file /Dependency/PxeBaseCodeBBTest/PxeBaseCodeBbTest.ini (PXEBAS~1.INI)
    Checking file /Dependency/ConfigKeywordHandlerBBTest/.
    Checking file /Dependency/ConfigKeywordHandlerBBTest/..
    Checking file /Dependency/ConfigKeywordHandlerBBTest/DriverSample.efi (DRIVER~1.EFI)
    Checking file /Ents/.
    Checking file /Ents/..
    Checking file /Ents/Support (SUPPORT)
    Checking file /Ents/Test (TEST)
    Checking file /Ents/Support/.
    Checking file /Ents/Support/..
    Checking file /Ents/Support/SerialMonitor.efi (SERIAL~1.EFI)
    Checking file /Ents/Support/ManagedNetworkMonitor.efi (MANAGE~1.EFI)
    Checking file /Ents/Support/IP4NetworkMonitor.efi (IP4NET~1.EFI)
    Checking file /Ents/Support/Eftp.efi (EFTP.EFI)
    Checking file /Ents/Test/.
    Checking file /Ents/Test/..
    Checking file /Ents/Test/BootService_ENTSTest.efi (BOOTSE~1.EFI)
    Checking file /Ents/Test/RuntimeService_ENTSTest.efi (RUNTIM~1.EFI)
    Checking file /Ents/Test/GenericService_ENTSTest.efi (GENERI~1.EFI)
    Checking file /Ents/Test/SimpleNetwork_ENTSTest.efi (SIMPLE~1.EFI)
    Checking file /Ents/Test/PXEBaseCode_ENTSTest.efi (PXEBAS~1.EFI)
    Checking file /Ents/Test/MnpSB_ENTSTest.efi (MNPSB_~1.EFI)
    Checking file /Ents/Test/Mnp_ENTSTest.efi (MNP_EN~1.EFI)
    Checking file /Ents/Test/ArpServiceBinding_ENTSTest.efi (ARPSER~1.EFI)
    Checking file /Ents/Test/Arp_ENTSTest.efi (ARP_EN~1.EFI)
    Checking file /Ents/Test/Ip4Config2_ENTSTest.efi (IP4CON~1.EFI)
    Checking file /Ents/Test/Ip4Config_ENTSTest.efi (IP4CON~2.EFI)
    Checking file /Ents/Test/Ip4ServiceBinding_ENTSTest.efi (IP4SER~1.EFI)
    Checking file /Ents/Test/Ip4_ENTSTest.efi (IP4_EN~1.EFI)
    Checking file /Ents/Test/Ip6Config_ENTSTest.efi (IP6CON~1.EFI)
    Checking file /Ents/Test/Ip6ServiceBinding_ENTSTest.efi (IP6SER~1.EFI)
    Checking file /Ents/Test/Ip6_ENTSTest.efi (IP6_EN~1.EFI)
    Checking file /Ents/Test/Udp4ServiceBinding_ENTSTest.efi (UDP4SE~1.EFI)
    Checking file /Ents/Test/Udp4_ENTSTest.efi (UDP4_E~1.EFI)
    Checking file /Ents/Test/Udp6ServiceBinding_ENTSTest.efi (UDP6SE~1.EFI)
    Checking file /Ents/Test/Udp6_ENTSTest.efi (UDP6_E~1.EFI)
    Checking file /Ents/Test/Dhcp4SB_ENTSTest.efi (DHCP4S~1.EFI)
    Checking file /Ents/Test/Dhcp4_ENTSTest.efi (DHCP4_~1.EFI)
    Checking file /Ents/Test/Dhcp6SB_ENTSTest.efi (DHCP6S~1.EFI)
    Checking file /Ents/Test/Dhcp6_ENTSTest.efi (DHCP6_~1.EFI)
    Checking file /Ents/Test/Mtftp4ServiceBinding_ENTSTest.efi (MTFTP4~1.EFI)
    Checking file /Ents/Test/Mtftp4_ENTSTest.efi (MTFTP4~2.EFI)
    Checking file /Ents/Test/Mtftp6ServiceBinding_ENTSTest.efi (MTFTP6~1.EFI)
    Checking file /Ents/Test/Mtftp6_ENTSTest.efi (MTFTP6~2.EFI)
    Checking file /Ents/Test/Tcp4ServiceBinding_ENTSTest.efi (TCP4SE~1.EFI)
    Checking file /Ents/Test/Tcp4_ENTSTest.efi (TCP4_E~1.EFI)
    Checking file /Ents/Test/Tcp6ServiceBinding_ENTSTest.efi (TCP6SE~1.EFI)
    Checking file /Ents/Test/Tcp6_ENTSTest.efi (TCP6_E~1.EFI)
    Checking file /Ents/Test/HttpServiceBinding_ENTSTest.efi (HTTPSE~1.EFI)
    Checking file /Ents/Test/Http_ENTSTest.efi (HTTP_E~1.EFI)
    Checking file /Proxy/.
    Checking file /Proxy/..
    Checking file /Report/.
    Checking file /Report/..
    Orphaned long file name part "PlatformConfig.ini"
      Auto-deleting.
    Checking file /Report/PlatformConfig.ini (PLATFO~1.INI)
    Checking file /SCRT/.
    Checking file /SCRT/..
    Checking file /SCRT/SCRTDRIVER.efi (SCRTDR~1.EFI)
    Checking file /SCRT/SCRTAPP.efi (SCRTAPP.EFI)
    Checking file /SCRT/SCRT.conf (SCRT~1.CON)
    Checking file /Sequence/.
    Checking file /Sequence/..
    Checking file /Sequence/uboot.seq (UBOOT.SEQ)
    Checking file /Support/.
    Checking file /Support/..
    Checking file /Support/StandardTest.efi (STANDA~1.EFI)
    Checking file /Support/TestProfile.efi (TESTPR~1.EFI)
    Checking file /Support/TestRecovery.efi (TESTRE~1.EFI)
    Checking file /Support/TestLogging.efi (TESTLO~1.EFI)
    Checking file /Test/.
    Checking file /Test/..
    Checking file /Test/EfiCompliantBBTest.efi (EFICOM~1.EFI)
    Checking file /Test/EventTimerTaskPriorityServicesBBTest.efi (EVENTT~1.EFI)
    Checking file /Test/MemoryAllocationServicesBBTest.efi (MEMORY~1.EFI)
    Checking file /Test/ProtocolHandlerServicesBBTest.efi (PROTOC~1.EFI)
    Checking file /Test/ImageServicesBBTest.efi (IMAGES~1.EFI)
    Checking file /Test/MiscBootServicesBBTest.efi (MISCBO~1.EFI)
    Checking file /Test/VariableServicesBBTest.efi (VARIAB~1.EFI)
    Checking file /Test/TimeServicesBBTest.efi (TIMESE~1.EFI)
    Checking file /Test/MiscRuntimeServicesBBTest.efi (MISCRU~1.EFI)
    Checking file /Test/BisBBTest.efi (BISBBT~1.EFI)
    Checking file /Test/BlockIoBBTest.efi (BLOCKI~1.EFI)
    Checking file /Test/BlockIo2BBTest.efi (BLOCKI~2.EFI)
    Checking file /Test/BusSpecificDriverOverrideBBTest.efi (BUSSPE~1.EFI)
    Checking file /Test/DebugPortBBTest.efi (DEBUGP~1.EFI)
    Checking file /Test/DebugSupportBBTest.efi (DEBUGS~1.EFI)
    Checking file /Test/DecompressBBTest.efi (DECOMP~1.EFI)
    Checking file /Test/DevicePathBBTest.efi (DEVICE~1.EFI)
    Checking file /Test/DevicePathUtilitiesBBTest.efi (DEVICE~2.EFI)
    Checking file /Test/DevicePathToTextBBTest.efi (DEVICE~3.EFI)
    Checking file /Test/DevicePathFromTextBBTest.efi (DEVICE~4.EFI)
    Checking file /Test/DiskIoBBTest.efi (DISKIO~1.EFI)
    Checking file /Test/EbcBBTest.efi (EBCBBT~1.EFI)
    Checking file /Test/LoadedImageBBTest.efi (LOADED~1.EFI)
    Checking file /Test/LoadFileBBTest.efi (LOADFI~1.EFI)
    Checking file /Test/PciIoBBTest.efi (PCIIOB~1.EFI)
    Checking file /Test/PciRootBridgeIoBBTest.efi (PCIROO~1.EFI)
    Checking file /Test/PlatformDriverOverrideBBTest.efi (PLATFO~1.EFI)
    Checking file /Test/PxeBaseCodeBBTest.efi (PXEBAS~1.EFI)
    Checking file /Test/ScsiIoBBTest.efi (SCSIIO~1.EFI)
    Checking file /Test/ExtScsiPassThruBBTest.efi (EXTSCS~1.EFI)
    Checking file /Test/AtaPassThruBBTest.efi (ATAPAS~1.EFI)
    Checking file /Test/iScsiInitiatorNameBBTest.efi (ISCSII~1.EFI)
    Checking file /Test/SerialIoBBTest.efi (SERIAL~1.EFI)
    Checking file /Test/SimpleFileSystemBBTest.efi (SIMPLE~1.EFI)
    Checking file /Test/SimpleNetworkBBTest.efi (SIMPLE~2.EFI)
    Checking file /Test/SimplePointerBBTest.efi (SIMPLE~3.EFI)
    Checking file /Test/SimpleTextInBBTest.efi (SIMPLE~4.EFI)
    Checking file /Test/SimpleTextOutBBTest.efi (SIMPLE~5.EFI)
    Checking file /Test/GraphicsOutputBBTest.efi (GRAPHI~1.EFI)
    Checking file /Test/UnicodeCollation2BBTest.efi (UNICOD~1.EFI)
    Checking file /Test/UsbIoTest.efi (USBIOT~1.EFI)
    Checking file /Test/Usb2HcTest.efi (USB2HC~1.EFI)
    Checking file /Test/TapeBBTest.efi (TAPEBB~1.EFI)
    Checking file /Test/AcpiTableProtocolBBTest.efi (ACPITA~1.EFI)
    Checking file /Test/SimpleTextInputExBBTest.efi (SIMPLE~6.EFI)
    Checking file /Test/ComponentName2BBTest.efi (COMPON~1.EFI)
    Checking file /Test/DriverDiagnostics2BBTest.efi (DRIVER~1.EFI)
    Checking file /Test/HIIDatabaseBBTest.efi (HIIDAT~1.EFI)
    Checking file /Test/HIIStringBBTest.efi (HIISTR~1.EFI)
    Checking file /Test/HIIFontBBTest.efi (HIIFON~1.EFI)
    Checking file /Test/HIIFontExBBTest.efi (HIIFON~2.EFI)
    Checking file /Test/HIIImageBBTest.efi (HIIIMA~1.EFI)
    Checking file /Test/HIIImageExBBTest.efi (HIIIMA~2.EFI)
    Checking file /Test/AbsolutePointerBBTest.efi (ABSOLU~1.EFI)
    Checking file /Test/PlatformToDriverConfigurationBBTest.efi (PLATFO~2.EFI)
    Checking file /Test/HIIConfigAccessBBTest.efi (HIICON~1.EFI)
    Checking file /Test/HIIConfigRoutingBBTest.efi (HIICON~2.EFI)
    Checking file /Test/VlanConfigBBTest.efi (VLANCO~1.EFI)
    Checking file /Test/IPsecConfigBBTest.efi (IPSECC~1.EFI)
    Checking file /Test/IPsec2BBTest.efi (IPSEC2~1.EFI)
    Checking file /Test/StorageSecurityCommandBBTest.efi (STORAG~1.EFI)
    Checking file /Test/FirmwareManagementBBTest.efi (FIRMWA~1.EFI)
    Checking file /Test/AdapterInfoBBTest.efi (ADAPTE~1.EFI)
    Checking file /Test/DiskIo2BBTest.efi (DISKIO~2.EFI)
    Checking file /Test/TimeStampBBTest.efi (TIMEST~1.EFI)
    Checking file /Test/RandomNumberBBTest.efi (RANDOM~1.EFI)
    Checking file /Test/Hash2BBTest.efi (HASH2B~1.EFI)
    Checking file /Test/Pkcs7BBTest.efi (PKCS7B~1.EFI)
    Checking file /Test/ConfigKeywordHandlerBBTest.efi (CONFIG~1.EFI)
    Checking file /Test/RegularExpressionBBTest.efi (REGULA~1.EFI)
    Checking file /Test/RamDiskProtocolBBTest.efi (RAMDIS~1.EFI)
    Checking file /Test/NVMEPassThruBBTest.efi (NVMEPA~1.EFI)
    Checking file /Test/EraseBlockBBTest.efi (ERASEB~1.EFI)
    Checking file /Test/SDMMCPassThruBBTest.efi (SDMMCP~1.EFI)
    Checking file /Test/PartitionInfoBBTest.efi (PARTIT~1.EFI)
    Checking file /Test/UFSDeviceConfigBBTest.efi (UFSDEV~1.EFI)
    Checking file /Test/ResetNotificationBBTest.efi (RESETN~1.EFI)
    Checking file /Overall/.
    Checking file /Overall/..
    Orphaned long file name part "Summary.log"
      Auto-deleting.
    Checking file /Overall/Summary.log (SUMMARY.LOG)
    Orphaned long file name part "Summary.ekl"
      Auto-deleting.
    Checking file /Overall/Summary.ekl (SUMMARY.EKL)
    Checking file /Log/.
    Checking file /Log/..
    Checking file /Log/BootServicesTest (BOOTSE~1)
    Checking file /Log/RuntimeServicesTest (RUNTIM~1)
    Checking file /Log/LoadedImageProtocolTest0 (LOADED~1)
    Checking file /Log/DevicePathProcotols (DEVICE~1)
    Checking file /Log/NetworkSupportTest (NETWOR~1)
    Checking file /Log/StringServiceTest (STRING~1)
    Checking file /Log/ConsoleSupportTest (CONSOL~1)
    Checking file /Log/GenericTest (GENERI~1)
    Checking file /Log/MediaAccessTest (MEDIAA~1)
    Checking file /Log/HIITest (HIITEST)
    Checking file /Log/SecureTechTest (SECURE~1)
    Checking file /Log/BootServicesTest/.
    Checking file /Log/BootServicesTest/..
    Checking file /Log/BootServicesTest/EventTimerandPriorityServicesTest0 (EVENTT~1)
    Checking file /Log/BootServicesTest/MemoryAllocationServicesTest0 (MEMORY~1)
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0 (PROTOC~1)
    Checking file /Log/BootServicesTest/ImageServicesTest0 (IMAGES~1)
    Checking file /Log/BootServicesTest/MiscBootServicesTest0 (MISCBO~1)
    Checking file /Log/BootServicesTest/EventTimerandPriorityServicesTest0/.
    Checking file /Log/BootServicesTest/EventTimerandPriorityServicesTest0/..
    Orphaned long file name part "CheckEvent_Conf_0_0_C4A57D1B-59CD-4722-A7FE-DF79446D0332.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/EventTimerandPriorityServicesTest0/CheckEvent_Conf_0_0_C4A57D1B-59CD-4722-A7FE-DF79446D0332.log (CHECKE~1.LOG)
    Orphaned long file name part "CheckEvent_Conf_0_0_C4A57D1B-59CD-4722-A7FE-DF79446D0332.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/EventTimerandPriorityServicesTest0/CheckEvent_Conf_0_0_C4A57D1B-59CD-4722-A7FE-DF79446D0332.ekl (CHECKE~1.EKL)
    Orphaned long file name part "CheckEvent_Func_0_0_29481844-C567-4A8D-B92F-D57B32F039B8.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/EventTimerandPriorityServicesTest0/CheckEvent_Func_0_0_29481844-C567-4A8D-B92F-D57B32F039B8.log (CHECKE~1.LOG)
    Orphaned long file name part "CheckEvent_Func_0_0_29481844-C567-4A8D-B92F-D57B32F039B8.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/EventTimerandPriorityServicesTest0/CheckEvent_Func_0_0_29481844-C567-4A8D-B92F-D57B32F039B8.ekl (CHECKE~1.EKL)
    Orphaned long file name part "CloseEvent_Func_0_0_EFBD4523-10DD-44B3-A520-58AF83E5BF64.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/EventTimerandPriorityServicesTest0/CloseEvent_Func_0_0_EFBD4523-10DD-44B3-A520-58AF83E5BF64.log (CLOSEE~1.LOG)
    Orphaned long file name part "CloseEvent_Func_0_0_EFBD4523-10DD-44B3-A520-58AF83E5BF64.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/EventTimerandPriorityServicesTest0/CloseEvent_Func_0_0_EFBD4523-10DD-44B3-A520-58AF83E5BF64.ekl (CLOSEE~1.EKL)
    Orphaned long file name part "CreateEventEx_Conf_0_0_F9B16C34-EAB5-4C9C-BE90-01B12E64F117.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/EventTimerandPriorityServicesTest0/CreateEventEx_Conf_0_0_F9B16C34-EAB5-4C9C-BE90-01B12E64F117.log (CREATE~1.LOG)
    Orphaned long file name part "CreateEventEx_Conf_0_0_F9B16C34-EAB5-4C9C-BE90-01B12E64F117.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/EventTimerandPriorityServicesTest0/CreateEventEx_Conf_0_0_F9B16C34-EAB5-4C9C-BE90-01B12E64F117.ekl (CREATE~1.EKL)
    Orphaned long file name part "CreateEventEx_Func_0_0_0F9FA263-7396-4759-8F4C-EFC6B6F159B8.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/EventTimerandPriorityServicesTest0/CreateEventEx_Func_0_0_0F9FA263-7396-4759-8F4C-EFC6B6F159B8.log (CREATE~1.LOG)
    Orphaned long file name part "CreateEventEx_Func_0_0_0F9FA263-7396-4759-8F4C-EFC6B6F159B8.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/EventTimerandPriorityServicesTest0/CreateEventEx_Func_0_0_0F9FA263-7396-4759-8F4C-EFC6B6F159B8.ekl (CREATE~1.EKL)
    Orphaned long file name part "CreateEvent_Conf_0_0_50BF9D26-B53D-4CFF-BC10-BC6581BF509D.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/EventTimerandPriorityServicesTest0/CreateEvent_Conf_0_0_50BF9D26-B53D-4CFF-BC10-BC6581BF509D.log (CREATE~1.LOG)
    Orphaned long file name part "CreateEvent_Conf_0_0_50BF9D26-B53D-4CFF-BC10-BC6581BF509D.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/EventTimerandPriorityServicesTest0/CreateEvent_Conf_0_0_50BF9D26-B53D-4CFF-BC10-BC6581BF509D.ekl (CREATE~1.EKL)
    Orphaned long file name part "CreateEvent_Func_0_0_83CF7F0B-C274-4918-AEA6-413DA9CF68CF.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/EventTimerandPriorityServicesTest0/CreateEvent_Func_0_0_83CF7F0B-C274-4918-AEA6-413DA9CF68CF.log (CREATE~1.LOG)
    Orphaned long file name part "CreateEvent_Func_0_0_83CF7F0B-C274-4918-AEA6-413DA9CF68CF.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/EventTimerandPriorityServicesTest0/CreateEvent_Func_0_0_83CF7F0B-C274-4918-AEA6-413DA9CF68CF.ekl (CREATE~1.EKL)
    Orphaned long file name part "RaiseTPL_Func_0_0_D4A835EB-0830-4C7A-B306-2E3ECAB4A694.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/EventTimerandPriorityServicesTest0/RaiseTPL_Func_0_0_D4A835EB-0830-4C7A-B306-2E3ECAB4A694.log (RAISET~1.LOG)
    Orphaned long file name part "RaiseTPL_Func_0_0_D4A835EB-0830-4C7A-B306-2E3ECAB4A694.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/EventTimerandPriorityServicesTest0/RaiseTPL_Func_0_0_D4A835EB-0830-4C7A-B306-2E3ECAB4A694.ekl (RAISET~1.EKL)
    Orphaned long file name part "RestoreTPL_Func_0_0_8C096F99-268C-42FC-A6C0-E10EB70506C0.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/EventTimerandPriorityServicesTest0/RestoreTPL_Func_0_0_8C096F99-268C-42FC-A6C0-E10EB70506C0.log (RESTOR~1.LOG)
    Orphaned long file name part "RestoreTPL_Func_0_0_8C096F99-268C-42FC-A6C0-E10EB70506C0.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/EventTimerandPriorityServicesTest0/RestoreTPL_Func_0_0_8C096F99-268C-42FC-A6C0-E10EB70506C0.ekl (RESTOR~1.EKL)
    Orphaned long file name part "SetTimer_Conf_0_0_0BDE93B5-BC1E-4B6D-A960-2FBE3888ADCC.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/EventTimerandPriorityServicesTest0/SetTimer_Conf_0_0_0BDE93B5-BC1E-4B6D-A960-2FBE3888ADCC.log (SETTIM~1.LOG)
    Orphaned long file name part "SetTimer_Conf_0_0_0BDE93B5-BC1E-4B6D-A960-2FBE3888ADCC.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/EventTimerandPriorityServicesTest0/SetTimer_Conf_0_0_0BDE93B5-BC1E-4B6D-A960-2FBE3888ADCC.ekl (SETTIM~1.EKL)
    Orphaned long file name part "SetTimer_Func_0_0_86BAAB81-D547-45F5-AE0F-8647FE91559D.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/EventTimerandPriorityServicesTest0/SetTimer_Func_0_0_86BAAB81-D547-45F5-AE0F-8647FE91559D.log (SETTIM~1.LOG)
    Orphaned long file name part "SetTimer_Func_0_0_86BAAB81-D547-45F5-AE0F-8647FE91559D.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/EventTimerandPriorityServicesTest0/SetTimer_Func_0_0_86BAAB81-D547-45F5-AE0F-8647FE91559D.ekl (SETTIM~1.EKL)
    Orphaned long file name part "SignalEvent_Func_0_0_8C3860C8-DF25-4B8D-98B6-07791D661F5D.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/EventTimerandPriorityServicesTest0/SignalEvent_Func_0_0_8C3860C8-DF25-4B8D-98B6-07791D661F5D.log (SIGNAL~1.LOG)
    Orphaned long file name part "SignalEvent_Func_0_0_8C3860C8-DF25-4B8D-98B6-07791D661F5D.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/EventTimerandPriorityServicesTest0/SignalEvent_Func_0_0_8C3860C8-DF25-4B8D-98B6-07791D661F5D.ekl (SIGNAL~1.EKL)
    Orphaned long file name part "WaitForEvent_Conf_0_0_69442339-151E-4EAA-A2B6-84F789D60D83.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/EventTimerandPriorityServicesTest0/WaitForEvent_Conf_0_0_69442339-151E-4EAA-A2B6-84F789D60D83.log (WAITFO~1.LOG)
    Orphaned long file name part "WaitForEvent_Conf_0_0_69442339-151E-4EAA-A2B6-84F789D60D83.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/EventTimerandPriorityServicesTest0/WaitForEvent_Conf_0_0_69442339-151E-4EAA-A2B6-84F789D60D83.ekl (WAITFO~1.EKL)
    Orphaned long file name part "WaitForEvent_Func_0_0_A64FFBC1-6B44-45BB-973A-887D91FE4A6B.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/EventTimerandPriorityServicesTest0/WaitForEvent_Func_0_0_A64FFBC1-6B44-45BB-973A-887D91FE4A6B.log (WAITFO~1.LOG)
    Orphaned long file name part "WaitForEvent_Func_0_0_A64FFBC1-6B44-45BB-973A-887D91FE4A6B.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/EventTimerandPriorityServicesTest0/WaitForEvent_Func_0_0_A64FFBC1-6B44-45BB-973A-887D91FE4A6B.ekl (WAITFO~1.EKL)
    /Log/BootServicesTest/EventTimerandPriorityServicesTest0/CheckEvent_Conf_0_0_C4A57D1B-59CD-4722-A7FE-DF79446D0332.log
      Duplicate directory entry.
      First    Size 3256 bytes, date 01:00:00 Jan 01 1980
      Second   Size 4970 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.000
    /Log/BootServicesTest/EventTimerandPriorityServicesTest0/CheckEvent_Conf_0_0_C4A57D1B-59CD-4722-A7FE-DF79446D0332.ekl
      Duplicate directory entry.
      First    Size 1272 bytes, date 01:00:00 Jan 01 1980
      Second   Size 2958 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.001
    /Log/BootServicesTest/EventTimerandPriorityServicesTest0/CreateEventEx_Conf_0_0_F9B16C34-EAB5-4C9C-BE90-01B12E64F117.log
      Duplicate directory entry.
      First    Size 56964 bytes, date 01:00:00 Jan 01 1980
      Second   Size 4874 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.002
    /Log/BootServicesTest/EventTimerandPriorityServicesTest0/CreateEventEx_Conf_0_0_F9B16C34-EAB5-4C9C-BE90-01B12E64F117.log
      Duplicate directory entry.
      First    Size 56964 bytes, date 01:00:00 Jan 01 1980
      Second   Size 24866 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.003
    /Log/BootServicesTest/EventTimerandPriorityServicesTest0/CreateEventEx_Conf_0_0_F9B16C34-EAB5-4C9C-BE90-01B12E64F117.log
      Duplicate directory entry.
      First    Size 56964 bytes, date 01:00:00 Jan 01 1980
      Second   Size 11910 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.004
    /Log/BootServicesTest/EventTimerandPriorityServicesTest0/CreateEventEx_Conf_0_0_F9B16C34-EAB5-4C9C-BE90-01B12E64F117.ekl
      Duplicate directory entry.
      First    Size 54284 bytes, date 01:00:00 Jan 01 1980
      Second   Size 2848 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.005
    /Log/BootServicesTest/EventTimerandPriorityServicesTest0/CreateEventEx_Conf_0_0_F9B16C34-EAB5-4C9C-BE90-01B12E64F117.ekl
      Duplicate directory entry.
      First    Size 54284 bytes, date 01:00:00 Jan 01 1980
      Second   Size 22562 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.006
    /Log/BootServicesTest/EventTimerandPriorityServicesTest0/CreateEventEx_Conf_0_0_F9B16C34-EAB5-4C9C-BE90-01B12E64F117.ekl
      Duplicate directory entry.
      First    Size 54284 bytes, date 01:00:00 Jan 01 1980
      Second   Size 9798 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.007
    /Log/BootServicesTest/EventTimerandPriorityServicesTest0/SetTimer_Conf_0_0_0BDE93B5-BC1E-4B6D-A960-2FBE3888ADCC.log
      Duplicate directory entry.
      First    Size 5150 bytes, date 01:00:00 Jan 01 1980
      Second   Size 6038 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.008
    /Log/BootServicesTest/EventTimerandPriorityServicesTest0/SetTimer_Conf_0_0_0BDE93B5-BC1E-4B6D-A960-2FBE3888ADCC.ekl
      Duplicate directory entry.
      First    Size 3152 bytes, date 01:00:00 Jan 01 1980
      Second   Size 4022 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.009
    /Log/BootServicesTest/EventTimerandPriorityServicesTest0/WaitForEvent_Conf_0_0_69442339-151E-4EAA-A2B6-84F789D60D83.log
      Duplicate directory entry.
      First    Size 5140 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3920 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.010
    /Log/BootServicesTest/EventTimerandPriorityServicesTest0/WaitForEvent_Conf_0_0_69442339-151E-4EAA-A2B6-84F789D60D83.ekl
      Duplicate directory entry.
      First    Size 3110 bytes, date 01:00:00 Jan 01 1980
      Second   Size 1912 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.011
    Checking file /Log/BootServicesTest/MemoryAllocationServicesTest0/.
    Checking file /Log/BootServicesTest/MemoryAllocationServicesTest0/..
    Orphaned long file name part "AllocatePages_Conf_0_0_4E87315F-BAD6-4B90-88C3-2972B1F9ACBE.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/MemoryAllocationServicesTest0/AllocatePages_Conf_0_0_4E87315F-BAD6-4B90-88C3-2972B1F9ACBE.log (ALLOCA~1.LOG)
    Orphaned long file name part "AllocatePages_Conf_0_0_4E87315F-BAD6-4B90-88C3-2972B1F9ACBE.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/MemoryAllocationServicesTest0/AllocatePages_Conf_0_0_4E87315F-BAD6-4B90-88C3-2972B1F9ACBE.ekl (ALLOCA~1.EKL)
    Orphaned long file name part "AllocatePages_Func_0_0_21338335-67BA-4392-8D5E-7184C6D601A6.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/MemoryAllocationServicesTest0/AllocatePages_Func_0_0_21338335-67BA-4392-8D5E-7184C6D601A6.log (ALLOCA~1.LOG)
    Orphaned long file name part "AllocatePages_Func_0_0_21338335-67BA-4392-8D5E-7184C6D601A6.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/MemoryAllocationServicesTest0/AllocatePages_Func_0_0_21338335-67BA-4392-8D5E-7184C6D601A6.ekl (ALLOCA~1.EKL)
    Orphaned long file name part "AllocatePool_Conf_0_0_90023546-6C92-430A-B253-70110D9EFDFF.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/MemoryAllocationServicesTest0/AllocatePool_Conf_0_0_90023546-6C92-430A-B253-70110D9EFDFF.log (ALLOCA~1.LOG)
    Orphaned long file name part "AllocatePool_Conf_0_0_90023546-6C92-430A-B253-70110D9EFDFF.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/MemoryAllocationServicesTest0/AllocatePool_Conf_0_0_90023546-6C92-430A-B253-70110D9EFDFF.ekl (ALLOCA~1.EKL)
    Orphaned long file name part "AllocatePool_Func_0_0_04D5B638-E15A-4839-9E7A-6F1F6A3C5888.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/MemoryAllocationServicesTest0/AllocatePool_Func_0_0_04D5B638-E15A-4839-9E7A-6F1F6A3C5888.log (ALLOCA~1.LOG)
    Orphaned long file name part "AllocatePool_Func_0_0_04D5B638-E15A-4839-9E7A-6F1F6A3C5888.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/MemoryAllocationServicesTest0/AllocatePool_Func_0_0_04D5B638-E15A-4839-9E7A-6F1F6A3C5888.ekl (ALLOCA~1.EKL)
    Orphaned long file name part "FreePages_Conf_0_0_F30940B6-DE0D-47B2-BEBE-E1C20C9213E9.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/MemoryAllocationServicesTest0/FreePages_Conf_0_0_F30940B6-DE0D-47B2-BEBE-E1C20C9213E9.log (FREEPA~1.LOG)
    Orphaned long file name part "FreePages_Conf_0_0_F30940B6-DE0D-47B2-BEBE-E1C20C9213E9.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/MemoryAllocationServicesTest0/FreePages_Conf_0_0_F30940B6-DE0D-47B2-BEBE-E1C20C9213E9.ekl (FREEPA~1.EKL)
    Orphaned long file name part "FreePages_Func_0_0_2CF12F16-962E-439D-A1BF-4E915184EBAE.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/MemoryAllocationServicesTest0/FreePages_Func_0_0_2CF12F16-962E-439D-A1BF-4E915184EBAE.log (FREEPA~1.LOG)
    Orphaned long file name part "FreePages_Func_0_0_2CF12F16-962E-439D-A1BF-4E915184EBAE.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/MemoryAllocationServicesTest0/FreePages_Func_0_0_2CF12F16-962E-439D-A1BF-4E915184EBAE.ekl (FREEPA~1.EKL)
    Orphaned long file name part "FreePool_Conf_0_0_49709F9F-A4D8-42D6-A684-4975EE0099DB.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/MemoryAllocationServicesTest0/FreePool_Conf_0_0_49709F9F-A4D8-42D6-A684-4975EE0099DB.log (FREEPO~1.LOG)
    Orphaned long file name part "FreePool_Conf_0_0_49709F9F-A4D8-42D6-A684-4975EE0099DB.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/MemoryAllocationServicesTest0/FreePool_Conf_0_0_49709F9F-A4D8-42D6-A684-4975EE0099DB.ekl (FREEPO~1.EKL)
    Orphaned long file name part "FreePool_Func_0_0_D9980A61-670B-4078-9049-1309FCEC7106.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/MemoryAllocationServicesTest0/FreePool_Func_0_0_D9980A61-670B-4078-9049-1309FCEC7106.log (FREEPO~1.LOG)
    Orphaned long file name part "FreePool_Func_0_0_D9980A61-670B-4078-9049-1309FCEC7106.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/MemoryAllocationServicesTest0/FreePool_Func_0_0_D9980A61-670B-4078-9049-1309FCEC7106.ekl (FREEPO~1.EKL)
    Orphaned long file name part "GetMemoryMap_Conf_0_0_2C437186-D178-40CF-A7B1-A2E86AF06D86.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/MemoryAllocationServicesTest0/GetMemoryMap_Conf_0_0_2C437186-D178-40CF-A7B1-A2E86AF06D86.log (GETMEM~1.LOG)
    Orphaned long file name part "GetMemoryMap_Conf_0_0_2C437186-D178-40CF-A7B1-A2E86AF06D86.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/MemoryAllocationServicesTest0/GetMemoryMap_Conf_0_0_2C437186-D178-40CF-A7B1-A2E86AF06D86.ekl (GETMEM~1.EKL)
    Orphaned long file name part "GetMemoryMap_Func_0_0_0CDE8BE7-85DC-4E7C-A584-566A643A3562.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/MemoryAllocationServicesTest0/GetMemoryMap_Func_0_0_0CDE8BE7-85DC-4E7C-A584-566A643A3562.log (GETMEM~1.LOG)
    Orphaned long file name part "GetMemoryMap_Func_0_0_0CDE8BE7-85DC-4E7C-A584-566A643A3562.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/MemoryAllocationServicesTest0/GetMemoryMap_Func_0_0_0CDE8BE7-85DC-4E7C-A584-566A643A3562.ekl (GETMEM~1.EKL)
    /Log/BootServicesTest/MemoryAllocationServicesTest0/AllocatePages_Conf_0_0_4E87315F-BAD6-4B90-88C3-2972B1F9ACBE.log
      Duplicate directory entry.
      First    Size 9244 bytes, date 01:00:00 Jan 01 1980
      Second   Size 790594 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.000
    /Log/BootServicesTest/MemoryAllocationServicesTest0/AllocatePages_Conf_0_0_4E87315F-BAD6-4B90-88C3-2972B1F9ACBE.log
      Duplicate directory entry.
      First    Size 9244 bytes, date 01:00:00 Jan 01 1980
      Second   Size 6466 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.001
    /Log/BootServicesTest/MemoryAllocationServicesTest0/AllocatePages_Conf_0_0_4E87315F-BAD6-4B90-88C3-2972B1F9ACBE.log
      Duplicate directory entry.
      First    Size 9244 bytes, date 01:00:00 Jan 01 1980
      Second   Size 28668 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.002
    /Log/BootServicesTest/MemoryAllocationServicesTest0/AllocatePages_Conf_0_0_4E87315F-BAD6-4B90-88C3-2972B1F9ACBE.ekl
      Duplicate directory entry.
      First    Size 7138 bytes, date 01:00:00 Jan 01 1980
      Second   Size 774688 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.003
    /Log/BootServicesTest/MemoryAllocationServicesTest0/AllocatePages_Conf_0_0_4E87315F-BAD6-4B90-88C3-2972B1F9ACBE.ekl
      Duplicate directory entry.
      First    Size 7138 bytes, date 01:00:00 Jan 01 1980
      Second   Size 4420 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.004
    /Log/BootServicesTest/MemoryAllocationServicesTest0/AllocatePages_Conf_0_0_4E87315F-BAD6-4B90-88C3-2972B1F9ACBE.ekl
      Duplicate directory entry.
      First    Size 7138 bytes, date 01:00:00 Jan 01 1980
      Second   Size 26214 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.005
    /Log/BootServicesTest/MemoryAllocationServicesTest0/FreePages_Conf_0_0_F30940B6-DE0D-47B2-BEBE-E1C20C9213E9.log
      Duplicate directory entry.
      First    Size 4212 bytes, date 01:00:00 Jan 01 1980
      Second   Size 28350 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.006
    /Log/BootServicesTest/MemoryAllocationServicesTest0/FreePages_Conf_0_0_F30940B6-DE0D-47B2-BEBE-E1C20C9213E9.ekl
      Duplicate directory entry.
      First    Size 2230 bytes, date 01:00:00 Jan 01 1980
      Second   Size 25920 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.007
    /Log/BootServicesTest/MemoryAllocationServicesTest0/FreePool_Conf_0_0_49709F9F-A4D8-42D6-A684-4975EE0099DB.log
      Duplicate directory entry.
      First    Size 3116 bytes, date 01:00:00 Jan 01 1980
      Second   Size 28244 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.008
    /Log/BootServicesTest/MemoryAllocationServicesTest0/FreePool_Conf_0_0_49709F9F-A4D8-42D6-A684-4975EE0099DB.ekl
      Duplicate directory entry.
      First    Size 1162 bytes, date 01:00:00 Jan 01 1980
      Second   Size 25822 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.009
    /Log/BootServicesTest/MemoryAllocationServicesTest0/GetMemoryMap_Conf_0_0_2C437186-D178-40CF-A7B1-A2E86AF06D86.log
      Duplicate directory entry.
      First    Size 4836 bytes, date 01:00:00 Jan 01 1980
      Second   Size 10502 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.010
    /Log/BootServicesTest/MemoryAllocationServicesTest0/GetMemoryMap_Conf_0_0_2C437186-D178-40CF-A7B1-A2E86AF06D86.ekl
      Duplicate directory entry.
      First    Size 2820 bytes, date 01:00:00 Jan 01 1980
      Second   Size 8378 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.011
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/..
    Orphaned long file name part "CloseProtocol_Conf_0_0_85302E6F-328B-407B-BD6D-835DD54BA54B.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/CloseProtocol_Conf_0_0_85302E6F-328B-407B-BD6D-835DD54BA54B.log (CLOSEP~1.LOG)
    Orphaned long file name part "CloseProtocol_Conf_0_0_85302E6F-328B-407B-BD6D-835DD54BA54B.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/CloseProtocol_Conf_0_0_85302E6F-328B-407B-BD6D-835DD54BA54B.ekl (CLOSEP~1.EKL)
    Orphaned long file name part "CloseProtocol_Func_0_0_11B44246-A65E-4832-8589-8F606929C9FB.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/CloseProtocol_Func_0_0_11B44246-A65E-4832-8589-8F606929C9FB.log (CLOSEP~1.LOG)
    Orphaned long file name part "CloseProtocol_Func_0_0_11B44246-A65E-4832-8589-8F606929C9FB.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/CloseProtocol_Func_0_0_11B44246-A65E-4832-8589-8F606929C9FB.ekl (CLOSEP~1.EKL)
    Orphaned long file name part "ConnectController_Conf_0_0_B6C90CCE-9063-4A76-B82D-CAD4191E7514.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/ConnectController_Conf_0_0_B6C90CCE-9063-4A76-B82D-CAD4191E7514.log (CONNEC~1.LOG)
    Orphaned long file name part "ConnectController_Conf_0_0_B6C90CCE-9063-4A76-B82D-CAD4191E7514.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/ConnectController_Conf_0_0_B6C90CCE-9063-4A76-B82D-CAD4191E7514.ekl (CONNEC~1.EKL)
    Orphaned long file name part "ConnectController_Func_0_0_705E2497-1B8F-4307-91E1-F33F2F2B5506.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/ConnectController_Func_0_0_705E2497-1B8F-4307-91E1-F33F2F2B5506.log (CONNEC~1.LOG)
    Orphaned long file name part "ConnectController_Func_0_0_705E2497-1B8F-4307-91E1-F33F2F2B5506.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/ConnectController_Func_0_0_705E2497-1B8F-4307-91E1-F33F2F2B5506.ekl (CONNEC~1.EKL)
    Orphaned long file name part "DisconnectController_Conf_0_0_94EEDBEC-55CA-442E-B99F-0788B8E51C10.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/DisconnectController_Conf_0_0_94EEDBEC-55CA-442E-B99F-0788B8E51C10.log (DISCON~1.LOG)
    Orphaned long file name part "DisconnectController_Conf_0_0_94EEDBEC-55CA-442E-B99F-0788B8E51C10.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/DisconnectController_Conf_0_0_94EEDBEC-55CA-442E-B99F-0788B8E51C10.ekl (DISCON~1.EKL)
    Orphaned long file name part "DisconnectController_Func_0_0_2AEEA797-C967-463E-BBBC-1D2490D17C91.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/DisconnectController_Func_0_0_2AEEA797-C967-463E-BBBC-1D2490D17C91.log (DISCON~1.LOG)
    Orphaned long file name part "DisconnectController_Func_0_0_2AEEA797-C967-463E-BBBC-1D2490D17C91.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/DisconnectController_Func_0_0_2AEEA797-C967-463E-BBBC-1D2490D17C91.ekl (DISCON~1.EKL)
    Orphaned long file name part "HandleProtocol_Conf_0_0_231E4965-FDA4-4FA2-8AE2-8C7902C507E9.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/HandleProtocol_Conf_0_0_231E4965-FDA4-4FA2-8AE2-8C7902C507E9.log (HANDLE~1.LOG)
    Orphaned long file name part "HandleProtocol_Conf_0_0_231E4965-FDA4-4FA2-8AE2-8C7902C507E9.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/HandleProtocol_Conf_0_0_231E4965-FDA4-4FA2-8AE2-8C7902C507E9.ekl (HANDLE~1.EKL)
    Orphaned long file name part "HandleProtocol_Func_0_0_D689E19D-54FE-40DC-9118-B9ABF2C00048.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/HandleProtocol_Func_0_0_D689E19D-54FE-40DC-9118-B9ABF2C00048.log (HANDLE~1.LOG)
    Orphaned long file name part "HandleProtocol_Func_0_0_D689E19D-54FE-40DC-9118-B9ABF2C00048.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/HandleProtocol_Func_0_0_D689E19D-54FE-40DC-9118-B9ABF2C00048.ekl (HANDLE~1.EKL)
    Orphaned long file name part "InstallMultipleProtocolInterfaces_Conf_0_0_B6DE8DE0-7375-4804-A029-9ED0CB43F74D.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/InstallMultipleProtocolInterfaces_Conf_0_0_B6DE8DE0-7375-4804-A029-9ED0CB43F74D.log (INSTAL~1.LOG)
    Orphaned long file name part "InstallMultipleProtocolInterfaces_Conf_0_0_B6DE8DE0-7375-4804-A029-9ED0CB43F74D.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/InstallMultipleProtocolInterfaces_Conf_0_0_B6DE8DE0-7375-4804-A029-9ED0CB43F74D.ekl (INSTAL~1.EKL)
    Orphaned long file name part "InstallMultipleProtocolInterfaces_Func_0_0_717259A7-658C-4616-B52C-6C8F661EA726.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/InstallMultipleProtocolInterfaces_Func_0_0_717259A7-658C-4616-B52C-6C8F661EA726.log (INSTAL~1.LOG)
    Orphaned long file name part "InstallMultipleProtocolInterfaces_Func_0_0_717259A7-658C-4616-B52C-6C8F661EA726.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/InstallMultipleProtocolInterfaces_Func_0_0_717259A7-658C-4616-B52C-6C8F661EA726.ekl (INSTAL~1.EKL)
    Orphaned long file name part "InstallProtocolInterface_Conf_0_0_6DF68724-5D03-4555-9FDC-AB4CE42B4509.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/InstallProtocolInterface_Conf_0_0_6DF68724-5D03-4555-9FDC-AB4CE42B4509.log (INSTAL~1.LOG)
    Orphaned long file name part "InstallProtocolInterface_Conf_0_0_6DF68724-5D03-4555-9FDC-AB4CE42B4509.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/InstallProtocolInterface_Conf_0_0_6DF68724-5D03-4555-9FDC-AB4CE42B4509.ekl (INSTAL~1.EKL)
    Orphaned long file name part "InstallProtocolInterface_Func_0_0_EDC7240B-6A14-45D4-937B-A2B62C51127B.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/InstallProtocolInterface_Func_0_0_EDC7240B-6A14-45D4-937B-A2B62C51127B.log (INSTAL~1.LOG)
    Orphaned long file name part "InstallProtocolInterface_Func_0_0_EDC7240B-6A14-45D4-937B-A2B62C51127B.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/InstallProtocolInterface_Func_0_0_EDC7240B-6A14-45D4-937B-A2B62C51127B.ekl (INSTAL~1.EKL)
    Orphaned long file name part "LocateDevicePath_Conf_0_0_624E28E8-78BC-4D77-AB85-D2CBD3744E21.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/LocateDevicePath_Conf_0_0_624E28E8-78BC-4D77-AB85-D2CBD3744E21.log (LOCATE~1.LOG)
    Orphaned long file name part "LocateDevicePath_Conf_0_0_624E28E8-78BC-4D77-AB85-D2CBD3744E21.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/LocateDevicePath_Conf_0_0_624E28E8-78BC-4D77-AB85-D2CBD3744E21.ekl (LOCATE~1.EKL)
    Orphaned long file name part "LocateDevicePath_Func_0_0_8E436AAF-37E9-4190-8DC7-5799D4769B19.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/LocateDevicePath_Func_0_0_8E436AAF-37E9-4190-8DC7-5799D4769B19.log (LOCATE~1.LOG)
    Orphaned long file name part "LocateDevicePath_Func_0_0_8E436AAF-37E9-4190-8DC7-5799D4769B19.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/LocateDevicePath_Func_0_0_8E436AAF-37E9-4190-8DC7-5799D4769B19.ekl (LOCATE~1.EKL)
    Orphaned long file name part "LocateHandleBuffer_Conf_0_0_6BAE06D3-3BE7-480E-9E71-332AD0C8213E.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/LocateHandleBuffer_Conf_0_0_6BAE06D3-3BE7-480E-9E71-332AD0C8213E.log (LOCATE~1.LOG)
    Orphaned long file name part "LocateHandleBuffer_Conf_0_0_6BAE06D3-3BE7-480E-9E71-332AD0C8213E.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/LocateHandleBuffer_Conf_0_0_6BAE06D3-3BE7-480E-9E71-332AD0C8213E.ekl (LOCATE~1.EKL)
    Orphaned long file name part "LocateHandleBuffer_Func_0_0_A21FFA59-09A2-46D4-A1FF-94D5C6061491.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/LocateHandleBuffer_Func_0_0_A21FFA59-09A2-46D4-A1FF-94D5C6061491.log (LOCATE~1.LOG)
    Orphaned long file name part "LocateHandleBuffer_Func_0_0_A21FFA59-09A2-46D4-A1FF-94D5C6061491.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/LocateHandleBuffer_Func_0_0_A21FFA59-09A2-46D4-A1FF-94D5C6061491.ekl (LOCATE~1.EKL)
    Orphaned long file name part "LocateHandle_Conf_0_0_A829FD94-B308-4B8F-873F-1EAFF35464BC.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/LocateHandle_Conf_0_0_A829FD94-B308-4B8F-873F-1EAFF35464BC.log (LOCATE~1.LOG)
    Orphaned long file name part "LocateHandle_Conf_0_0_A829FD94-B308-4B8F-873F-1EAFF35464BC.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/LocateHandle_Conf_0_0_A829FD94-B308-4B8F-873F-1EAFF35464BC.ekl (LOCATE~1.EKL)
    Orphaned long file name part "LocateHandle_Func_0_0_11779290-1B6E-4A3F-ABAD-0816EBCA6E5F.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/LocateHandle_Func_0_0_11779290-1B6E-4A3F-ABAD-0816EBCA6E5F.log (LOCATE~1.LOG)
    Orphaned long file name part "LocateHandle_Func_0_0_11779290-1B6E-4A3F-ABAD-0816EBCA6E5F.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/LocateHandle_Func_0_0_11779290-1B6E-4A3F-ABAD-0816EBCA6E5F.ekl (LOCATE~1.EKL)
    Orphaned long file name part "LocateProtocol_Conf_0_0_852C03C5-5FF1-48E6-A8A4-496EA1148A33.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/LocateProtocol_Conf_0_0_852C03C5-5FF1-48E6-A8A4-496EA1148A33.log (LOCATE~1.LOG)
    Orphaned long file name part "LocateProtocol_Conf_0_0_852C03C5-5FF1-48E6-A8A4-496EA1148A33.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/LocateProtocol_Conf_0_0_852C03C5-5FF1-48E6-A8A4-496EA1148A33.ekl (LOCATE~1.EKL)
    Orphaned long file name part "LocateProtocol_Func_0_0_E5D3C7D0-1CF8-4CC1-8F00-CC91ACF2889E.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/LocateProtocol_Func_0_0_E5D3C7D0-1CF8-4CC1-8F00-CC91ACF2889E.log (LOCATE~1.LOG)
    Orphaned long file name part "LocateProtocol_Func_0_0_E5D3C7D0-1CF8-4CC1-8F00-CC91ACF2889E.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/LocateProtocol_Func_0_0_E5D3C7D0-1CF8-4CC1-8F00-CC91ACF2889E.ekl (LOCATE~1.EKL)
    Orphaned long file name part "OpenProtocolInformation_Conf_0_0_6B57A087-F432-4DA7-AB65-A3BC2F2CE3F1.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/OpenProtocolInformation_Conf_0_0_6B57A087-F432-4DA7-AB65-A3BC2F2CE3F1.log (OPENPR~1.LOG)
    Orphaned long file name part "OpenProtocolInformation_Conf_0_0_6B57A087-F432-4DA7-AB65-A3BC2F2CE3F1.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/OpenProtocolInformation_Conf_0_0_6B57A087-F432-4DA7-AB65-A3BC2F2CE3F1.ekl (OPENPR~1.EKL)
    Orphaned long file name part "OpenProtocolInformation_Func_0_0_89FBAE4A-6132-44E0-BBF0-0B5C3CA8A2A5.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/OpenProtocolInformation_Func_0_0_89FBAE4A-6132-44E0-BBF0-0B5C3CA8A2A5.log (OPENPR~1.LOG)
    Orphaned long file name part "OpenProtocolInformation_Func_0_0_89FBAE4A-6132-44E0-BBF0-0B5C3CA8A2A5.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/OpenProtocolInformation_Func_0_0_89FBAE4A-6132-44E0-BBF0-0B5C3CA8A2A5.ekl (OPENPR~1.EKL)
    Orphaned long file name part "OpenProtocol_Conf_0_0_F9DF2097-7C10-4551-914C-551192C01981.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/OpenProtocol_Conf_0_0_F9DF2097-7C10-4551-914C-551192C01981.log (OPENPR~1.LOG)
    Orphaned long file name part "OpenProtocol_Conf_0_0_F9DF2097-7C10-4551-914C-551192C01981.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/OpenProtocol_Conf_0_0_F9DF2097-7C10-4551-914C-551192C01981.ekl (OPENPR~1.EKL)
    Orphaned long file name part "OpenProtocol_Func_1_0_0_7A4B18A0-7B00-4786-8128-564F3BA41CE1.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/OpenProtocol_Func_1_0_0_7A4B18A0-7B00-4786-8128-564F3BA41CE1.log (OPENPR~1.LOG)
    Orphaned long file name part "OpenProtocol_Func_1_0_0_7A4B18A0-7B00-4786-8128-564F3BA41CE1.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/OpenProtocol_Func_1_0_0_7A4B18A0-7B00-4786-8128-564F3BA41CE1.ekl (OPENPR~1.EKL)
    Orphaned long file name part "OpenProtocol_Func_2_0_0_4F00A0C1-77BF-4CE9-B4A6-578976DF5288.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/OpenProtocol_Func_2_0_0_4F00A0C1-77BF-4CE9-B4A6-578976DF5288.log (OPENPR~1.LOG)
    Orphaned long file name part "OpenProtocol_Func_2_0_0_4F00A0C1-77BF-4CE9-B4A6-578976DF5288.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/OpenProtocol_Func_2_0_0_4F00A0C1-77BF-4CE9-B4A6-578976DF5288.ekl (OPENPR~1.EKL)
    Orphaned long file name part "OpenProtocol_Func_3_0_0_D0BB122F-231E-4EEF-94D4-4E03A79C469D.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/OpenProtocol_Func_3_0_0_D0BB122F-231E-4EEF-94D4-4E03A79C469D.log (OPENPR~1.LOG)
    Orphaned long file name part "OpenProtocol_Func_3_0_0_D0BB122F-231E-4EEF-94D4-4E03A79C469D.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/OpenProtocol_Func_3_0_0_D0BB122F-231E-4EEF-94D4-4E03A79C469D.ekl (OPENPR~1.EKL)
    Orphaned long file name part "ProtocolsPerHandle_Conf_0_0_F02E4084-6FD5-4B01-8C3E-ACC959FB6BA0.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/ProtocolsPerHandle_Conf_0_0_F02E4084-6FD5-4B01-8C3E-ACC959FB6BA0.log (PROTOC~1.LOG)
    Orphaned long file name part "ProtocolsPerHandle_Conf_0_0_F02E4084-6FD5-4B01-8C3E-ACC959FB6BA0.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/ProtocolsPerHandle_Conf_0_0_F02E4084-6FD5-4B01-8C3E-ACC959FB6BA0.ekl (PROTOC~1.EKL)
    Orphaned long file name part "ProtocolsPerHandle_Func_0_0_C1126254-8FD3-4170-A0A1-99D4CEE214CB.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/ProtocolsPerHandle_Func_0_0_C1126254-8FD3-4170-A0A1-99D4CEE214CB.log (PROTOC~1.LOG)
    Orphaned long file name part "ProtocolsPerHandle_Func_0_0_C1126254-8FD3-4170-A0A1-99D4CEE214CB.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/ProtocolsPerHandle_Func_0_0_C1126254-8FD3-4170-A0A1-99D4CEE214CB.ekl (PROTOC~1.EKL)
    Orphaned long file name part "RegisterProtocolNotify_Conf_0_0_91666998-769F-4075-8D43-C5F391736453.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/RegisterProtocolNotify_Conf_0_0_91666998-769F-4075-8D43-C5F391736453.log (REGIST~1.LOG)
    Orphaned long file name part "RegisterProtocolNotify_Conf_0_0_91666998-769F-4075-8D43-C5F391736453.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/RegisterProtocolNotify_Conf_0_0_91666998-769F-4075-8D43-C5F391736453.ekl (REGIST~1.EKL)
    Orphaned long file name part "RegisterProtocolNotify_Func_0_0_B6A82616-E08E-4226-A8E2-E6912BAA8E8C.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/RegisterProtocolNotify_Func_0_0_B6A82616-E08E-4226-A8E2-E6912BAA8E8C.log (REGIST~1.LOG)
    Orphaned long file name part "RegisterProtocolNotify_Func_0_0_B6A82616-E08E-4226-A8E2-E6912BAA8E8C.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/RegisterProtocolNotify_Func_0_0_B6A82616-E08E-4226-A8E2-E6912BAA8E8C.ekl (REGIST~1.EKL)
    Orphaned long file name part "ReinstallProtocolInterface_Conf_0_0_9FEF66C1-3509-4E88-846D-B9CC264F69BC.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/ReinstallProtocolInterface_Conf_0_0_9FEF66C1-3509-4E88-846D-B9CC264F69BC.log (REINST~1.LOG)
    Orphaned long file name part "ReinstallProtocolInterface_Conf_0_0_9FEF66C1-3509-4E88-846D-B9CC264F69BC.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/ReinstallProtocolInterface_Conf_0_0_9FEF66C1-3509-4E88-846D-B9CC264F69BC.ekl (REINST~1.EKL)
    Orphaned long file name part "ReinstallProtocolInterface_Func_0_0_CDF41A28-EC2A-4B25-922C-77B0EC18C797.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/ReinstallProtocolInterface_Func_0_0_CDF41A28-EC2A-4B25-922C-77B0EC18C797.log (REINST~1.LOG)
    Orphaned long file name part "ReinstallProtocolInterface_Func_0_0_CDF41A28-EC2A-4B25-922C-77B0EC18C797.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/ReinstallProtocolInterface_Func_0_0_CDF41A28-EC2A-4B25-922C-77B0EC18C797.ekl (REINST~1.EKL)
    Orphaned long file name part "UninstallMultipleProtocolInterfaces_Conf_0_0_DB11A27E-2FC0-42F0-A0C6-F12BC2E255E3.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/UninstallMultipleProtocolInterfaces_Conf_0_0_DB11A27E-2FC0-42F0-A0C6-F12BC2E255E3.log (UNINST~1.LOG)
    Orphaned long file name part "UninstallMultipleProtocolInterfaces_Conf_0_0_DB11A27E-2FC0-42F0-A0C6-F12BC2E255E3.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/UninstallMultipleProtocolInterfaces_Conf_0_0_DB11A27E-2FC0-42F0-A0C6-F12BC2E255E3.ekl (UNINST~1.EKL)
    Orphaned long file name part "UninstallMultipleProtocolInterfaces_Func_0_0_283CCDDA-D4CD-4BD1-8A9D-A4AEF1A7A214.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/UninstallMultipleProtocolInterfaces_Func_0_0_283CCDDA-D4CD-4BD1-8A9D-A4AEF1A7A214.log (UNINST~1.LOG)
    Orphaned long file name part "UninstallMultipleProtocolInterfaces_Func_0_0_283CCDDA-D4CD-4BD1-8A9D-A4AEF1A7A214.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/UninstallMultipleProtocolInterfaces_Func_0_0_283CCDDA-D4CD-4BD1-8A9D-A4AEF1A7A214.ekl (UNINST~1.EKL)
    Orphaned long file name part "UninstallProtocolInterface_Conf_0_0_C46151F4-362F-41F6-8BBE-81D0C6A9381F.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/UninstallProtocolInterface_Conf_0_0_C46151F4-362F-41F6-8BBE-81D0C6A9381F.log (UNINST~1.LOG)
    Orphaned long file name part "UninstallProtocolInterface_Conf_0_0_C46151F4-362F-41F6-8BBE-81D0C6A9381F.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/UninstallProtocolInterface_Conf_0_0_C46151F4-362F-41F6-8BBE-81D0C6A9381F.ekl (UNINST~1.EKL)
    Orphaned long file name part "UninstallProtocolInterface_Func_0_0_4AA7DD8F-E3C3-434D-AE27-8C9DA66F58A3.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/UninstallProtocolInterface_Func_0_0_4AA7DD8F-E3C3-434D-AE27-8C9DA66F58A3.log (UNINST~1.LOG)
    Orphaned long file name part "UninstallProtocolInterface_Func_0_0_4AA7DD8F-E3C3-434D-AE27-8C9DA66F58A3.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ProtocolHandlerServicesTest0/UninstallProtocolInterface_Func_0_0_4AA7DD8F-E3C3-434D-AE27-8C9DA66F58A3.ekl (UNINST~1.EKL)
    /Log/BootServicesTest/ProtocolHandlerServicesTest0/CloseProtocol_Conf_0_0_85302E6F-328B-407B-BD6D-835DD54BA54B.log
      Duplicate directory entry.
      First    Size 5854 bytes, date 01:00:00 Jan 01 1980
      Second   Size 37174 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.000
    /Log/BootServicesTest/ProtocolHandlerServicesTest0/CloseProtocol_Conf_0_0_85302E6F-328B-407B-BD6D-835DD54BA54B.ekl
      Duplicate directory entry.
      First    Size 3820 bytes, date 01:00:00 Jan 01 1980
      Second   Size 34554 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.001
    /Log/BootServicesTest/ProtocolHandlerServicesTest0/ConnectController_Conf_0_0_B6C90CCE-9063-4A76-B82D-CAD4191E7514.log
      Duplicate directory entry.
      First    Size 4292 bytes, date 01:00:00 Jan 01 1980
      Second   Size 450866 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.002
    /Log/BootServicesTest/ProtocolHandlerServicesTest0/ConnectController_Conf_0_0_B6C90CCE-9063-4A76-B82D-CAD4191E7514.ekl
      Duplicate directory entry.
      First    Size 2256 bytes, date 01:00:00 Jan 01 1980
      Second   Size 440682 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.003
    /Log/BootServicesTest/ProtocolHandlerServicesTest0/DisconnectController_Conf_0_0_94EEDBEC-55CA-442E-B99F-0788B8E51C10.log
      Duplicate directory entry.
      First    Size 4372 bytes, date 01:00:00 Jan 01 1980
      Second   Size 25660 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.004
    /Log/BootServicesTest/ProtocolHandlerServicesTest0/DisconnectController_Conf_0_0_94EEDBEC-55CA-442E-B99F-0788B8E51C10.ekl
      Duplicate directory entry.
      First    Size 2312 bytes, date 01:00:00 Jan 01 1980
      Second   Size 23224 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.005
    /Log/BootServicesTest/ProtocolHandlerServicesTest0/HandleProtocol_Conf_0_0_231E4965-FDA4-4FA2-8AE2-8C7902C507E9.log
      Duplicate directory entry.
      First    Size 5352 bytes, date 01:00:00 Jan 01 1980
      Second   Size 8884 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.006
    /Log/BootServicesTest/ProtocolHandlerServicesTest0/HandleProtocol_Conf_0_0_231E4965-FDA4-4FA2-8AE2-8C7902C507E9.ekl
      Duplicate directory entry.
      First    Size 3320 bytes, date 01:00:00 Jan 01 1980
      Second   Size 6766 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.007
    /Log/BootServicesTest/ProtocolHandlerServicesTest0/InstallMultipleProtocolInterfaces_Conf_0_0_B6DE8DE0-7375-4804-A029-9ED0CB43F74D.log
      Duplicate directory entry.
      First    Size 6988 bytes, date 01:00:00 Jan 01 1980
      Second   Size 63014 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.008
    /Log/BootServicesTest/ProtocolHandlerServicesTest0/InstallMultipleProtocolInterfaces_Conf_0_0_B6DE8DE0-7375-4804-A029-9ED0CB43F74D.log
      Duplicate directory entry.
      First    Size 6988 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5554 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.009
    /Log/BootServicesTest/ProtocolHandlerServicesTest0/InstallMultipleProtocolInterfaces_Conf_0_0_B6DE8DE0-7375-4804-A029-9ED0CB43F74D.log
      Duplicate directory entry.
      First    Size 6988 bytes, date 01:00:00 Jan 01 1980
      Second   Size 89806 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.010
    /Log/BootServicesTest/ProtocolHandlerServicesTest0/InstallMultipleProtocolInterfaces_Conf_0_0_B6DE8DE0-7375-4804-A029-9ED0CB43F74D.ekl
      Duplicate directory entry.
      First    Size 4784 bytes, date 01:00:00 Jan 01 1980
      Second   Size 59836 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.011
    /Log/BootServicesTest/ProtocolHandlerServicesTest0/InstallMultipleProtocolInterfaces_Conf_0_0_B6DE8DE0-7375-4804-A029-9ED0CB43F74D.ekl
      Duplicate directory entry.
      First    Size 4784 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3442 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.012
    /Log/BootServicesTest/ProtocolHandlerServicesTest0/InstallMultipleProtocolInterfaces_Conf_0_0_B6DE8DE0-7375-4804-A029-9ED0CB43F74D.ekl
      Duplicate directory entry.
      First    Size 4784 bytes, date 01:00:00 Jan 01 1980
      Second   Size 86094 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.013
    /Log/BootServicesTest/ProtocolHandlerServicesTest0/LocateDevicePath_Conf_0_0_624E28E8-78BC-4D77-AB85-D2CBD3744E21.log
      Duplicate directory entry.
      First    Size 6448 bytes, date 01:00:00 Jan 01 1980
      Second   Size 72234 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.014
    /Log/BootServicesTest/ProtocolHandlerServicesTest0/LocateDevicePath_Conf_0_0_624E28E8-78BC-4D77-AB85-D2CBD3744E21.log
      Duplicate directory entry.
      First    Size 6448 bytes, date 01:00:00 Jan 01 1980
      Second   Size 4308 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.015
    /Log/BootServicesTest/ProtocolHandlerServicesTest0/LocateDevicePath_Conf_0_0_624E28E8-78BC-4D77-AB85-D2CBD3744E21.log
      Duplicate directory entry.
      First    Size 6448 bytes, date 01:00:00 Jan 01 1980
      Second   Size 61050 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.016
    /Log/BootServicesTest/ProtocolHandlerServicesTest0/LocateDevicePath_Conf_0_0_624E28E8-78BC-4D77-AB85-D2CBD3744E21.log
      Duplicate directory entry.
      First    Size 6448 bytes, date 01:00:00 Jan 01 1980
      Second   Size 6432 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.017
    /Log/BootServicesTest/ProtocolHandlerServicesTest0/LocateDevicePath_Conf_0_0_624E28E8-78BC-4D77-AB85-D2CBD3744E21.log
      Duplicate directory entry.
      First    Size 6448 bytes, date 01:00:00 Jan 01 1980
      Second   Size 119166 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.018
    /Log/BootServicesTest/ProtocolHandlerServicesTest0/LocateDevicePath_Conf_0_0_624E28E8-78BC-4D77-AB85-D2CBD3744E21.log
      Duplicate directory entry.
      First    Size 6448 bytes, date 01:00:00 Jan 01 1980
      Second   Size 4788 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.019
    /Log/BootServicesTest/ProtocolHandlerServicesTest0/LocateDevicePath_Conf_0_0_624E28E8-78BC-4D77-AB85-D2CBD3744E21.log
      Duplicate directory entry.
      First    Size 6448 bytes, date 01:00:00 Jan 01 1980
      Second   Size 12116 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.020
    /Log/BootServicesTest/ProtocolHandlerServicesTest0/LocateDevicePath_Conf_0_0_624E28E8-78BC-4D77-AB85-D2CBD3744E21.ekl
      Duplicate directory entry.
      First    Size 4380 bytes, date 01:00:00 Jan 01 1980
      Second   Size 68796 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.021
    /Log/BootServicesTest/ProtocolHandlerServicesTest0/LocateDevicePath_Conf_0_0_624E28E8-78BC-4D77-AB85-D2CBD3744E21.ekl
      Duplicate directory entry.
      First    Size 4380 bytes, date 01:00:00 Jan 01 1980
      Second   Size 2264 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.022
    /Log/BootServicesTest/ProtocolHandlerServicesTest0/LocateDevicePath_Conf_0_0_624E28E8-78BC-4D77-AB85-D2CBD3744E21.ekl
      Duplicate directory entry.
      First    Size 4380 bytes, date 01:00:00 Jan 01 1980
      Second   Size 57968 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.023
    /Log/BootServicesTest/ProtocolHandlerServicesTest0/LocateDevicePath_Conf_0_0_624E28E8-78BC-4D77-AB85-D2CBD3744E21.ekl
      Duplicate directory entry.
      First    Size 4380 bytes, date 01:00:00 Jan 01 1980
      Second   Size 4396 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.024
    /Log/BootServicesTest/ProtocolHandlerServicesTest0/LocateDevicePath_Conf_0_0_624E28E8-78BC-4D77-AB85-D2CBD3744E21.ekl
      Duplicate directory entry.
      First    Size 4380 bytes, date 01:00:00 Jan 01 1980
      Second   Size 115052 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.025
    /Log/BootServicesTest/ProtocolHandlerServicesTest0/LocateDevicePath_Conf_0_0_624E28E8-78BC-4D77-AB85-D2CBD3744E21.ekl
      Duplicate directory entry.
      First    Size 4380 bytes, date 01:00:00 Jan 01 1980
      Second   Size 2766 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.026
    /Log/BootServicesTest/ProtocolHandlerServicesTest0/LocateDevicePath_Conf_0_0_624E28E8-78BC-4D77-AB85-D2CBD3744E21.ekl
      Duplicate directory entry.
      First    Size 4380 bytes, date 01:00:00 Jan 01 1980
      Second   Size 9938 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.027
    /Log/BootServicesTest/ProtocolHandlerServicesTest0/OpenProtocolInformation_Conf_0_0_6B57A087-F432-4DA7-AB65-A3BC2F2CE3F1.log
      Duplicate directory entry.
      First    Size 3280 bytes, date 01:00:00 Jan 01 1980
      Second   Size 41658 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.028
    /Log/BootServicesTest/ProtocolHandlerServicesTest0/OpenProtocolInformation_Conf_0_0_6B57A087-F432-4DA7-AB65-A3BC2F2CE3F1.log
      Duplicate directory entry.
      First    Size 3280 bytes, date 01:00:00 Jan 01 1980
      Second   Size 9634 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.029
    /Log/BootServicesTest/ProtocolHandlerServicesTest0/OpenProtocolInformation_Conf_0_0_6B57A087-F432-4DA7-AB65-A3BC2F2CE3F1.log
      Duplicate directory entry.
      First    Size 3280 bytes, date 01:00:00 Jan 01 1980
      Second   Size 66092 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.030
    /Log/BootServicesTest/ProtocolHandlerServicesTest0/OpenProtocolInformation_Conf_0_0_6B57A087-F432-4DA7-AB65-A3BC2F2CE3F1.log
      Duplicate directory entry.
      First    Size 3280 bytes, date 01:00:00 Jan 01 1980
      Second   Size 71608 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.031
    /Log/BootServicesTest/ProtocolHandlerServicesTest0/OpenProtocolInformation_Conf_0_0_6B57A087-F432-4DA7-AB65-A3BC2F2CE3F1.log
      Duplicate directory entry.
      First    Size 3280 bytes, date 01:00:00 Jan 01 1980
      Second   Size 55566 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.032
    /Log/BootServicesTest/ProtocolHandlerServicesTest0/OpenProtocolInformation_Conf_0_0_6B57A087-F432-4DA7-AB65-A3BC2F2CE3F1.ekl
      Duplicate directory entry.
      First    Size 1216 bytes, date 01:00:00 Jan 01 1980
      Second   Size 38898 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.033
    /Log/BootServicesTest/ProtocolHandlerServicesTest0/OpenProtocolInformation_Conf_0_0_6B57A087-F432-4DA7-AB65-A3BC2F2CE3F1.ekl
      Duplicate directory entry.
      First    Size 1216 bytes, date 01:00:00 Jan 01 1980
      Second   Size 7536 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.034
    /Log/BootServicesTest/ProtocolHandlerServicesTest0/OpenProtocolInformation_Conf_0_0_6B57A087-F432-4DA7-AB65-A3BC2F2CE3F1.ekl
      Duplicate directory entry.
      First    Size 1216 bytes, date 01:00:00 Jan 01 1980
      Second   Size 62882 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.035
    /Log/BootServicesTest/ProtocolHandlerServicesTest0/OpenProtocolInformation_Conf_0_0_6B57A087-F432-4DA7-AB65-A3BC2F2CE3F1.ekl
      Duplicate directory entry.
      First    Size 1216 bytes, date 01:00:00 Jan 01 1980
      Second   Size 68316 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.036
    /Log/BootServicesTest/ProtocolHandlerServicesTest0/OpenProtocolInformation_Conf_0_0_6B57A087-F432-4DA7-AB65-A3BC2F2CE3F1.ekl
      Duplicate directory entry.
      First    Size 1216 bytes, date 01:00:00 Jan 01 1980
      Second   Size 52552 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.037
    /Log/BootServicesTest/ProtocolHandlerServicesTest0/ProtocolsPerHandle_Conf_0_0_F02E4084-6FD5-4B01-8C3E-ACC959FB6BA0.log
      Duplicate directory entry.
      First    Size 4400 bytes, date 01:00:00 Jan 01 1980
      Second   Size 12828 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.038
    /Log/BootServicesTest/ProtocolHandlerServicesTest0/ProtocolsPerHandle_Conf_0_0_F02E4084-6FD5-4B01-8C3E-ACC959FB6BA0.ekl
      Duplicate directory entry.
      First    Size 2356 bytes, date 01:00:00 Jan 01 1980
      Second   Size 10618 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.039
    /Log/BootServicesTest/ProtocolHandlerServicesTest0/RegisterProtocolNotify_Conf_0_0_91666998-769F-4075-8D43-C5F391736453.log
      Duplicate directory entry.
      First    Size 4398 bytes, date 01:00:00 Jan 01 1980
      Second   Size 45192 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.040
    /Log/BootServicesTest/ProtocolHandlerServicesTest0/RegisterProtocolNotify_Conf_0_0_91666998-769F-4075-8D43-C5F391736453.ekl
      Duplicate directory entry.
      First    Size 2322 bytes, date 01:00:00 Jan 01 1980
      Second   Size 42366 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.041
    /Log/BootServicesTest/ProtocolHandlerServicesTest0/ReinstallProtocolInterface_Conf_0_0_9FEF66C1-3509-4E88-846D-B9CC264F69BC.log
      Duplicate directory entry.
      First    Size 5562 bytes, date 01:00:00 Jan 01 1980
      Second   Size 59498 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.042
    /Log/BootServicesTest/ProtocolHandlerServicesTest0/ReinstallProtocolInterface_Conf_0_0_9FEF66C1-3509-4E88-846D-B9CC264F69BC.ekl
      Duplicate directory entry.
      First    Size 3434 bytes, date 01:00:00 Jan 01 1980
      Second   Size 56410 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.043
    /Log/BootServicesTest/ProtocolHandlerServicesTest0/UninstallMultipleProtocolInterfaces_Conf_0_0_DB11A27E-2FC0-42F0-A0C6-F12BC2E255E3.log
      Duplicate directory entry.
      First    Size 4046 bytes, date 01:00:00 Jan 01 1980
      Second   Size 83296 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.044
    /Log/BootServicesTest/ProtocolHandlerServicesTest0/UninstallMultipleProtocolInterfaces_Conf_0_0_DB11A27E-2FC0-42F0-A0C6-F12BC2E255E3.log
      Duplicate directory entry.
      First    Size 4046 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5562 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.045
    /Log/BootServicesTest/ProtocolHandlerServicesTest0/UninstallMultipleProtocolInterfaces_Conf_0_0_DB11A27E-2FC0-42F0-A0C6-F12BC2E255E3.log
      Duplicate directory entry.
      First    Size 4046 bytes, date 01:00:00 Jan 01 1980
      Second   Size 65880 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.046
    /Log/BootServicesTest/ProtocolHandlerServicesTest0/UninstallMultipleProtocolInterfaces_Conf_0_0_DB11A27E-2FC0-42F0-A0C6-F12BC2E255E3.ekl
      Duplicate directory entry.
      First    Size 1876 bytes, date 01:00:00 Jan 01 1980
      Second   Size 79778 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.047
    /Log/BootServicesTest/ProtocolHandlerServicesTest0/UninstallMultipleProtocolInterfaces_Conf_0_0_DB11A27E-2FC0-42F0-A0C6-F12BC2E255E3.ekl
      Duplicate directory entry.
      First    Size 1876 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3434 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.048
    /Log/BootServicesTest/ProtocolHandlerServicesTest0/UninstallMultipleProtocolInterfaces_Conf_0_0_DB11A27E-2FC0-42F0-A0C6-F12BC2E255E3.ekl
      Duplicate directory entry.
      First    Size 1876 bytes, date 01:00:00 Jan 01 1980
      Second   Size 62670 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.049
    Checking file /Log/BootServicesTest/ImageServicesTest0/.
    Checking file /Log/BootServicesTest/ImageServicesTest0/..
    Orphaned long file name part "ExitBootServices_Conf_0_0_303ABFAB-C865-4255-86E3-6EEF175E30DD.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ImageServicesTest0/ExitBootServices_Conf_0_0_303ABFAB-C865-4255-86E3-6EEF175E30DD.log (EXITBO~1.LOG)
    Orphaned long file name part "ExitBootServices_Conf_0_0_303ABFAB-C865-4255-86E3-6EEF175E30DD.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ImageServicesTest0/ExitBootServices_Conf_0_0_303ABFAB-C865-4255-86E3-6EEF175E30DD.ekl (EXITBO~1.EKL)
    Orphaned long file name part "Exit_Conf_0_0_DD6E776A-53A5-4A72-9EA6-FB71A7096EB5.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ImageServicesTest0/Exit_Conf_0_0_DD6E776A-53A5-4A72-9EA6-FB71A7096EB5.log (EXIT_C~1.LOG)
    Orphaned long file name part "Exit_Conf_0_0_DD6E776A-53A5-4A72-9EA6-FB71A7096EB5.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ImageServicesTest0/Exit_Conf_0_0_DD6E776A-53A5-4A72-9EA6-FB71A7096EB5.ekl (EXIT_C~1.EKL)
    Orphaned long file name part "Exit_Func_0_0_1491FD0D-E7C0-460F-946D-2AF78567D1AA.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ImageServicesTest0/Exit_Func_0_0_1491FD0D-E7C0-460F-946D-2AF78567D1AA.log (EXIT_F~1.LOG)
    Orphaned long file name part "Exit_Func_0_0_1491FD0D-E7C0-460F-946D-2AF78567D1AA.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ImageServicesTest0/Exit_Func_0_0_1491FD0D-E7C0-460F-946D-2AF78567D1AA.ekl (EXIT_F~1.EKL)
    Orphaned long file name part "LoadImage_Conf_0_0_225239AD-DCB8-4367-8FD8-8E190E1A0308.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ImageServicesTest0/LoadImage_Conf_0_0_225239AD-DCB8-4367-8FD8-8E190E1A0308.log (LOADIM~1.LOG)
    Orphaned long file name part "LoadImage_Conf_0_0_225239AD-DCB8-4367-8FD8-8E190E1A0308.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ImageServicesTest0/LoadImage_Conf_0_0_225239AD-DCB8-4367-8FD8-8E190E1A0308.ekl (LOADIM~1.EKL)
    Orphaned long file name part "LoadImage_Func_0_0_2FF0431A-8E07-4CDB-A298-D004566A74D4.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ImageServicesTest0/LoadImage_Func_0_0_2FF0431A-8E07-4CDB-A298-D004566A74D4.log (LOADIM~1.LOG)
    Orphaned long file name part "LoadImage_Func_0_0_2FF0431A-8E07-4CDB-A298-D004566A74D4.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ImageServicesTest0/LoadImage_Func_0_0_2FF0431A-8E07-4CDB-A298-D004566A74D4.ekl (LOADIM~1.EKL)
    Orphaned long file name part "StartImage_Conf_0_0_61995EF9-D030-44B1-864C-55EF7D7CBB74.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ImageServicesTest0/StartImage_Conf_0_0_61995EF9-D030-44B1-864C-55EF7D7CBB74.log (STARTI~1.LOG)
    Orphaned long file name part "StartImage_Conf_0_0_61995EF9-D030-44B1-864C-55EF7D7CBB74.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ImageServicesTest0/StartImage_Conf_0_0_61995EF9-D030-44B1-864C-55EF7D7CBB74.ekl (STARTI~1.EKL)
    Orphaned long file name part "StartImage_Func_0_0_D407BC73-BB7E-443C-9A61-97C70B7A1D62.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ImageServicesTest0/StartImage_Func_0_0_D407BC73-BB7E-443C-9A61-97C70B7A1D62.log (STARTI~1.LOG)
    Orphaned long file name part "StartImage_Func_0_0_D407BC73-BB7E-443C-9A61-97C70B7A1D62.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ImageServicesTest0/StartImage_Func_0_0_D407BC73-BB7E-443C-9A61-97C70B7A1D62.ekl (STARTI~1.EKL)
    Orphaned long file name part "UnloadImage_Conf_0_0_B9AFCAC3-198F-4783-A8CA-795978DFCFBA.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ImageServicesTest0/UnloadImage_Conf_0_0_B9AFCAC3-198F-4783-A8CA-795978DFCFBA.log (UNLOAD~1.LOG)
    Orphaned long file name part "UnloadImage_Conf_0_0_B9AFCAC3-198F-4783-A8CA-795978DFCFBA.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ImageServicesTest0/UnloadImage_Conf_0_0_B9AFCAC3-198F-4783-A8CA-795978DFCFBA.ekl (UNLOAD~1.EKL)
    Orphaned long file name part "UnloadImage_Func_0_0_4EA3EEA6-F7C9-4568-B81E-10D3E0FED6E7.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ImageServicesTest0/UnloadImage_Func_0_0_4EA3EEA6-F7C9-4568-B81E-10D3E0FED6E7.log (UNLOAD~1.LOG)
    Orphaned long file name part "UnloadImage_Func_0_0_4EA3EEA6-F7C9-4568-B81E-10D3E0FED6E7.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/ImageServicesTest0/UnloadImage_Func_0_0_4EA3EEA6-F7C9-4568-B81E-10D3E0FED6E7.ekl (UNLOAD~1.EKL)
    /Log/BootServicesTest/ImageServicesTest0/LoadImage_Conf_0_0_225239AD-DCB8-4367-8FD8-8E190E1A0308.log
      Duplicate directory entry.
      First    Size 7000 bytes, date 01:00:00 Jan 01 1980
      Second   Size 37468 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.000
    /Log/BootServicesTest/ImageServicesTest0/LoadImage_Conf_0_0_225239AD-DCB8-4367-8FD8-8E190E1A0308.ekl
      Duplicate directory entry.
      First    Size 4876 bytes, date 01:00:00 Jan 01 1980
      Second   Size 34706 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.001
    /Log/BootServicesTest/ImageServicesTest0/StartImage_Conf_0_0_61995EF9-D030-44B1-864C-55EF7D7CBB74.log
      Duplicate directory entry.
      First    Size 4126 bytes, date 01:00:00 Jan 01 1980
      Second   Size 14236 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.002
    /Log/BootServicesTest/ImageServicesTest0/StartImage_Conf_0_0_61995EF9-D030-44B1-864C-55EF7D7CBB74.ekl
      Duplicate directory entry.
      First    Size 2054 bytes, date 01:00:00 Jan 01 1980
      Second   Size 11948 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.003
    /Log/BootServicesTest/ImageServicesTest0/UnloadImage_Conf_0_0_B9AFCAC3-198F-4783-A8CA-795978DFCFBA.log
      Duplicate directory entry.
      First    Size 4142 bytes, date 01:00:00 Jan 01 1980
      Second   Size 24950 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.004
    /Log/BootServicesTest/ImageServicesTest0/UnloadImage_Conf_0_0_B9AFCAC3-198F-4783-A8CA-795978DFCFBA.ekl
      Duplicate directory entry.
      First    Size 2062 bytes, date 01:00:00 Jan 01 1980
      Second   Size 22444 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.005
    Checking file /Log/BootServicesTest/MiscBootServicesTest0/.
    Checking file /Log/BootServicesTest/MiscBootServicesTest0/..
    Orphaned long file name part "CalculateCrc32_Conf_0_0_718165E6-C904-43F1-9A93-DDE3467EEDC2.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/MiscBootServicesTest0/CalculateCrc32_Conf_0_0_718165E6-C904-43F1-9A93-DDE3467EEDC2.log (CALCUL~1.LOG)
    Orphaned long file name part "CalculateCrc32_Conf_0_0_718165E6-C904-43F1-9A93-DDE3467EEDC2.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/MiscBootServicesTest0/CalculateCrc32_Conf_0_0_718165E6-C904-43F1-9A93-DDE3467EEDC2.ekl (CALCUL~1.EKL)
    Orphaned long file name part "CalculateCrc32_Func_0_0_B510F99F-FEE9-4AF6-BB0F-3C958EF7F166.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/MiscBootServicesTest0/CalculateCrc32_Func_0_0_B510F99F-FEE9-4AF6-BB0F-3C958EF7F166.log (CALCUL~1.LOG)
    Orphaned long file name part "CalculateCrc32_Func_0_0_B510F99F-FEE9-4AF6-BB0F-3C958EF7F166.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/MiscBootServicesTest0/CalculateCrc32_Func_0_0_B510F99F-FEE9-4AF6-BB0F-3C958EF7F166.ekl (CALCUL~1.EKL)
    Orphaned long file name part "CopyMem_Func_0_0_4397A610-8D5D-441B-8E7D-C23377F3EB67.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/MiscBootServicesTest0/CopyMem_Func_0_0_4397A610-8D5D-441B-8E7D-C23377F3EB67.log (COPYME~1.LOG)
    Orphaned long file name part "CopyMem_Func_0_0_4397A610-8D5D-441B-8E7D-C23377F3EB67.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/MiscBootServicesTest0/CopyMem_Func_0_0_4397A610-8D5D-441B-8E7D-C23377F3EB67.ekl (COPYME~1.EKL)
    Orphaned long file name part "GetNextMonotonicCount_Conf_0_0_E9544E95-2792-494C-AC39-CC33688F9513.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/MiscBootServicesTest0/GetNextMonotonicCount_Conf_0_0_E9544E95-2792-494C-AC39-CC33688F9513.log (GETNEX~1.LOG)
    Orphaned long file name part "GetNextMonotonicCount_Conf_0_0_E9544E95-2792-494C-AC39-CC33688F9513.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/MiscBootServicesTest0/GetNextMonotonicCount_Conf_0_0_E9544E95-2792-494C-AC39-CC33688F9513.ekl (GETNEX~1.EKL)
    Orphaned long file name part "GetNextMonotonicCount_Func_0_0_D35AAEF2-55FB-4377-A07B-29DCA3201F19.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/MiscBootServicesTest0/GetNextMonotonicCount_Func_0_0_D35AAEF2-55FB-4377-A07B-29DCA3201F19.log (GETNEX~1.LOG)
    Orphaned long file name part "GetNextMonotonicCount_Func_0_0_D35AAEF2-55FB-4377-A07B-29DCA3201F19.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/MiscBootServicesTest0/GetNextMonotonicCount_Func_0_0_D35AAEF2-55FB-4377-A07B-29DCA3201F19.ekl (GETNEX~1.EKL)
    Orphaned long file name part "InstallConfigurationTable_Conf_0_0_E00A6879-AF7E-4238-AAD1-0B891E71D721.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/MiscBootServicesTest0/InstallConfigurationTable_Conf_0_0_E00A6879-AF7E-4238-AAD1-0B891E71D721.log (INSTAL~1.LOG)
    Orphaned long file name part "InstallConfigurationTable_Conf_0_0_E00A6879-AF7E-4238-AAD1-0B891E71D721.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/MiscBootServicesTest0/InstallConfigurationTable_Conf_0_0_E00A6879-AF7E-4238-AAD1-0B891E71D721.ekl (INSTAL~1.EKL)
    Orphaned long file name part "InstallConfigurationTable_Func_0_0_911FB78B-1A6D-46C4-9F68-509CFB593D98.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/MiscBootServicesTest0/InstallConfigurationTable_Func_0_0_911FB78B-1A6D-46C4-9F68-509CFB593D98.log (INSTAL~1.LOG)
    Orphaned long file name part "InstallConfigurationTable_Func_0_0_911FB78B-1A6D-46C4-9F68-509CFB593D98.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/MiscBootServicesTest0/InstallConfigurationTable_Func_0_0_911FB78B-1A6D-46C4-9F68-509CFB593D98.ekl (INSTAL~1.EKL)
    Orphaned long file name part "SetMem_Func_0_0_315BE343-A32D-461D-A3CC-5E6895CC2CBA.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/MiscBootServicesTest0/SetMem_Func_0_0_315BE343-A32D-461D-A3CC-5E6895CC2CBA.log (SETMEM~1.LOG)
    Orphaned long file name part "SetMem_Func_0_0_315BE343-A32D-461D-A3CC-5E6895CC2CBA.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/MiscBootServicesTest0/SetMem_Func_0_0_315BE343-A32D-461D-A3CC-5E6895CC2CBA.ekl (SETMEM~1.EKL)
    Orphaned long file name part "SetWatchdogTimer_Conf_0_0_FF388AE5-4C51-45C6-9D37-6DE04BF9219A.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/MiscBootServicesTest0/SetWatchdogTimer_Conf_0_0_FF388AE5-4C51-45C6-9D37-6DE04BF9219A.log (SETWAT~1.LOG)
    Orphaned long file name part "SetWatchdogTimer_Conf_0_0_FF388AE5-4C51-45C6-9D37-6DE04BF9219A.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/MiscBootServicesTest0/SetWatchdogTimer_Conf_0_0_FF388AE5-4C51-45C6-9D37-6DE04BF9219A.ekl (SETWAT~1.EKL)
    Orphaned long file name part "SetWatchdogTimer_Func_0_0_F17B25A1-866B-4791-BC9C-BB3D19E4B3F8.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/MiscBootServicesTest0/SetWatchdogTimer_Func_0_0_F17B25A1-866B-4791-BC9C-BB3D19E4B3F8.log (SETWAT~1.LOG)
    Orphaned long file name part "SetWatchdogTimer_Func_0_0_F17B25A1-866B-4791-BC9C-BB3D19E4B3F8.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/MiscBootServicesTest0/SetWatchdogTimer_Func_0_0_F17B25A1-866B-4791-BC9C-BB3D19E4B3F8.ekl (SETWAT~1.EKL)
    Orphaned long file name part "Stall_Func_0_0_539675B8-D9B3-4DC7-A8D0-FF19BBA13B86.log"
      Auto-deleting.
    Checking file /Log/BootServicesTest/MiscBootServicesTest0/Stall_Func_0_0_539675B8-D9B3-4DC7-A8D0-FF19BBA13B86.log (STALL_~1.LOG)
    Orphaned long file name part "Stall_Func_0_0_539675B8-D9B3-4DC7-A8D0-FF19BBA13B86.ekl"
      Auto-deleting.
    Checking file /Log/BootServicesTest/MiscBootServicesTest0/Stall_Func_0_0_539675B8-D9B3-4DC7-A8D0-FF19BBA13B86.ekl (STALL_~1.EKL)
    /Log/BootServicesTest/MiscBootServicesTest0/CalculateCrc32_Conf_0_0_718165E6-C904-43F1-9A93-DDE3467EEDC2.log
      Duplicate directory entry.
      First    Size 4126 bytes, date 01:00:00 Jan 01 1980
      Second   Size 4052 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.000
    /Log/BootServicesTest/MiscBootServicesTest0/CalculateCrc32_Conf_0_0_718165E6-C904-43F1-9A93-DDE3467EEDC2.ekl
      Duplicate directory entry.
      First    Size 2106 bytes, date 01:00:00 Jan 01 1980
      Second   Size 2036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.001
    /Log/BootServicesTest/MiscBootServicesTest0/GetNextMonotonicCount_Conf_0_0_E9544E95-2792-494C-AC39-CC33688F9513.log
      Duplicate directory entry.
      First    Size 3204 bytes, date 01:00:00 Jan 01 1980
      Second   Size 13234 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.002
    /Log/BootServicesTest/MiscBootServicesTest0/GetNextMonotonicCount_Conf_0_0_E9544E95-2792-494C-AC39-CC33688F9513.ekl
      Duplicate directory entry.
      First    Size 1110 bytes, date 01:00:00 Jan 01 1980
      Second   Size 9800 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.003
    /Log/BootServicesTest/MiscBootServicesTest0/InstallConfigurationTable_Conf_0_0_E00A6879-AF7E-4238-AAD1-0B891E71D721.log
      Duplicate directory entry.
      First    Size 3772 bytes, date 01:00:00 Jan 01 1980
      Second   Size 20652 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.004
    /Log/BootServicesTest/MiscBootServicesTest0/InstallConfigurationTable_Conf_0_0_E00A6879-AF7E-4238-AAD1-0B891E71D721.ekl
      Duplicate directory entry.
      First    Size 1674 bytes, date 01:00:00 Jan 01 1980
      Second   Size 18216 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.005
    /Log/BootServicesTest/MiscBootServicesTest0/SetWatchdogTimer_Conf_0_0_FF388AE5-4C51-45C6-9D37-6DE04BF9219A.log
      Duplicate directory entry.
      First    Size 2650 bytes, date 01:00:00 Jan 01 1980
      Second   Size 24394 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.006
    /Log/BootServicesTest/MiscBootServicesTest0/SetWatchdogTimer_Conf_0_0_FF388AE5-4C51-45C6-9D37-6DE04BF9219A.ekl
      Duplicate directory entry.
      First    Size 468 bytes, date 01:00:00 Jan 01 1980
      Second   Size 19842 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.007
    Checking file /Log/RuntimeServicesTest/.
    Checking file /Log/RuntimeServicesTest/..
    Checking file /Log/RuntimeServicesTest/VariableServicesTest0 (VARIAB~1)
    Checking file /Log/RuntimeServicesTest/TimeServicesTest0 (TIMESE~1)
    Checking file /Log/RuntimeServicesTest/MiscRuntimeServicesTest0 (MISCRU~1)
    Checking file /Log/RuntimeServicesTest/VariableServicesTest0/.
    Checking file /Log/RuntimeServicesTest/VariableServicesTest0/..
    Orphaned long file name part "AuthVar_Conf_0_0_28155531-80C5-4AD0-8471-A5E2AECF236C.log"
      Auto-deleting.
    Checking file /Log/RuntimeServicesTest/VariableServicesTest0/AuthVar_Conf_0_0_28155531-80C5-4AD0-8471-A5E2AECF236C.log (AUTHVA~1.LOG)
    Orphaned long file name part "AuthVar_Conf_0_0_28155531-80C5-4AD0-8471-A5E2AECF236C.ekl"
      Auto-deleting.
    Checking file /Log/RuntimeServicesTest/VariableServicesTest0/AuthVar_Conf_0_0_28155531-80C5-4AD0-8471-A5E2AECF236C.ekl (AUTHVA~1.EKL)
    Orphaned long file name part "AuthVar_Func_0_0_9338D0EC-807B-4750-986A-8F2A91BB3616.log"
      Auto-deleting.
    Checking file /Log/RuntimeServicesTest/VariableServicesTest0/AuthVar_Func_0_0_9338D0EC-807B-4750-986A-8F2A91BB3616.log (AUTHVA~1.LOG)
    Orphaned long file name part "AuthVar_Func_0_0_9338D0EC-807B-4750-986A-8F2A91BB3616.ekl"
      Auto-deleting.
    Checking file /Log/RuntimeServicesTest/VariableServicesTest0/AuthVar_Func_0_0_9338D0EC-807B-4750-986A-8F2A91BB3616.ekl (AUTHVA~1.EKL)
    Orphaned long file name part "GetNextVariableName_Conf_0_0_E8014C92-15C4-42A8-8B0D-6080C47D3778.log"
      Auto-deleting.
    Checking file /Log/RuntimeServicesTest/VariableServicesTest0/GetNextVariableName_Conf_0_0_E8014C92-15C4-42A8-8B0D-6080C47D3778.log (GETNEX~1.LOG)
    Orphaned long file name part "GetNextVariableName_Conf_0_0_E8014C92-15C4-42A8-8B0D-6080C47D3778.ekl"
      Auto-deleting.
    Checking file /Log/RuntimeServicesTest/VariableServicesTest0/GetNextVariableName_Conf_0_0_E8014C92-15C4-42A8-8B0D-6080C47D3778.ekl (GETNEX~1.EKL)
    Orphaned long file name part "GetNextVariableName_Func_0_0_66A7216F-A855-47D3-919C-B6D34668BE8E.log"
      Auto-deleting.
    Checking file /Log/RuntimeServicesTest/VariableServicesTest0/GetNextVariableName_Func_0_0_66A7216F-A855-47D3-919C-B6D34668BE8E.log (GETNEX~1.LOG)
    Orphaned long file name part "GetNextVariableName_Func_0_0_66A7216F-A855-47D3-919C-B6D34668BE8E.ekl"
      Auto-deleting.
    Checking file /Log/RuntimeServicesTest/VariableServicesTest0/GetNextVariableName_Func_0_0_66A7216F-A855-47D3-919C-B6D34668BE8E.ekl (GETNEX~1.EKL)
    Orphaned long file name part "GetVariable_Conf_0_0_D90941AA-B626-4665-BA14-64084396F31D.log"
      Auto-deleting.
    Checking file /Log/RuntimeServicesTest/VariableServicesTest0/GetVariable_Conf_0_0_D90941AA-B626-4665-BA14-64084396F31D.log (GETVAR~1.LOG)
    Orphaned long file name part "GetVariable_Conf_0_0_D90941AA-B626-4665-BA14-64084396F31D.ekl"
      Auto-deleting.
    Checking file /Log/RuntimeServicesTest/VariableServicesTest0/GetVariable_Conf_0_0_D90941AA-B626-4665-BA14-64084396F31D.ekl (GETVAR~1.EKL)
    Orphaned long file name part "GetVariable_Func_0_0_5E7928AA-CF97-469C-A6CA-A5577135C10C.log"
      Auto-deleting.
    Checking file /Log/RuntimeServicesTest/VariableServicesTest0/GetVariable_Func_0_0_5E7928AA-CF97-469C-A6CA-A5577135C10C.log (GETVAR~1.LOG)
    Orphaned long file name part "GetVariable_Func_0_0_5E7928AA-CF97-469C-A6CA-A5577135C10C.ekl"
      Auto-deleting.
    Checking file /Log/RuntimeServicesTest/VariableServicesTest0/GetVariable_Func_0_0_5E7928AA-CF97-469C-A6CA-A5577135C10C.ekl (GETVAR~1.EKL)
    Orphaned long file name part "HardwareErrorRecord_Conf_0_0_CF94F695-7917-4F78-A0A8-F0B509099297.log"
      Auto-deleting.
    Checking file /Log/RuntimeServicesTest/VariableServicesTest0/HardwareErrorRecord_Conf_0_0_CF94F695-7917-4F78-A0A8-F0B509099297.log (HARDWA~1.LOG)
    Orphaned long file name part "HardwareErrorRecord_Conf_0_0_CF94F695-7917-4F78-A0A8-F0B509099297.ekl"
      Auto-deleting.
    Checking file /Log/RuntimeServicesTest/VariableServicesTest0/HardwareErrorRecord_Conf_0_0_CF94F695-7917-4F78-A0A8-F0B509099297.ekl (HARDWA~1.EKL)
    Orphaned long file name part "HardwareErrorRecord_Func_0_0_EFABA332-13E8-4730-97CB-48CE9F0826C5.log"
      Auto-deleting.
    Checking file /Log/RuntimeServicesTest/VariableServicesTest0/HardwareErrorRecord_Func_0_0_EFABA332-13E8-4730-97CB-48CE9F0826C5.log (HARDWA~1.LOG)
    Orphaned long file name part "HardwareErrorRecord_Func_0_0_EFABA332-13E8-4730-97CB-48CE9F0826C5.ekl"
      Auto-deleting.
    Checking file /Log/RuntimeServicesTest/VariableServicesTest0/HardwareErrorRecord_Func_0_0_EFABA332-13E8-4730-97CB-48CE9F0826C5.ekl (HARDWA~1.EKL)
    Orphaned long file name part "QueryVariableInfo_Conf_0_0_61758774-91A3-47DD-BDBD-B81094A5F62D.log"
      Auto-deleting.
    Checking file /Log/RuntimeServicesTest/VariableServicesTest0/QueryVariableInfo_Conf_0_0_61758774-91A3-47DD-BDBD-B81094A5F62D.log (QUERYV~1.LOG)
    Orphaned long file name part "QueryVariableInfo_Conf_0_0_61758774-91A3-47DD-BDBD-B81094A5F62D.ekl"
      Auto-deleting.
    Checking file /Log/RuntimeServicesTest/VariableServicesTest0/QueryVariableInfo_Conf_0_0_61758774-91A3-47DD-BDBD-B81094A5F62D.ekl (QUERYV~1.EKL)
    Orphaned long file name part "QueryVariableInfo_Func_0_0_9ADC0F36-FC24-4731-8981-4AA5CDE31634.log"
      Auto-deleting.
    Checking file /Log/RuntimeServicesTest/VariableServicesTest0/QueryVariableInfo_Func_0_0_9ADC0F36-FC24-4731-8981-4AA5CDE31634.log (QUERYV~1.LOG)
    Orphaned long file name part "QueryVariableInfo_Func_0_0_9ADC0F36-FC24-4731-8981-4AA5CDE31634.ekl"
      Auto-deleting.
    Checking file /Log/RuntimeServicesTest/VariableServicesTest0/QueryVariableInfo_Func_0_0_9ADC0F36-FC24-4731-8981-4AA5CDE31634.ekl (QUERYV~1.EKL)
    Orphaned long file name part "SetVariable_Conf_0_0_C0391B41-591F-4173-8CE3-5FF9158A948C.log"
      Auto-deleting.
    Checking file /Log/RuntimeServicesTest/VariableServicesTest0/SetVariable_Conf_0_0_C0391B41-591F-4173-8CE3-5FF9158A948C.log (SETVAR~1.LOG)
    Orphaned long file name part "SetVariable_Conf_0_0_C0391B41-591F-4173-8CE3-5FF9158A948C.ekl"
      Auto-deleting.
    Checking file /Log/RuntimeServicesTest/VariableServicesTest0/SetVariable_Conf_0_0_C0391B41-591F-4173-8CE3-5FF9158A948C.ekl (SETVAR~1.EKL)
    Orphaned long file name part "SetVariable_Func_0_0_D4700FE8-9832-4353-961F-74682D3701F6.log"
      Auto-deleting.
    Checking file /Log/RuntimeServicesTest/VariableServicesTest0/SetVariable_Func_0_0_D4700FE8-9832-4353-961F-74682D3701F6.log (SETVAR~1.LOG)
    Orphaned long file name part "SetVariable_Func_0_0_D4700FE8-9832-4353-961F-74682D3701F6.ekl"
      Auto-deleting.
    Checking file /Log/RuntimeServicesTest/VariableServicesTest0/SetVariable_Func_0_0_D4700FE8-9832-4353-961F-74682D3701F6.ekl (SETVAR~1.EKL)
    /Log/RuntimeServicesTest/VariableServicesTest0/AuthVar_Conf_0_0_28155531-80C5-4AD0-8471-A5E2AECF236C.log
      Duplicate directory entry.
      First    Size 22788 bytes, date 01:00:00 Jan 01 1980
      Second   Size 4524 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.000
    /Log/RuntimeServicesTest/VariableServicesTest0/AuthVar_Conf_0_0_28155531-80C5-4AD0-8471-A5E2AECF236C.ekl
      Duplicate directory entry.
      First    Size 20402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 2458 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.001
    /Log/RuntimeServicesTest/VariableServicesTest0/GetNextVariableName_Conf_0_0_E8014C92-15C4-42A8-8B0D-6080C47D3778.log
      Duplicate directory entry.
      First    Size 7980 bytes, date 01:00:00 Jan 01 1980
      Second   Size 7126 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.002
    /Log/RuntimeServicesTest/VariableServicesTest0/GetNextVariableName_Conf_0_0_E8014C92-15C4-42A8-8B0D-6080C47D3778.ekl
      Duplicate directory entry.
      First    Size 5734 bytes, date 01:00:00 Jan 01 1980
      Second   Size 4732 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.003
    /Log/RuntimeServicesTest/VariableServicesTest0/GetVariable_Conf_0_0_D90941AA-B626-4665-BA14-64084396F31D.log
      Duplicate directory entry.
      First    Size 8646 bytes, date 01:00:00 Jan 01 1980
      Second   Size 13928 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.004
    /Log/RuntimeServicesTest/VariableServicesTest0/GetVariable_Conf_0_0_D90941AA-B626-4665-BA14-64084396F31D.ekl
      Duplicate directory entry.
      First    Size 6148 bytes, date 01:00:00 Jan 01 1980
      Second   Size 9256 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.005
    /Log/RuntimeServicesTest/VariableServicesTest0/HardwareErrorRecord_Conf_0_0_CF94F695-7917-4F78-A0A8-F0B509099297.log
      Duplicate directory entry.
      First    Size 2918 bytes, date 01:00:00 Jan 01 1980
      Second   Size 2912 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.006
    /Log/RuntimeServicesTest/VariableServicesTest0/HardwareErrorRecord_Conf_0_0_CF94F695-7917-4F78-A0A8-F0B509099297.ekl
      Duplicate directory entry.
      First    Size 478 bytes, date 01:00:00 Jan 01 1980
      Second   Size 544 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.007
    /Log/RuntimeServicesTest/VariableServicesTest0/QueryVariableInfo_Conf_0_0_61758774-91A3-47DD-BDBD-B81094A5F62D.log
      Duplicate directory entry.
      First    Size 4658 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5008 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.008
    /Log/RuntimeServicesTest/VariableServicesTest0/QueryVariableInfo_Conf_0_0_61758774-91A3-47DD-BDBD-B81094A5F62D.ekl
      Duplicate directory entry.
      First    Size 2496 bytes, date 01:00:00 Jan 01 1980
      Second   Size 2842 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.009
    /Log/RuntimeServicesTest/VariableServicesTest0/SetVariable_Conf_0_0_C0391B41-591F-4173-8CE3-5FF9158A948C.log
      Duplicate directory entry.
      First    Size 23862 bytes, date 01:00:00 Jan 01 1980
      Second   Size 58248 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.010
    /Log/RuntimeServicesTest/VariableServicesTest0/SetVariable_Conf_0_0_C0391B41-591F-4173-8CE3-5FF9158A948C.ekl
      Duplicate directory entry.
      First    Size 20314 bytes, date 01:00:00 Jan 01 1980
      Second   Size 42552 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.011
    Checking file /Log/RuntimeServicesTest/TimeServicesTest0/.
    Checking file /Log/RuntimeServicesTest/TimeServicesTest0/..
    Orphaned long file name part "GetTime_Conf_0_0_C3756910-91B4-4BBF-BF40-3315F13C2D4D.log"
      Auto-deleting.
    Checking file /Log/RuntimeServicesTest/TimeServicesTest0/GetTime_Conf_0_0_C3756910-91B4-4BBF-BF40-3315F13C2D4D.log (GETTIM~1.LOG)
    Orphaned long file name part "GetTime_Conf_0_0_C3756910-91B4-4BBF-BF40-3315F13C2D4D.ekl"
      Auto-deleting.
    Checking file /Log/RuntimeServicesTest/TimeServicesTest0/GetTime_Conf_0_0_C3756910-91B4-4BBF-BF40-3315F13C2D4D.ekl (GETTIM~1.EKL)
    Orphaned long file name part "GetTime_Func_0_0_7F27237A-D0F7-451E-BDA9-F6365915FF15.log"
      Auto-deleting.
    Checking file /Log/RuntimeServicesTest/TimeServicesTest0/GetTime_Func_0_0_7F27237A-D0F7-451E-BDA9-F6365915FF15.log (GETTIM~1.LOG)
    Orphaned long file name part "GetTime_Func_0_0_7F27237A-D0F7-451E-BDA9-F6365915FF15.ekl"
      Auto-deleting.
    Checking file /Log/RuntimeServicesTest/TimeServicesTest0/GetTime_Func_0_0_7F27237A-D0F7-451E-BDA9-F6365915FF15.ekl (GETTIM~1.EKL)
    Orphaned long file name part "GetWakeupTime_Conf_0_0_735BA337-2A44-46A2-AFAB-AFBED7358F08.log"
      Auto-deleting.
    Checking file /Log/RuntimeServicesTest/TimeServicesTest0/GetWakeupTime_Conf_0_0_735BA337-2A44-46A2-AFAB-AFBED7358F08.log (GETWAK~1.LOG)
    Orphaned long file name part "GetWakeupTime_Conf_0_0_735BA337-2A44-46A2-AFAB-AFBED7358F08.ekl"
      Auto-deleting.
    Checking file /Log/RuntimeServicesTest/TimeServicesTest0/GetWakeupTime_Conf_0_0_735BA337-2A44-46A2-AFAB-AFBED7358F08.ekl (GETWAK~1.EKL)
    Orphaned long file name part "GetWakeupTime_Func_0_0_F508572D-74F7-4C6C-9CEF-DBA49C56F7AE.log"
      Auto-deleting.
    Checking file /Log/RuntimeServicesTest/TimeServicesTest0/GetWakeupTime_Func_0_0_F508572D-74F7-4C6C-9CEF-DBA49C56F7AE.log (GETWAK~1.LOG)
    Orphaned long file name part "GetWakeupTime_Func_0_0_F508572D-74F7-4C6C-9CEF-DBA49C56F7AE.ekl"
      Auto-deleting.
    Checking file /Log/RuntimeServicesTest/TimeServicesTest0/GetWakeupTime_Func_0_0_F508572D-74F7-4C6C-9CEF-DBA49C56F7AE.ekl (GETWAK~1.EKL)
    Orphaned long file name part "SetTime_Conf_0_0_A8821B44-6CE4-462A-BCD9-527B1A22AF13.log"
      Auto-deleting.
    Checking file /Log/RuntimeServicesTest/TimeServicesTest0/SetTime_Conf_0_0_A8821B44-6CE4-462A-BCD9-527B1A22AF13.log (SETTIM~1.LOG)
    Orphaned long file name part "SetTime_Conf_0_0_A8821B44-6CE4-462A-BCD9-527B1A22AF13.ekl"
      Auto-deleting.
    Checking file /Log/RuntimeServicesTest/TimeServicesTest0/SetTime_Conf_0_0_A8821B44-6CE4-462A-BCD9-527B1A22AF13.ekl (SETTIM~1.EKL)
    Orphaned long file name part "SetTime_Func_0_0_603B46BE-7E14-408A-93D7-DD9DEC732968.log"
      Auto-deleting.
    Checking file /Log/RuntimeServicesTest/TimeServicesTest0/SetTime_Func_0_0_603B46BE-7E14-408A-93D7-DD9DEC732968.log (SETTIM~1.LOG)
    Orphaned long file name part "SetTime_Func_0_0_603B46BE-7E14-408A-93D7-DD9DEC732968.ekl"
      Auto-deleting.
    Checking file /Log/RuntimeServicesTest/TimeServicesTest0/SetTime_Func_0_0_603B46BE-7E14-408A-93D7-DD9DEC732968.ekl (SETTIM~1.EKL)
    Orphaned long file name part "SetWakeupTime_Conf_0_0_8721B500-F13A-40FA-8217-70ACDDDC67BF.log"
      Auto-deleting.
    Checking file /Log/RuntimeServicesTest/TimeServicesTest0/SetWakeupTime_Conf_0_0_8721B500-F13A-40FA-8217-70ACDDDC67BF.log (SETWAK~1.LOG)
    Orphaned long file name part "SetWakeupTime_Conf_0_0_8721B500-F13A-40FA-8217-70ACDDDC67BF.ekl"
      Auto-deleting.
    Checking file /Log/RuntimeServicesTest/TimeServicesTest0/SetWakeupTime_Conf_0_0_8721B500-F13A-40FA-8217-70ACDDDC67BF.ekl (SETWAK~1.EKL)
    Orphaned long file name part "SetWakeupTime_Func_0_0_8A878BFB-6BE1-4226-8F69-4EBF7A1FF9A5.log"
      Auto-deleting.
    Checking file /Log/RuntimeServicesTest/TimeServicesTest0/SetWakeupTime_Func_0_0_8A878BFB-6BE1-4226-8F69-4EBF7A1FF9A5.log (SETWAK~1.LOG)
    Orphaned long file name part "SetWakeupTime_Func_0_0_8A878BFB-6BE1-4226-8F69-4EBF7A1FF9A5.ekl"
      Auto-deleting.
    Checking file /Log/RuntimeServicesTest/TimeServicesTest0/SetWakeupTime_Func_0_0_8A878BFB-6BE1-4226-8F69-4EBF7A1FF9A5.ekl (SETWAK~1.EKL)
    /Log/RuntimeServicesTest/TimeServicesTest0/GetTime_Conf_0_0_C3756910-91B4-4BBF-BF40-3315F13C2D4D.log
      Duplicate directory entry.
      First    Size 3018 bytes, date 01:00:00 Jan 01 1980
      Second   Size 6422 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.000
    /Log/RuntimeServicesTest/TimeServicesTest0/GetTime_Conf_0_0_C3756910-91B4-4BBF-BF40-3315F13C2D4D.ekl
      Duplicate directory entry.
      First    Size 964 bytes, date 01:00:00 Jan 01 1980
      Second   Size 4402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.001
    /Log/RuntimeServicesTest/TimeServicesTest0/GetWakeupTime_Conf_0_0_735BA337-2A44-46A2-AFAB-AFBED7358F08.log
      Duplicate directory entry.
      First    Size 3098 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3088 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.002
    /Log/RuntimeServicesTest/TimeServicesTest0/GetWakeupTime_Conf_0_0_735BA337-2A44-46A2-AFAB-AFBED7358F08.ekl
      Duplicate directory entry.
      First    Size 1082 bytes, date 01:00:00 Jan 01 1980
      Second   Size 1076 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.003
    /Log/RuntimeServicesTest/TimeServicesTest0/SetTime_Conf_0_0_A8821B44-6CE4-462A-BCD9-527B1A22AF13.log
      Duplicate directory entry.
      First    Size 12838 bytes, date 01:00:00 Jan 01 1980
      Second   Size 12920 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.004
    /Log/RuntimeServicesTest/TimeServicesTest0/SetTime_Conf_0_0_A8821B44-6CE4-462A-BCD9-527B1A22AF13.ekl
      Duplicate directory entry.
      First    Size 10682 bytes, date 01:00:00 Jan 01 1980
      Second   Size 8290 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.005
    /Log/RuntimeServicesTest/TimeServicesTest0/SetWakeupTime_Conf_0_0_8721B500-F13A-40FA-8217-70ACDDDC67BF.log
      Duplicate directory entry.
      First    Size 3098 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3088 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.006
    /Log/RuntimeServicesTest/TimeServicesTest0/SetWakeupTime_Conf_0_0_8721B500-F13A-40FA-8217-70ACDDDC67BF.ekl
      Duplicate directory entry.
      First    Size 1082 bytes, date 01:00:00 Jan 01 1980
      Second   Size 1074 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.007
    Checking file /Log/RuntimeServicesTest/MiscRuntimeServicesTest0/.
    Checking file /Log/RuntimeServicesTest/MiscRuntimeServicesTest0/..
    Orphaned long file name part "QueryCapsuleCapabilities_Conf_0_0_2411C48B-74D1-4E2F-942B-C31E54B5E1B4.log"
      Auto-deleting.
    Checking file /Log/RuntimeServicesTest/MiscRuntimeServicesTest0/QueryCapsuleCapabilities_Conf_0_0_2411C48B-74D1-4E2F-942B-C31E54B5E1B4.log (QUERYC~1.LOG)
    Orphaned long file name part "QueryCapsuleCapabilities_Conf_0_0_2411C48B-74D1-4E2F-942B-C31E54B5E1B4.ekl"
      Auto-deleting.
    Checking file /Log/RuntimeServicesTest/MiscRuntimeServicesTest0/QueryCapsuleCapabilities_Conf_0_0_2411C48B-74D1-4E2F-942B-C31E54B5E1B4.ekl (QUERYC~1.EKL)
    Orphaned long file name part "QueryCapsuleCapabilities_Func_0_0_72087EFE-F36C-4E46-8CCD-5E06A748BEF1.log"
      Auto-deleting.
    Checking file /Log/RuntimeServicesTest/MiscRuntimeServicesTest0/QueryCapsuleCapabilities_Func_0_0_72087EFE-F36C-4E46-8CCD-5E06A748BEF1.log (QUERYC~1.LOG)
    Orphaned long file name part "QueryCapsuleCapabilities_Func_0_0_72087EFE-F36C-4E46-8CCD-5E06A748BEF1.ekl"
      Auto-deleting.
    Checking file /Log/RuntimeServicesTest/MiscRuntimeServicesTest0/QueryCapsuleCapabilities_Func_0_0_72087EFE-F36C-4E46-8CCD-5E06A748BEF1.ekl (QUERYC~1.EKL)
    Orphaned long file name part "ResetSystem_Func_0_0_1DBEB615-9504-4E2F-BAFC-B3C6B2DEBC7B.log"
      Auto-deleting.
    Checking file /Log/RuntimeServicesTest/MiscRuntimeServicesTest0/ResetSystem_Func_0_0_1DBEB615-9504-4E2F-BAFC-B3C6B2DEBC7B.log (RESETS~1.LOG)
    Orphaned long file name part "ResetSystem_Func_0_0_1DBEB615-9504-4E2F-BAFC-B3C6B2DEBC7B.ekl"
      Auto-deleting.
    Checking file /Log/RuntimeServicesTest/MiscRuntimeServicesTest0/ResetSystem_Func_0_0_1DBEB615-9504-4E2F-BAFC-B3C6B2DEBC7B.ekl (RESETS~1.EKL)
    Orphaned long file name part "UpdateCapsule_Conf_0_0_7227CFAC-CA96-4680-9314-E3FBC60A2A61.log"
      Auto-deleting.
    Checking file /Log/RuntimeServicesTest/MiscRuntimeServicesTest0/UpdateCapsule_Conf_0_0_7227CFAC-CA96-4680-9314-E3FBC60A2A61.log (UPDATE~1.LOG)
    Orphaned long file name part "UpdateCapsule_Conf_0_0_7227CFAC-CA96-4680-9314-E3FBC60A2A61.ekl"
      Auto-deleting.
    Checking file /Log/RuntimeServicesTest/MiscRuntimeServicesTest0/UpdateCapsule_Conf_0_0_7227CFAC-CA96-4680-9314-E3FBC60A2A61.ekl (UPDATE~1.EKL)
    /Log/RuntimeServicesTest/MiscRuntimeServicesTest0/QueryCapsuleCapabilities_Conf_0_0_2411C48B-74D1-4E2F-942B-C31E54B5E1B4.log
      Duplicate directory entry.
      First    Size 3448 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3518 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.000
    /Log/RuntimeServicesTest/MiscRuntimeServicesTest0/QueryCapsuleCapabilities_Conf_0_0_2411C48B-74D1-4E2F-942B-C31E54B5E1B4.ekl
      Duplicate directory entry.
      First    Size 1280 bytes, date 01:00:00 Jan 01 1980
      Second   Size 1354 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.001
    Checking file /Log/LoadedImageProtocolTest0/.
    Checking file /Log/LoadedImageProtocolTest0/..
    Orphaned long file name part "LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_1_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_1_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_1_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_1_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_2_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_2_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_2_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_2_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_3_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_3_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_3_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_3_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_4_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_4_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_4_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_4_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_5_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_5_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_5_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_5_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_6_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_6_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_6_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_6_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_7_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_7_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_7_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_7_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_8_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_8_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_8_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_8_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_9_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_9_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_9_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_9_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_10_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_10_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_10_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_10_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_11_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_11_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_11_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_11_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_12_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_12_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_12_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_12_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_13_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_13_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_13_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_13_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_14_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_14_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_14_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_14_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_15_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_15_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_15_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_15_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_16_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_16_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_16_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_16_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_17_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_17_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_17_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_17_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_18_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_18_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_18_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_18_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_19_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_19_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_19_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_19_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_20_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_20_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_20_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_20_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_21_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_21_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_21_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_21_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_22_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_22_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_22_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_22_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_23_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_23_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_23_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_23_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_24_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_24_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_24_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_24_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_25_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_25_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_25_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_25_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_26_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_26_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_26_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_26_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_27_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_27_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_27_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_27_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_28_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_28_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_28_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_28_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_29_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_29_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_29_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_29_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_30_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_30_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_30_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_30_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_31_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_31_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_31_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_31_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_32_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_32_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_32_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_32_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_33_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_33_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_33_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_33_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_34_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_34_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_34_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_34_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_35_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_35_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_35_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_35_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_36_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_36_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_36_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_36_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_37_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_37_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_37_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_37_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_38_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_38_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_38_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_38_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_39_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_39_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_39_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_39_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_40_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_40_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_40_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_40_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_41_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_41_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_41_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_41_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_42_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_42_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_42_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_42_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_43_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_43_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_43_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_43_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_44_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_44_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_44_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_44_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_45_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_45_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_45_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_45_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_46_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_46_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_46_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_46_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_47_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_47_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_47_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_47_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_48_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_48_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_48_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_48_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_49_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_49_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_49_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_49_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_50_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_50_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_50_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_50_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_51_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_51_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_51_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_51_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_52_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_52_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_52_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_52_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_53_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_53_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_53_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_53_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_54_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_54_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_54_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_54_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_55_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_55_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_55_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_55_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_56_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_56_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_56_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_56_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_57_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_57_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_57_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_57_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_58_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_58_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_58_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_58_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_59_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_59_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_59_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_59_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_60_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_60_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_60_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_60_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_61_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_61_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_61_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_61_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_62_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_62_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_62_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_62_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_63_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_63_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_63_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_63_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_64_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_64_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_64_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_64_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_65_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_65_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_65_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_65_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_66_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_66_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_66_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_66_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_67_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_67_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_67_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_67_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_68_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_68_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_68_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_68_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_69_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_69_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_69_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_69_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_70_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_70_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_70_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_70_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_71_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_71_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_71_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_71_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_72_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_72_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_72_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_72_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_73_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_73_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_73_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_73_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_74_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_74_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_74_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_74_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_75_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_75_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_75_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_75_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_76_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_76_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_76_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_76_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_77_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_77_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_77_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_77_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_78_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_78_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_78_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_78_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_79_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_79_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_79_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_79_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_80_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_80_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_80_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_80_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_81_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_81_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_81_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_81_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest1_82_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_82_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest1_82_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_82_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_0_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_0_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_0_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_0_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_1_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_1_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_1_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_1_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_2_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_2_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_2_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_2_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_3_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_3_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_3_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_3_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_4_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_4_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_4_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_4_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_5_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_5_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_5_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_5_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_6_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_6_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_6_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_6_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_7_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_7_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_7_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_7_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_8_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_8_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_8_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_8_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_9_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_9_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_9_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_9_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_10_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_10_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_10_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_10_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_11_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_11_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_11_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_11_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_12_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_12_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_12_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_12_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_13_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_13_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_13_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_13_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_14_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_14_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_14_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_14_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_15_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_15_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_15_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_15_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_16_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_16_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_16_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_16_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_17_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_17_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_17_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_17_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_18_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_18_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_18_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_18_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_19_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_19_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_19_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_19_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_20_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_20_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_20_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_20_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_21_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_21_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_21_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_21_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_22_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_22_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_22_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_22_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_23_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_23_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_23_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_23_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_24_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_24_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_24_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_24_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_25_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_25_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_25_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_25_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_26_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_26_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_26_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_26_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_27_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_27_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_27_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_27_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_28_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_28_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_28_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_28_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_29_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_29_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_29_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_29_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_30_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_30_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_30_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_30_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_31_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_31_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_31_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_31_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_32_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_32_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_32_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_32_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_33_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_33_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_33_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_33_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_34_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_34_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_34_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_34_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_35_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_35_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_35_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_35_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_36_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_36_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_36_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_36_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_37_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_37_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_37_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_37_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_38_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_38_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_38_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_38_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_39_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_39_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_39_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_39_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_40_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_40_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_40_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_40_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_41_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_41_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_41_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_41_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_42_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_42_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_42_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_42_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_43_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_43_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_43_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_43_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_44_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_44_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_44_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_44_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_45_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_45_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_45_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_45_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_46_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_46_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_46_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_46_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_47_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_47_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_47_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_47_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_48_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_48_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_48_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_48_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_49_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_49_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_49_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_49_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_50_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_50_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_50_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_50_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_51_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_51_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_51_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_51_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_52_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_52_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_52_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_52_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_53_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_53_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_53_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_53_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_54_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_54_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_54_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_54_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_55_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_55_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_55_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_55_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_56_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_56_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_56_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_56_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_57_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_57_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_57_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_57_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_58_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_58_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_58_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_58_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_59_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_59_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_59_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_59_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_60_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_60_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_60_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_60_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_61_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_61_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_61_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_61_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_62_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_62_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_62_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_62_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_63_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_63_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_63_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_63_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_64_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_64_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_64_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_64_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_65_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_65_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_65_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_65_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_66_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_66_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_66_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_66_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_67_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_67_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_67_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_67_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_68_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_68_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_68_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_68_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_69_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_69_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_69_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_69_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_70_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_70_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_70_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_70_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_71_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_71_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_71_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_71_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_72_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_72_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_72_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_72_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_73_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_73_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_73_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_73_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_74_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_74_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_74_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_74_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_75_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_75_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_75_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_75_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_76_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_76_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_76_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_76_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_77_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_77_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_77_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_77_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_78_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_78_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_78_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_78_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_79_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_79_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_79_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_79_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_80_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_80_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_80_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_80_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_81_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_81_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_81_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_81_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    Orphaned long file name part "LoadedImageProtocolTest2_82_0_524114F0-FB32-494B-814D-9597059EE5C5.log"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_82_0_524114F0-FB32-494B-814D-9597059EE5C5.log (LOADED~1.LOG)
    Orphaned long file name part "LoadedImageProtocolTest2_82_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl"
      Auto-deleting.
    Checking file /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest2_82_0_524114F0-FB32-494B-814D-9597059EE5C5.ekl (LOADED~1.EKL)
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30032 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.000
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30032 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.001
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30032 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.002
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30032 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.003
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30032 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.004
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30032 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.005
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30032 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.006
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30032 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.007
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30032 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.008
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.009
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.010
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.011
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.012
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.013
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.014
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.015
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.016
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.017
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.018
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.019
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.020
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.021
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.022
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.023
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.024
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.025
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.026
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.027
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.028
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.029
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.030
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.031
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.032
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.033
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.034
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.035
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.036
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.037
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.038
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.039
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.040
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.041
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.042
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.043
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.044
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.045
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.046
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.047
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.048
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.049
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.050
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.051
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.052
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.053
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.054
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.055
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.056
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.057
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.058
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.059
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.060
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.061
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.062
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.063
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.064
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.065
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.066
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.067
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.068
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.069
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.070
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.071
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.072
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.073
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.074
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.075
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.076
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.077
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.078
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.079
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.080
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30036 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.081
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 4796 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.082
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 4796 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.083
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5342 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.084
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5342 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.085
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5342 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.086
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5342 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.087
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.088
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5342 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.089
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5342 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.090
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.091
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5350 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.092
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.093
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5350 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.094
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.095
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.096
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.097
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.098
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5350 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.099
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.100
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.101
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.102
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.103
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.104
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.105
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5350 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.106
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.107
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.108
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.109
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.110
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.111
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5350 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.112
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5350 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.113
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.114
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.115
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.116
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.117
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.118
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.119
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.120
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5350 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.121
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.122
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.123
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.124
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.125
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.126
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.127
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.128
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.129
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.130
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.131
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.132
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.133
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.134
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.135
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.136
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.137
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.138
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.139
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.140
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.141
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.142
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.143
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.144
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.145
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.146
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5350 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.147
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.148
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.149
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.150
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5350 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.151
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.152
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.153
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.154
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.155
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.156
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.157
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.158
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.159
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.160
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.161
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.162
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.163
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.log
      Duplicate directory entry.
      First    Size 30032 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.164
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.165
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.166
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.167
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.168
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.169
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.170
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.171
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.172
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.173
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.174
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.175
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.176
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.177
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.178
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.179
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.180
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.181
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.182
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.183
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.184
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.185
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.186
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.187
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.188
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.189
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.190
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.191
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.192
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.193
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.194
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.195
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.196
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.197
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.198
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.199
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.200
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.201
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.202
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.203
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.204
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.205
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.206
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.207
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.208
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.209
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.210
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.211
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.212
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.213
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.214
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.215
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.216
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.217
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.218
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.219
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.220
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.221
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.222
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.223
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.224
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.225
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.226
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.227
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.228
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.229
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.230
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.231
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.232
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.233
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.234
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.235
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.236
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.237
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.238
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.239
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.240
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.241
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.242
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.243
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.244
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.245
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27402 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.246
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 2704 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.247
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 2704 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.248
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.249
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.250
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.251
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.252
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3244 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.253
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.254
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.255
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3244 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.256
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3244 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.257
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.258
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3244 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.259
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.260
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.261
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.262
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.263
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3244 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.264
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.265
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.266
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.267
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.268
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.269
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.270
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3244 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.271
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.272
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.273
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.274
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.275
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.276
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3244 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.277
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3244 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.278
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.279
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.280
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.281
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.282
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.283
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.284
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.285
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3244 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.286
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.287
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.288
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.289
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.290
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.291
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.292
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.293
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.294
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.295
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.296
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.297
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.298
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.299
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.300
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.301
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.302
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.303
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.304
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.305
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.306
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.307
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.308
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.309
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.310
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.311
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3244 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.312
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.313
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.314
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.315
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3244 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.316
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.317
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.318
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.319
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.320
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.321
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.322
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.323
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.324
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.325
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.326
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.327
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.328
    /Log/LoadedImageProtocolTest0/LoadedImageProtocolTest1_0_0_DEBE1157-53D2-42A1-B6DE-E0D46C9ACED7.ekl
      Duplicate directory entry.
      First    Size 27402 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.329
    Checking file /Log/DevicePathProcotols/.
    Checking file /Log/DevicePathProcotols/..
    Checking file /Log/DevicePathProcotols/DevicePathProcotolTest0 (DEVICE~1)
    Checking file /Log/DevicePathProcotols/DevicePathUtilitiesProcotolTest0 (DEVICE~1)
    Checking file /Log/DevicePathProcotols/DevicePathToTextProcotolTest0 (DEVICE~1)
    /Log/DevicePathProcotols/DevicePathProcotolTest0
      Duplicate directory entry.
      First    Size 0 bytes, date 01:00:00 Dec 31 1979
      Second   Size 0 bytes, date 01:00:00 Dec 31 1979
      Auto-renaming second.
      Renamed to FSCK0000.000
    /Log/DevicePathProcotols/DevicePathProcotolTest0
      Duplicate directory entry.
      First    Size 0 bytes, date 01:00:00 Dec 31 1979
      Second   Size 0 bytes, date 01:00:00 Dec 31 1979
      Auto-renaming second.
      Renamed to FSCK0000.001
    Checking file /Log/DevicePathProcotols/DevicePathProcotolTest0/.
    Checking file /Log/DevicePathProcotols/DevicePathProcotolTest0/..
    Orphaned long file name part "PathNode_Conf_0_0_C24C24FA-4A52-4968-BA54-16570F09BCA3.log"
      Auto-deleting.
    Checking file /Log/DevicePathProcotols/DevicePathProcotolTest0/PathNode_Conf_0_0_C24C24FA-4A52-4968-BA54-16570F09BCA3.log (PATHNO~1.LOG)
    Orphaned long file name part "PathNode_Conf_0_0_C24C24FA-4A52-4968-BA54-16570F09BCA3.ekl"
      Auto-deleting.
    Checking file /Log/DevicePathProcotols/DevicePathProcotolTest0/PathNode_Conf_0_0_C24C24FA-4A52-4968-BA54-16570F09BCA3.ekl (PATHNO~1.EKL)
    Orphaned long file name part "PathNode_Conf_1_0_C24C24FA-4A52-4968-BA54-16570F09BCA3.log"
      Auto-deleting.
    Checking file /Log/DevicePathProcotols/DevicePathProcotolTest0/PathNode_Conf_1_0_C24C24FA-4A52-4968-BA54-16570F09BCA3.log (PATHNO~1.LOG)
    Orphaned long file name part "PathNode_Conf_1_0_C24C24FA-4A52-4968-BA54-16570F09BCA3.ekl"
      Auto-deleting.
    Checking file /Log/DevicePathProcotols/DevicePathProcotolTest0/PathNode_Conf_1_0_C24C24FA-4A52-4968-BA54-16570F09BCA3.ekl (PATHNO~1.EKL)
    Orphaned long file name part "PathNode_Conf_2_0_C24C24FA-4A52-4968-BA54-16570F09BCA3.log"
      Auto-deleting.
    Checking file /Log/DevicePathProcotols/DevicePathProcotolTest0/PathNode_Conf_2_0_C24C24FA-4A52-4968-BA54-16570F09BCA3.log (PATHNO~1.LOG)
    Orphaned long file name part "PathNode_Conf_2_0_C24C24FA-4A52-4968-BA54-16570F09BCA3.ekl"
      Auto-deleting.
    Checking file /Log/DevicePathProcotols/DevicePathProcotolTest0/PathNode_Conf_2_0_C24C24FA-4A52-4968-BA54-16570F09BCA3.ekl (PATHNO~1.EKL)
    Orphaned long file name part "PathNode_Conf_3_0_C24C24FA-4A52-4968-BA54-16570F09BCA3.log"
      Auto-deleting.
    Checking file /Log/DevicePathProcotols/DevicePathProcotolTest0/PathNode_Conf_3_0_C24C24FA-4A52-4968-BA54-16570F09BCA3.log (PATHNO~1.LOG)
    Orphaned long file name part "PathNode_Conf_3_0_C24C24FA-4A52-4968-BA54-16570F09BCA3.ekl"
      Auto-deleting.
    Checking file /Log/DevicePathProcotols/DevicePathProcotolTest0/PathNode_Conf_3_0_C24C24FA-4A52-4968-BA54-16570F09BCA3.ekl (PATHNO~1.EKL)
    /Log/DevicePathProcotols/DevicePathProcotolTest0/PathNode_Conf_0_0_C24C24FA-4A52-4968-BA54-16570F09BCA3.log
      Duplicate directory entry.
      First    Size 3924 bytes, date 01:00:00 Jan 01 1980
      Second   Size 4504 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.000
    /Log/DevicePathProcotols/DevicePathProcotolTest0/PathNode_Conf_0_0_C24C24FA-4A52-4968-BA54-16570F09BCA3.log
      Duplicate directory entry.
      First    Size 3924 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5116 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.001
    /Log/DevicePathProcotols/DevicePathProcotolTest0/PathNode_Conf_0_0_C24C24FA-4A52-4968-BA54-16570F09BCA3.log
      Duplicate directory entry.
      First    Size 3924 bytes, date 01:00:00 Jan 01 1980
      Second   Size 4574 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.002
    /Log/DevicePathProcotols/DevicePathProcotolTest0/PathNode_Conf_0_0_C24C24FA-4A52-4968-BA54-16570F09BCA3.ekl
      Duplicate directory entry.
      First    Size 1798 bytes, date 01:00:00 Jan 01 1980
      Second   Size 2368 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.003
    /Log/DevicePathProcotols/DevicePathProcotolTest0/PathNode_Conf_0_0_C24C24FA-4A52-4968-BA54-16570F09BCA3.ekl
      Duplicate directory entry.
      First    Size 1798 bytes, date 01:00:00 Jan 01 1980
      Second   Size 2970 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.004
    /Log/DevicePathProcotols/DevicePathProcotolTest0/PathNode_Conf_0_0_C24C24FA-4A52-4968-BA54-16570F09BCA3.ekl
      Duplicate directory entry.
      First    Size 1798 bytes, date 01:00:00 Jan 01 1980
      Second   Size 2438 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.005
    Checking file /Log/DevicePathProcotols/DevicePathUtilitiesProcotolTest0/.
    Checking file /Log/DevicePathProcotols/DevicePathUtilitiesProcotolTest0/..
    Orphaned long file name part "AppendDeviceNode_Conformance_0_0_88203701-B540-407C-97F0-CA8B2F872180.log"
      Auto-deleting.
    Checking file /Log/DevicePathProcotols/DevicePathUtilitiesProcotolTest0/AppendDeviceNode_Conformance_0_0_88203701-B540-407C-97F0-CA8B2F872180.log (APPEND~1.LOG)
    Orphaned long file name part "AppendDeviceNode_Conformance_0_0_88203701-B540-407C-97F0-CA8B2F872180.ekl"
      Auto-deleting.
    Checking file /Log/DevicePathProcotols/DevicePathUtilitiesProcotolTest0/AppendDeviceNode_Conformance_0_0_88203701-B540-407C-97F0-CA8B2F872180.ekl (APPEND~1.EKL)
    Orphaned long file name part "AppendDeviceNode_Functionality_0_0_E80D2CCD-CF48-437C-9559-FB98D09933CA.log"
      Auto-deleting.
    Checking file /Log/DevicePathProcotols/DevicePathUtilitiesProcotolTest0/AppendDeviceNode_Functionality_0_0_E80D2CCD-CF48-437C-9559-FB98D09933CA.log (APPEND~1.LOG)
    Orphaned long file name part "AppendDeviceNode_Functionality_0_0_E80D2CCD-CF48-437C-9559-FB98D09933CA.ekl"
      Auto-deleting.
    Checking file /Log/DevicePathProcotols/DevicePathUtilitiesProcotolTest0/AppendDeviceNode_Functionality_0_0_E80D2CCD-CF48-437C-9559-FB98D09933CA.ekl (APPEND~1.EKL)
    Orphaned long file name part "AppendDevicePathInstance_Conformance_0_0_05F7832C-F274-4D65-B869-7B361F079EAA.log"
      Auto-deleting.
    Checking file /Log/DevicePathProcotols/DevicePathUtilitiesProcotolTest0/AppendDevicePathInstance_Conformance_0_0_05F7832C-F274-4D65-B869-7B361F079EAA.log (APPEND~1.LOG)
    Orphaned long file name part "AppendDevicePathInstance_Conformance_0_0_05F7832C-F274-4D65-B869-7B361F079EAA.ekl"
      Auto-deleting.
    Checking file /Log/DevicePathProcotols/DevicePathUtilitiesProcotolTest0/AppendDevicePathInstance_Conformance_0_0_05F7832C-F274-4D65-B869-7B361F079EAA.ekl (APPEND~1.EKL)
    Orphaned long file name part "AppendDevicePathInstance_Functionality_0_0_71299E5E-A094-40DD-A043-E765F358A3A6.log"
      Auto-deleting.
    Checking file /Log/DevicePathProcotols/DevicePathUtilitiesProcotolTest0/AppendDevicePathInstance_Functionality_0_0_71299E5E-A094-40DD-A043-E765F358A3A6.log (APPEND~1.LOG)
    Orphaned long file name part "AppendDevicePathInstance_Functionality_0_0_71299E5E-A094-40DD-A043-E765F358A3A6.ekl"
      Auto-deleting.
    Checking file /Log/DevicePathProcotols/DevicePathUtilitiesProcotolTest0/AppendDevicePathInstance_Functionality_0_0_71299E5E-A094-40DD-A043-E765F358A3A6.ekl (APPEND~1.EKL)
    Orphaned long file name part "AppendDevicePath_Conformance_0_0_91E4223C-F958-44CB-A65C-C4FD445CD158.log"
      Auto-deleting.
    Checking file /Log/DevicePathProcotols/DevicePathUtilitiesProcotolTest0/AppendDevicePath_Conformance_0_0_91E4223C-F958-44CB-A65C-C4FD445CD158.log (APPEND~1.LOG)
    Orphaned long file name part "AppendDevicePath_Conformance_0_0_91E4223C-F958-44CB-A65C-C4FD445CD158.ekl"
      Auto-deleting.
    Checking file /Log/DevicePathProcotols/DevicePathUtilitiesProcotolTest0/AppendDevicePath_Conformance_0_0_91E4223C-F958-44CB-A65C-C4FD445CD158.ekl (APPEND~1.EKL)
    Orphaned long file name part "AppendDevicePath_Functionality_0_0_1BCEC639-96E1-4DAF-886B-853589107F04.log"
      Auto-deleting.
    Checking file /Log/DevicePathProcotols/DevicePathUtilitiesProcotolTest0/AppendDevicePath_Functionality_0_0_1BCEC639-96E1-4DAF-886B-853589107F04.log (APPEND~1.LOG)
    Orphaned long file name part "AppendDevicePath_Functionality_0_0_1BCEC639-96E1-4DAF-886B-853589107F04.ekl"
      Auto-deleting.
    Checking file /Log/DevicePathProcotols/DevicePathUtilitiesProcotolTest0/AppendDevicePath_Functionality_0_0_1BCEC639-96E1-4DAF-886B-853589107F04.ekl (APPEND~1.EKL)
    Orphaned long file name part "CreatDeviceNode_Functionality_0_0_FDA477C2-3678-4C81-B308-6283F248F214.log"
      Auto-deleting.
    Checking file /Log/DevicePathProcotols/DevicePathUtilitiesProcotolTest0/CreatDeviceNode_Functionality_0_0_FDA477C2-3678-4C81-B308-6283F248F214.log (CREATD~1.LOG)
    Orphaned long file name part "CreatDeviceNode_Functionality_0_0_FDA477C2-3678-4C81-B308-6283F248F214.ekl"
      Auto-deleting.
    Checking file /Log/DevicePathProcotols/DevicePathUtilitiesProcotolTest0/CreatDeviceNode_Functionality_0_0_FDA477C2-3678-4C81-B308-6283F248F214.ekl (CREATD~1.EKL)
    Orphaned long file name part "CreateDeviceNode_Conformance_0_0_6FFC463D-16EE-46DF-B942-0FAD75C983C8.log"
      Auto-deleting.
    Checking file /Log/DevicePathProcotols/DevicePathUtilitiesProcotolTest0/CreateDeviceNode_Conformance_0_0_6FFC463D-16EE-46DF-B942-0FAD75C983C8.log (CREATE~1.LOG)
    Orphaned long file name part "CreateDeviceNode_Conformance_0_0_6FFC463D-16EE-46DF-B942-0FAD75C983C8.ekl"
      Auto-deleting.
    Checking file /Log/DevicePathProcotols/DevicePathUtilitiesProcotolTest0/CreateDeviceNode_Conformance_0_0_6FFC463D-16EE-46DF-B942-0FAD75C983C8.ekl (CREATE~1.EKL)
    Orphaned long file name part "DuplicateDevicePath_Functionality_0_0_615C73A8-6E80-4C9B-80C5-242B239B0725.log"
      Auto-deleting.
    Checking file /Log/DevicePathProcotols/DevicePathUtilitiesProcotolTest0/DuplicateDevicePath_Functionality_0_0_615C73A8-6E80-4C9B-80C5-242B239B0725.log (DUPLIC~1.LOG)
    Orphaned long file name part "DuplicateDevicePath_Functionality_0_0_615C73A8-6E80-4C9B-80C5-242B239B0725.ekl"
      Auto-deleting.
    Checking file /Log/DevicePathProcotols/DevicePathUtilitiesProcotolTest0/DuplicateDevicePath_Functionality_0_0_615C73A8-6E80-4C9B-80C5-242B239B0725.ekl (DUPLIC~1.EKL)
    Orphaned long file name part "DuplicateDevicePath_Conformance_0_0_74C9CD0A-348E-4AE4-91A2-7799E5432BBD.log"
      Auto-deleting.
    Checking file /Log/DevicePathProcotols/DevicePathUtilitiesProcotolTest0/DuplicateDevicePath_Conformance_0_0_74C9CD0A-348E-4AE4-91A2-7799E5432BBD.log (DUPLIC~1.LOG)
    Orphaned long file name part "DuplicateDevicePath_Conformance_0_0_74C9CD0A-348E-4AE4-91A2-7799E5432BBD.ekl"
      Auto-deleting.
    Checking file /Log/DevicePathProcotols/DevicePathUtilitiesProcotolTest0/DuplicateDevicePath_Conformance_0_0_74C9CD0A-348E-4AE4-91A2-7799E5432BBD.ekl (DUPLIC~1.EKL)
    Orphaned long file name part "GetDevicePathSize_Conformance_0_0_A2FBC1F0-35C3-42B9-B81F-5B30E14FFF2E.log"
      Auto-deleting.
    Checking file /Log/DevicePathProcotols/DevicePathUtilitiesProcotolTest0/GetDevicePathSize_Conformance_0_0_A2FBC1F0-35C3-42B9-B81F-5B30E14FFF2E.log (GETDEV~1.LOG)
    Orphaned long file name part "GetDevicePathSize_Conformance_0_0_A2FBC1F0-35C3-42B9-B81F-5B30E14FFF2E.ekl"
      Auto-deleting.
    Checking file /Log/DevicePathProcotols/DevicePathUtilitiesProcotolTest0/GetDevicePathSize_Conformance_0_0_A2FBC1F0-35C3-42B9-B81F-5B30E14FFF2E.ekl (GETDEV~1.EKL)
    Orphaned long file name part "GetDevicePathSize_Functionality_0_0_EA0908E7-4A59-4660-9FF6-B50764365591.log"
      Auto-deleting.
    Checking file /Log/DevicePathProcotols/DevicePathUtilitiesProcotolTest0/GetDevicePathSize_Functionality_0_0_EA0908E7-4A59-4660-9FF6-B50764365591.log (GETDEV~1.LOG)
    Orphaned long file name part "GetDevicePathSize_Functionality_0_0_EA0908E7-4A59-4660-9FF6-B50764365591.ekl"
      Auto-deleting.
    Checking file /Log/DevicePathProcotols/DevicePathUtilitiesProcotolTest0/GetDevicePathSize_Functionality_0_0_EA0908E7-4A59-4660-9FF6-B50764365591.ekl (GETDEV~1.EKL)
    Orphaned long file name part "GetNextDevicePathInstance_Conformance_0_0_3DDC0D17-610E-48EE-B2B7-5C10FAD2C8F5.log"
      Auto-deleting.
    Checking file /Log/DevicePathProcotols/DevicePathUtilitiesProcotolTest0/GetNextDevicePathInstance_Conformance_0_0_3DDC0D17-610E-48EE-B2B7-5C10FAD2C8F5.log (GETNEX~1.LOG)
    Orphaned long file name part "GetNextDevicePathInstance_Conformance_0_0_3DDC0D17-610E-48EE-B2B7-5C10FAD2C8F5.ekl"
      Auto-deleting.
    Checking file /Log/DevicePathProcotols/DevicePathUtilitiesProcotolTest0/GetNextDevicePathInstance_Conformance_0_0_3DDC0D17-610E-48EE-B2B7-5C10FAD2C8F5.ekl (GETNEX~1.EKL)
    Orphaned long file name part "GetNextDevicePathInstance_Functionality_0_0_2A2C4286-9B68-4C46-B7DD-B32B4B859AD4.log"
      Auto-deleting.
    Checking file /Log/DevicePathProcotols/DevicePathUtilitiesProcotolTest0/GetNextDevicePathInstance_Functionality_0_0_2A2C4286-9B68-4C46-B7DD-B32B4B859AD4.log (GETNEX~1.LOG)
    Orphaned long file name part "GetNextDevicePathInstance_Functionality_0_0_2A2C4286-9B68-4C46-B7DD-B32B4B859AD4.ekl"
      Auto-deleting.
    Checking file /Log/DevicePathProcotols/DevicePathUtilitiesProcotolTest0/GetNextDevicePathInstance_Functionality_0_0_2A2C4286-9B68-4C46-B7DD-B32B4B859AD4.ekl (GETNEX~1.EKL)
    Orphaned long file name part "IsDevicePathMultiInstance_Functionality_0_0_57C31FAF-A85F-45CD-934F-757C910A00FB.log"
      Auto-deleting.
    Checking file /Log/DevicePathProcotols/DevicePathUtilitiesProcotolTest0/IsDevicePathMultiInstance_Functionality_0_0_57C31FAF-A85F-45CD-934F-757C910A00FB.log (ISDEVI~1.LOG)
    Orphaned long file name part "IsDevicePathMultiInstance_Functionality_0_0_57C31FAF-A85F-45CD-934F-757C910A00FB.ekl"
      Auto-deleting.
    Checking file /Log/DevicePathProcotols/DevicePathUtilitiesProcotolTest0/IsDevicePathMultiInstance_Functionality_0_0_57C31FAF-A85F-45CD-934F-757C910A00FB.ekl (ISDEVI~1.EKL)
    /Log/DevicePathProcotols/DevicePathUtilitiesProcotolTest0/AppendDeviceNode_Conformance_0_0_88203701-B540-407C-97F0-CA8B2F872180.log
      Duplicate directory entry.
      First    Size 4672 bytes, date 01:00:00 Jan 01 1980
      Second   Size 4444 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.000
    /Log/DevicePathProcotols/DevicePathUtilitiesProcotolTest0/AppendDeviceNode_Conformance_0_0_88203701-B540-407C-97F0-CA8B2F872180.log
      Duplicate directory entry.
      First    Size 4672 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3528 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.001
    /Log/DevicePathProcotols/DevicePathUtilitiesProcotolTest0/AppendDeviceNode_Conformance_0_0_88203701-B540-407C-97F0-CA8B2F872180.log
      Duplicate directory entry.
      First    Size 4672 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3766 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.002
    /Log/DevicePathProcotols/DevicePathUtilitiesProcotolTest0/AppendDeviceNode_Conformance_0_0_88203701-B540-407C-97F0-CA8B2F872180.log
      Duplicate directory entry.
      First    Size 4672 bytes, date 01:00:00 Jan 01 1980
      Second   Size 4642 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.003
    /Log/DevicePathProcotols/DevicePathUtilitiesProcotolTest0/AppendDeviceNode_Conformance_0_0_88203701-B540-407C-97F0-CA8B2F872180.log
      Duplicate directory entry.
      First    Size 4672 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3624 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.004
    /Log/DevicePathProcotols/DevicePathUtilitiesProcotolTest0/AppendDeviceNode_Conformance_0_0_88203701-B540-407C-97F0-CA8B2F872180.ekl
      Duplicate directory entry.
      First    Size 2608 bytes, date 01:00:00 Jan 01 1980
      Second   Size 2340 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.005
    /Log/DevicePathProcotols/DevicePathUtilitiesProcotolTest0/AppendDeviceNode_Conformance_0_0_88203701-B540-407C-97F0-CA8B2F872180.ekl
      Duplicate directory entry.
      First    Size 2608 bytes, date 01:00:00 Jan 01 1980
      Second   Size 1382 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.006
    /Log/DevicePathProcotols/DevicePathUtilitiesProcotolTest0/AppendDeviceNode_Conformance_0_0_88203701-B540-407C-97F0-CA8B2F872180.ekl
      Duplicate directory entry.
      First    Size 2608 bytes, date 01:00:00 Jan 01 1980
      Second   Size 1608 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.007
    /Log/DevicePathProcotols/DevicePathUtilitiesProcotolTest0/AppendDeviceNode_Conformance_0_0_88203701-B540-407C-97F0-CA8B2F872180.ekl
      Duplicate directory entry.
      First    Size 2608 bytes, date 01:00:00 Jan 01 1980
      Second   Size 2578 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.008
    /Log/DevicePathProcotols/DevicePathUtilitiesProcotolTest0/AppendDeviceNode_Conformance_0_0_88203701-B540-407C-97F0-CA8B2F872180.ekl
      Duplicate directory entry.
      First    Size 2608 bytes, date 01:00:00 Jan 01 1980
      Second   Size 1530 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.009
    /Log/DevicePathProcotols/DevicePathUtilitiesProcotolTest0/DuplicateDevicePath_Functionality_0_0_615C73A8-6E80-4C9B-80C5-242B239B0725.log
      Duplicate directory entry.
      First    Size 3568 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3408 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.010
    /Log/DevicePathProcotols/DevicePathUtilitiesProcotolTest0/DuplicateDevicePath_Functionality_0_0_615C73A8-6E80-4C9B-80C5-242B239B0725.ekl
      Duplicate directory entry.
      First    Size 1450 bytes, date 01:00:00 Jan 01 1980
      Second   Size 1240 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.011
    /Log/DevicePathProcotols/DevicePathUtilitiesProcotolTest0/GetDevicePathSize_Conformance_0_0_A2FBC1F0-35C3-42B9-B81F-5B30E14FFF2E.log
      Duplicate directory entry.
      First    Size 3372 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3596 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.012
    /Log/DevicePathProcotols/DevicePathUtilitiesProcotolTest0/GetDevicePathSize_Conformance_0_0_A2FBC1F0-35C3-42B9-B81F-5B30E14FFF2E.ekl
      Duplicate directory entry.
      First    Size 1220 bytes, date 01:00:00 Jan 01 1980
      Second   Size 1494 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.013
    /Log/DevicePathProcotols/DevicePathUtilitiesProcotolTest0/GetNextDevicePathInstance_Conformance_0_0_3DDC0D17-610E-48EE-B2B7-5C10FAD2C8F5.log
      Duplicate directory entry.
      First    Size 3540 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3706 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.014
    /Log/DevicePathProcotols/DevicePathUtilitiesProcotolTest0/GetNextDevicePathInstance_Conformance_0_0_3DDC0D17-610E-48EE-B2B7-5C10FAD2C8F5.ekl
      Duplicate directory entry.
      First    Size 1386 bytes, date 01:00:00 Jan 01 1980
      Second   Size 1540 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.015
    Checking file /Log/DevicePathProcotols/DevicePathToTextProcotolTest0/.
    Checking file /Log/DevicePathProcotols/DevicePathToTextProcotolTest0/..
    Orphaned long file name part "ConvertDeviceNodeToText_Conformance_0_0_60E1B540-3351-455B-B9F9-86625B7A154E.log"
      Auto-deleting.
    Checking file /Log/DevicePathProcotols/DevicePathToTextProcotolTest0/ConvertDeviceNodeToText_Conformance_0_0_60E1B540-3351-455B-B9F9-86625B7A154E.log (CONVER~1.LOG)
    Orphaned long file name part "ConvertDeviceNodeToText_Conformance_0_0_60E1B540-3351-455B-B9F9-86625B7A154E.ekl"
      Auto-deleting.
    Checking file /Log/DevicePathProcotols/DevicePathToTextProcotolTest0/ConvertDeviceNodeToText_Conformance_0_0_60E1B540-3351-455B-B9F9-86625B7A154E.ekl (CONVER~1.EKL)
    Orphaned long file name part "ConvertDeviceNodeToText_Coverage_0_0_C843762A-8D11-46B8-8417-97A892809AB0.log"
      Auto-deleting.
    Checking file /Log/DevicePathProcotols/DevicePathToTextProcotolTest0/ConvertDeviceNodeToText_Coverage_0_0_C843762A-8D11-46B8-8417-97A892809AB0.log (CONVER~1.LOG)
    Orphaned long file name part "ConvertDeviceNodeToText_Coverage_0_0_C843762A-8D11-46B8-8417-97A892809AB0.ekl"
      Auto-deleting.
    Checking file /Log/DevicePathProcotols/DevicePathToTextProcotolTest0/ConvertDeviceNodeToText_Coverage_0_0_C843762A-8D11-46B8-8417-97A892809AB0.ekl (CONVER~1.EKL)
    Orphaned long file name part "ConvertDeviceNodeToText_Functionality_0_0_A9092653-D44E-407F-A51E-940BE4770A26.log"
      Auto-deleting.
    Checking file /Log/DevicePathProcotols/DevicePathToTextProcotolTest0/ConvertDeviceNodeToText_Functionality_0_0_A9092653-D44E-407F-A51E-940BE4770A26.log (CONVER~1.LOG)
    Orphaned long file name part "ConvertDeviceNodeToText_Functionality_0_0_A9092653-D44E-407F-A51E-940BE4770A26.ekl"
      Auto-deleting.
    Checking file /Log/DevicePathProcotols/DevicePathToTextProcotolTest0/ConvertDeviceNodeToText_Functionality_0_0_A9092653-D44E-407F-A51E-940BE4770A26.ekl (CONVER~1.EKL)
    Orphaned long file name part "ConvertDevicePathToText_Conformance_0_0_F8489292-27F2-4AA6-A433-6D57A80B4A91.log"
      Auto-deleting.
    Checking file /Log/DevicePathProcotols/DevicePathToTextProcotolTest0/ConvertDevicePathToText_Conformance_0_0_F8489292-27F2-4AA6-A433-6D57A80B4A91.log (CONVER~1.LOG)
    Orphaned long file name part "ConvertDevicePathToText_Conformance_0_0_F8489292-27F2-4AA6-A433-6D57A80B4A91.ekl"
      Auto-deleting.
    Checking file /Log/DevicePathProcotols/DevicePathToTextProcotolTest0/ConvertDevicePathToText_Conformance_0_0_F8489292-27F2-4AA6-A433-6D57A80B4A91.ekl (CONVER~1.EKL)
    Orphaned long file name part "ConvertDevicePathToText_Functionality_0_0_1AB644BA-1CB5-4533-B5CD-301EEB5C09D4.log"
      Auto-deleting.
    Checking file /Log/DevicePathProcotols/DevicePathToTextProcotolTest0/ConvertDevicePathToText_Functionality_0_0_1AB644BA-1CB5-4533-B5CD-301EEB5C09D4.log (CONVER~1.LOG)
    Orphaned long file name part "ConvertDevicePathToText_Functionality_0_0_1AB644BA-1CB5-4533-B5CD-301EEB5C09D4.ekl"
      Auto-deleting.
    Checking file /Log/DevicePathProcotols/DevicePathToTextProcotolTest0/ConvertDevicePathToText_Functionality_0_0_1AB644BA-1CB5-4533-B5CD-301EEB5C09D4.ekl (CONVER~1.EKL)
    /Log/DevicePathProcotols/DevicePathToTextProcotolTest0/ConvertDeviceNodeToText_Conformance_0_0_60E1B540-3351-455B-B9F9-86625B7A154E.log
      Duplicate directory entry.
      First    Size 3434 bytes, date 01:00:00 Jan 01 1980
      Second   Size 48070 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.000
    /Log/DevicePathProcotols/DevicePathToTextProcotolTest0/ConvertDeviceNodeToText_Conformance_0_0_60E1B540-3351-455B-B9F9-86625B7A154E.log
      Duplicate directory entry.
      First    Size 3434 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5126 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.001
    /Log/DevicePathProcotols/DevicePathToTextProcotolTest0/ConvertDeviceNodeToText_Conformance_0_0_60E1B540-3351-455B-B9F9-86625B7A154E.log
      Duplicate directory entry.
      First    Size 3434 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3436 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.002
    /Log/DevicePathProcotols/DevicePathToTextProcotolTest0/ConvertDeviceNodeToText_Conformance_0_0_60E1B540-3351-455B-B9F9-86625B7A154E.log
      Duplicate directory entry.
      First    Size 3434 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5506 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.003
    /Log/DevicePathProcotols/DevicePathToTextProcotolTest0/ConvertDeviceNodeToText_Conformance_0_0_60E1B540-3351-455B-B9F9-86625B7A154E.ekl
      Duplicate directory entry.
      First    Size 1298 bytes, date 01:00:00 Jan 01 1980
      Second   Size 45346 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.004
    /Log/DevicePathProcotols/DevicePathToTextProcotolTest0/ConvertDeviceNodeToText_Conformance_0_0_60E1B540-3351-455B-B9F9-86625B7A154E.ekl
      Duplicate directory entry.
      First    Size 1298 bytes, date 01:00:00 Jan 01 1980
      Second   Size 2958 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.005
    /Log/DevicePathProcotols/DevicePathToTextProcotolTest0/ConvertDeviceNodeToText_Conformance_0_0_60E1B540-3351-455B-B9F9-86625B7A154E.ekl
      Duplicate directory entry.
      First    Size 1298 bytes, date 01:00:00 Jan 01 1980
      Second   Size 1300 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.006
    /Log/DevicePathProcotols/DevicePathToTextProcotolTest0/ConvertDeviceNodeToText_Conformance_0_0_60E1B540-3351-455B-B9F9-86625B7A154E.ekl
      Duplicate directory entry.
      First    Size 1298 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3338 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.007
    Checking file /Log/NetworkSupportTest/.
    Checking file /Log/NetworkSupportTest/..
    Checking file /Log/NetworkSupportTest/SimpleNetworkProtocolTest0 (SIMPLE~1)
    Checking file /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/.
    Checking file /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/..
    Orphaned long file name part "GetStatus_Conf_0_0_574C0B74-ADC3-46D9-A8FF-C8A44E6646FA.log"
      Auto-deleting.
    Checking file /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/GetStatus_Conf_0_0_574C0B74-ADC3-46D9-A8FF-C8A44E6646FA.log (GETSTA~1.LOG)
    Orphaned long file name part "GetStatus_Conf_0_0_574C0B74-ADC3-46D9-A8FF-C8A44E6646FA.ekl"
      Auto-deleting.
    Checking file /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/GetStatus_Conf_0_0_574C0B74-ADC3-46D9-A8FF-C8A44E6646FA.ekl (GETSTA~1.EKL)
    Orphaned long file name part "GetStatus_Func_0_0_85270BDF-5C38-47FC-A7DF-F30C9A740AAE.log"
      Auto-deleting.
    Checking file /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/GetStatus_Func_0_0_85270BDF-5C38-47FC-A7DF-F30C9A740AAE.log (GETSTA~1.LOG)
    Orphaned long file name part "GetStatus_Func_0_0_85270BDF-5C38-47FC-A7DF-F30C9A740AAE.ekl"
      Auto-deleting.
    Checking file /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/GetStatus_Func_0_0_85270BDF-5C38-47FC-A7DF-F30C9A740AAE.ekl (GETSTA~1.EKL)
    Orphaned long file name part "Initialize_Conf_0_0_BBDCEE3C-3E90-4AE3-ABE5-6CACEC8B6B23.log"
      Auto-deleting.
    Checking file /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/Initialize_Conf_0_0_BBDCEE3C-3E90-4AE3-ABE5-6CACEC8B6B23.log (INITIA~1.LOG)
    Orphaned long file name part "Initialize_Conf_0_0_BBDCEE3C-3E90-4AE3-ABE5-6CACEC8B6B23.ekl"
      Auto-deleting.
    Checking file /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/Initialize_Conf_0_0_BBDCEE3C-3E90-4AE3-ABE5-6CACEC8B6B23.ekl (INITIA~1.EKL)
    Orphaned long file name part "Initialize_Func_0_0_87689738-8DC6-4E4B-AE76-17CD96390956.log"
      Auto-deleting.
    Checking file /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/Initialize_Func_0_0_87689738-8DC6-4E4B-AE76-17CD96390956.log (INITIA~1.LOG)
    Orphaned long file name part "Initialize_Func_0_0_87689738-8DC6-4E4B-AE76-17CD96390956.ekl"
      Auto-deleting.
    Checking file /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/Initialize_Func_0_0_87689738-8DC6-4E4B-AE76-17CD96390956.ekl (INITIA~1.EKL)
    Orphaned long file name part "MCastIpToMac_Conf_0_0_D924B177-7E44-445D-92AA-5E15C0FD2E27.log"
      Auto-deleting.
    Checking file /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/MCastIpToMac_Conf_0_0_D924B177-7E44-445D-92AA-5E15C0FD2E27.log (MCASTI~1.LOG)
    Orphaned long file name part "MCastIpToMac_Conf_0_0_D924B177-7E44-445D-92AA-5E15C0FD2E27.ekl"
      Auto-deleting.
    Checking file /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/MCastIpToMac_Conf_0_0_D924B177-7E44-445D-92AA-5E15C0FD2E27.ekl (MCASTI~1.EKL)
    Orphaned long file name part "MCastIpToMac_Func_0_0_3DE1C94C-4CBB-47C4-9407-0C0F20FA66E7.log"
      Auto-deleting.
    Checking file /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/MCastIpToMac_Func_0_0_3DE1C94C-4CBB-47C4-9407-0C0F20FA66E7.log (MCASTI~1.LOG)
    Orphaned long file name part "MCastIpToMac_Func_0_0_3DE1C94C-4CBB-47C4-9407-0C0F20FA66E7.ekl"
      Auto-deleting.
    Checking file /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/MCastIpToMac_Func_0_0_3DE1C94C-4CBB-47C4-9407-0C0F20FA66E7.ekl (MCASTI~1.EKL)
    Orphaned long file name part "NVData_Conf_0_0_5408EB9D-B40A-47DD-BD04-E9A8B906661F.log"
      Auto-deleting.
    Checking file /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/NVData_Conf_0_0_5408EB9D-B40A-47DD-BD04-E9A8B906661F.log (NVDATA~1.LOG)
    Orphaned long file name part "NVData_Conf_0_0_5408EB9D-B40A-47DD-BD04-E9A8B906661F.ekl"
      Auto-deleting.
    Checking file /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/NVData_Conf_0_0_5408EB9D-B40A-47DD-BD04-E9A8B906661F.ekl (NVDATA~1.EKL)
    Orphaned long file name part "NVData_Func_0_0_426BE7F5-3F47-4919-9F77-C142BB0C9B27.log"
      Auto-deleting.
    Checking file /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/NVData_Func_0_0_426BE7F5-3F47-4919-9F77-C142BB0C9B27.log (NVDATA~1.LOG)
    Orphaned long file name part "NVData_Func_0_0_426BE7F5-3F47-4919-9F77-C142BB0C9B27.ekl"
      Auto-deleting.
    Checking file /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/NVData_Func_0_0_426BE7F5-3F47-4919-9F77-C142BB0C9B27.ekl (NVDATA~1.EKL)
    Orphaned long file name part "ReceiveFilter_Conf_0_0_534A9E0F-B31B-40C5-AD60-DF02C55361D4.log"
      Auto-deleting.
    Checking file /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/ReceiveFilter_Conf_0_0_534A9E0F-B31B-40C5-AD60-DF02C55361D4.log (RECEIV~1.LOG)
    Orphaned long file name part "ReceiveFilter_Conf_0_0_534A9E0F-B31B-40C5-AD60-DF02C55361D4.ekl"
      Auto-deleting.
    Checking file /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/ReceiveFilter_Conf_0_0_534A9E0F-B31B-40C5-AD60-DF02C55361D4.ekl (RECEIV~1.EKL)
    Orphaned long file name part "ReceiveFilter_Func_0_0_7A1E587D-53AC-444E-A5A1-81CD3F4F04D4.log"
      Auto-deleting.
    Checking file /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/ReceiveFilter_Func_0_0_7A1E587D-53AC-444E-A5A1-81CD3F4F04D4.log (RECEIV~1.LOG)
    Orphaned long file name part "ReceiveFilter_Func_0_0_7A1E587D-53AC-444E-A5A1-81CD3F4F04D4.ekl"
      Auto-deleting.
    Checking file /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/ReceiveFilter_Func_0_0_7A1E587D-53AC-444E-A5A1-81CD3F4F04D4.ekl (RECEIV~1.EKL)
    Orphaned long file name part "Receive_Conf_0_0_E648317F-90AA-4C8A-B0A7-8880F322DA54.log"
      Auto-deleting.
    Checking file /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/Receive_Conf_0_0_E648317F-90AA-4C8A-B0A7-8880F322DA54.log (RECEIV~1.LOG)
    Orphaned long file name part "Receive_Conf_0_0_E648317F-90AA-4C8A-B0A7-8880F322DA54.ekl"
      Auto-deleting.
    Checking file /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/Receive_Conf_0_0_E648317F-90AA-4C8A-B0A7-8880F322DA54.ekl (RECEIV~1.EKL)
    Orphaned long file name part "Reset_Conf_0_0_D15DD19B-9CBF-40B8-9776-C15EC53F6089.log"
      Auto-deleting.
    Checking file /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/Reset_Conf_0_0_D15DD19B-9CBF-40B8-9776-C15EC53F6089.log (RESET_~1.LOG)
    Orphaned long file name part "Reset_Conf_0_0_D15DD19B-9CBF-40B8-9776-C15EC53F6089.ekl"
      Auto-deleting.
    Checking file /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/Reset_Conf_0_0_D15DD19B-9CBF-40B8-9776-C15EC53F6089.ekl (RESET_~1.EKL)
    Orphaned long file name part "Reset_Func_0_0_BA628A58-E318-4E4A-BAC2-A7833ADF42D9.log"
      Auto-deleting.
    Checking file /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/Reset_Func_0_0_BA628A58-E318-4E4A-BAC2-A7833ADF42D9.log (RESET_~1.LOG)
    Orphaned long file name part "Reset_Func_0_0_BA628A58-E318-4E4A-BAC2-A7833ADF42D9.ekl"
      Auto-deleting.
    Checking file /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/Reset_Func_0_0_BA628A58-E318-4E4A-BAC2-A7833ADF42D9.ekl (RESET_~1.EKL)
    Orphaned long file name part "Shutdown_Conf_0_0_54C6EE8B-6B40-4536-8DAB-682FE13B25B4.log"
      Auto-deleting.
    Checking file /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/Shutdown_Conf_0_0_54C6EE8B-6B40-4536-8DAB-682FE13B25B4.log (SHUTDO~1.LOG)
    Orphaned long file name part "Shutdown_Conf_0_0_54C6EE8B-6B40-4536-8DAB-682FE13B25B4.ekl"
      Auto-deleting.
    Checking file /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/Shutdown_Conf_0_0_54C6EE8B-6B40-4536-8DAB-682FE13B25B4.ekl (SHUTDO~1.EKL)
    Orphaned long file name part "Shutdown_Func_0_0_6DD174AF-4706-4DE2-813C-239B250E7289.log"
      Auto-deleting.
    Checking file /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/Shutdown_Func_0_0_6DD174AF-4706-4DE2-813C-239B250E7289.log (SHUTDO~1.LOG)
    Orphaned long file name part "Shutdown_Func_0_0_6DD174AF-4706-4DE2-813C-239B250E7289.ekl"
      Auto-deleting.
    Checking file /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/Shutdown_Func_0_0_6DD174AF-4706-4DE2-813C-239B250E7289.ekl (SHUTDO~1.EKL)
    Orphaned long file name part "Start_Conf_0_0_352E6069-8282-49F8-BCED-850FF87CA31B.log"
      Auto-deleting.
    Checking file /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/Start_Conf_0_0_352E6069-8282-49F8-BCED-850FF87CA31B.log (START_~1.LOG)
    Orphaned long file name part "Start_Conf_0_0_352E6069-8282-49F8-BCED-850FF87CA31B.ekl"
      Auto-deleting.
    Checking file /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/Start_Conf_0_0_352E6069-8282-49F8-BCED-850FF87CA31B.ekl (START_~1.EKL)
    Orphaned long file name part "Start_Func_0_0_E6215C64-FC31-4A15-AA0A-BD9EF297B76A.log"
      Auto-deleting.
    Checking file /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/Start_Func_0_0_E6215C64-FC31-4A15-AA0A-BD9EF297B76A.log (START_~1.LOG)
    Orphaned long file name part "Start_Func_0_0_E6215C64-FC31-4A15-AA0A-BD9EF297B76A.ekl"
      Auto-deleting.
    Checking file /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/Start_Func_0_0_E6215C64-FC31-4A15-AA0A-BD9EF297B76A.ekl (START_~1.EKL)
    Orphaned long file name part "StationAddress_Conf_0_0_EC8714E0-2AB9-46E9-8F35-508334B118A7.log"
      Auto-deleting.
    Checking file /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/StationAddress_Conf_0_0_EC8714E0-2AB9-46E9-8F35-508334B118A7.log (STATIO~1.LOG)
    Orphaned long file name part "StationAddress_Conf_0_0_EC8714E0-2AB9-46E9-8F35-508334B118A7.ekl"
      Auto-deleting.
    Checking file /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/StationAddress_Conf_0_0_EC8714E0-2AB9-46E9-8F35-508334B118A7.ekl (STATIO~1.EKL)
    Orphaned long file name part "StationAddress_Func_0_0_762FCCB6-5CDB-4E23-8890-45CD233CD16F.log"
      Auto-deleting.
    Checking file /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/StationAddress_Func_0_0_762FCCB6-5CDB-4E23-8890-45CD233CD16F.log (STATIO~1.LOG)
    Orphaned long file name part "StationAddress_Func_0_0_762FCCB6-5CDB-4E23-8890-45CD233CD16F.ekl"
      Auto-deleting.
    Checking file /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/StationAddress_Func_0_0_762FCCB6-5CDB-4E23-8890-45CD233CD16F.ekl (STATIO~1.EKL)
    Orphaned long file name part "Statistics_Conf_0_0_122DD1F0-AF8E-4D3B-884B-14C2FF7AEFA7.log"
      Auto-deleting.
    Checking file /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/Statistics_Conf_0_0_122DD1F0-AF8E-4D3B-884B-14C2FF7AEFA7.log (STATIS~1.LOG)
    Orphaned long file name part "Statistics_Conf_0_0_122DD1F0-AF8E-4D3B-884B-14C2FF7AEFA7.ekl"
      Auto-deleting.
    Checking file /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/Statistics_Conf_0_0_122DD1F0-AF8E-4D3B-884B-14C2FF7AEFA7.ekl (STATIS~1.EKL)
    Orphaned long file name part "Statistics_Func_0_0_43E4BBA9-7570-4ADF-BCE7-1CDE3855B668.log"
      Auto-deleting.
    Checking file /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/Statistics_Func_0_0_43E4BBA9-7570-4ADF-BCE7-1CDE3855B668.log (STATIS~1.LOG)
    Orphaned long file name part "Statistics_Func_0_0_43E4BBA9-7570-4ADF-BCE7-1CDE3855B668.ekl"
      Auto-deleting.
    Checking file /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/Statistics_Func_0_0_43E4BBA9-7570-4ADF-BCE7-1CDE3855B668.ekl (STATIS~1.EKL)
    Orphaned long file name part "Stop_Conf_0_0_23CB3934-7327-45B1-B6D9-3B8F84613C9E.log"
      Auto-deleting.
    Checking file /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/Stop_Conf_0_0_23CB3934-7327-45B1-B6D9-3B8F84613C9E.log (STOP_C~1.LOG)
    Orphaned long file name part "Stop_Conf_0_0_23CB3934-7327-45B1-B6D9-3B8F84613C9E.ekl"
      Auto-deleting.
    Checking file /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/Stop_Conf_0_0_23CB3934-7327-45B1-B6D9-3B8F84613C9E.ekl (STOP_C~1.EKL)
    Orphaned long file name part "Stop_Func_0_0_3649957D-51DA-423D-A8AB-3C81161F1144.log"
      Auto-deleting.
    Checking file /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/Stop_Func_0_0_3649957D-51DA-423D-A8AB-3C81161F1144.log (STOP_F~1.LOG)
    Orphaned long file name part "Stop_Func_0_0_3649957D-51DA-423D-A8AB-3C81161F1144.ekl"
      Auto-deleting.
    Checking file /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/Stop_Func_0_0_3649957D-51DA-423D-A8AB-3C81161F1144.ekl (STOP_F~1.EKL)
    Orphaned long file name part "Transmit_Conf_0_0_5DDF5C49-7ACA-4724-9553-614A53EE998A.log"
      Auto-deleting.
    Checking file /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/Transmit_Conf_0_0_5DDF5C49-7ACA-4724-9553-614A53EE998A.log (TRANSM~1.LOG)
    Orphaned long file name part "Transmit_Conf_0_0_5DDF5C49-7ACA-4724-9553-614A53EE998A.ekl"
      Auto-deleting.
    Checking file /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/Transmit_Conf_0_0_5DDF5C49-7ACA-4724-9553-614A53EE998A.ekl (TRANSM~1.EKL)
    /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/GetStatus_Conf_0_0_574C0B74-ADC3-46D9-A8FF-C8A44E6646FA.log
      Duplicate directory entry.
      First    Size 3802 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3208 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.000
    /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/GetStatus_Conf_0_0_574C0B74-ADC3-46D9-A8FF-C8A44E6646FA.ekl
      Duplicate directory entry.
      First    Size 1910 bytes, date 01:00:00 Jan 01 1980
      Second   Size 1180 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.001
    /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/Initialize_Conf_0_0_BBDCEE3C-3E90-4AE3-ABE5-6CACEC8B6B23.log
      Duplicate directory entry.
      First    Size 3198 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3876 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.002
    /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/Initialize_Conf_0_0_BBDCEE3C-3E90-4AE3-ABE5-6CACEC8B6B23.ekl
      Duplicate directory entry.
      First    Size 1318 bytes, date 01:00:00 Jan 01 1980
      Second   Size 1992 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.003
    /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/MCastIpToMac_Conf_0_0_D924B177-7E44-445D-92AA-5E15C0FD2E27.log
      Duplicate directory entry.
      First    Size 3228 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3324 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.004
    /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/MCastIpToMac_Conf_0_0_D924B177-7E44-445D-92AA-5E15C0FD2E27.ekl
      Duplicate directory entry.
      First    Size 1332 bytes, date 01:00:00 Jan 01 1980
      Second   Size 1434 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.005
    /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/NVData_Conf_0_0_5408EB9D-B40A-47DD-BD04-E9A8B906661F.log
      Duplicate directory entry.
      First    Size 2716 bytes, date 01:00:00 Jan 01 1980
      Second   Size 2710 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.006
    /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/NVData_Conf_0_0_5408EB9D-B40A-47DD-BD04-E9A8B906661F.ekl
      Duplicate directory entry.
      First    Size 564 bytes, date 01:00:00 Jan 01 1980
      Second   Size 584 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.007
    /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/ReceiveFilter_Conf_0_0_534A9E0F-B31B-40C5-AD60-DF02C55361D4.log
      Duplicate directory entry.
      First    Size 2984 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3458 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.008
    /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/ReceiveFilter_Conf_0_0_534A9E0F-B31B-40C5-AD60-DF02C55361D4.log
      Duplicate directory entry.
      First    Size 2984 bytes, date 01:00:00 Jan 01 1980
      Second   Size 4326 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.009
    /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/ReceiveFilter_Conf_0_0_534A9E0F-B31B-40C5-AD60-DF02C55361D4.ekl
      Duplicate directory entry.
      First    Size 598 bytes, date 01:00:00 Jan 01 1980
      Second   Size 1418 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.010
    /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/ReceiveFilter_Conf_0_0_534A9E0F-B31B-40C5-AD60-DF02C55361D4.ekl
      Duplicate directory entry.
      First    Size 598 bytes, date 01:00:00 Jan 01 1980
      Second   Size 2470 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.011
    /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/Reset_Conf_0_0_D15DD19B-9CBF-40B8-9776-C15EC53F6089.log
      Duplicate directory entry.
      First    Size 3128 bytes, date 01:00:00 Jan 01 1980
      Second   Size 2570 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.012
    /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/Reset_Conf_0_0_D15DD19B-9CBF-40B8-9776-C15EC53F6089.ekl
      Duplicate directory entry.
      First    Size 1308 bytes, date 01:00:00 Jan 01 1980
      Second   Size 582 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.013
    /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/Shutdown_Conf_0_0_54C6EE8B-6B40-4536-8DAB-682FE13B25B4.log
      Duplicate directory entry.
      First    Size 3170 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3182 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.014
    /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/Shutdown_Conf_0_0_54C6EE8B-6B40-4536-8DAB-682FE13B25B4.ekl
      Duplicate directory entry.
      First    Size 1326 bytes, date 01:00:00 Jan 01 1980
      Second   Size 1344 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.015
    /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/Start_Conf_0_0_352E6069-8282-49F8-BCED-850FF87CA31B.log
      Duplicate directory entry.
      First    Size 3148 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3140 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.016
    /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/Start_Conf_0_0_352E6069-8282-49F8-BCED-850FF87CA31B.ekl
      Duplicate directory entry.
      First    Size 1328 bytes, date 01:00:00 Jan 01 1980
      Second   Size 1326 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.017
    /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/StationAddress_Conf_0_0_EC8714E0-2AB9-46E9-8F35-508334B118A7.log
      Duplicate directory entry.
      First    Size 2882 bytes, date 01:00:00 Jan 01 1980
      Second   Size 2876 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.018
    /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/StationAddress_Conf_0_0_EC8714E0-2AB9-46E9-8F35-508334B118A7.ekl
      Duplicate directory entry.
      First    Size 600 bytes, date 01:00:00 Jan 01 1980
      Second   Size 600 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.019
    /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/Statistics_Conf_0_0_122DD1F0-AF8E-4D3B-884B-14C2FF7AEFA7.log
      Duplicate directory entry.
      First    Size 2930 bytes, date 01:00:00 Jan 01 1980
      Second   Size 8552 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.020
    /Log/NetworkSupportTest/SimpleNetworkProtocolTest0/Statistics_Conf_0_0_122DD1F0-AF8E-4D3B-884B-14C2FF7AEFA7.ekl
      Duplicate directory entry.
      First    Size 604 bytes, date 01:00:00 Jan 01 1980
      Second   Size 1884 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.021
    Checking file /Log/StringServiceTest/.
    Checking file /Log/StringServiceTest/..
    Checking file /Log/StringServiceTest/UnicodeCollation2ProtocolTest0 (UNICOD~1)
    Checking file /Log/StringServiceTest/UnicodeCollation2ProtocolTest0/.
    Checking file /Log/StringServiceTest/UnicodeCollation2ProtocolTest0/..
    Orphaned long file name part "FatToStr_Func_0_0_74A6E2FF-9629-4914-A071-C1BB1ADC8693.log"
      Auto-deleting.
    Checking file /Log/StringServiceTest/UnicodeCollation2ProtocolTest0/FatToStr_Func_0_0_74A6E2FF-9629-4914-A071-C1BB1ADC8693.log (FATTOS~1.LOG)
    Orphaned long file name part "FatToStr_Func_0_0_74A6E2FF-9629-4914-A071-C1BB1ADC8693.ekl"
      Auto-deleting.
    Checking file /Log/StringServiceTest/UnicodeCollation2ProtocolTest0/FatToStr_Func_0_0_74A6E2FF-9629-4914-A071-C1BB1ADC8693.ekl (FATTOS~1.EKL)
    Orphaned long file name part "MetaiMatch_Func_0_0_9E918792-90DA-47B2-A602-A3FE7911A27F.log"
      Auto-deleting.
    Checking file /Log/StringServiceTest/UnicodeCollation2ProtocolTest0/MetaiMatch_Func_0_0_9E918792-90DA-47B2-A602-A3FE7911A27F.log (METAIM~1.LOG)
    Orphaned long file name part "MetaiMatch_Func_0_0_9E918792-90DA-47B2-A602-A3FE7911A27F.ekl"
      Auto-deleting.
    Checking file /Log/StringServiceTest/UnicodeCollation2ProtocolTest0/MetaiMatch_Func_0_0_9E918792-90DA-47B2-A602-A3FE7911A27F.ekl (METAIM~1.EKL)
    Orphaned long file name part "StriColl_Func_0_0_DAD20219-422F-43DA-A1FA-85CBE2EDD9C9.log"
      Auto-deleting.
    Checking file /Log/StringServiceTest/UnicodeCollation2ProtocolTest0/StriColl_Func_0_0_DAD20219-422F-43DA-A1FA-85CBE2EDD9C9.log (STRICO~1.LOG)
    Orphaned long file name part "StriColl_Func_0_0_DAD20219-422F-43DA-A1FA-85CBE2EDD9C9.ekl"
      Auto-deleting.
    Checking file /Log/StringServiceTest/UnicodeCollation2ProtocolTest0/StriColl_Func_0_0_DAD20219-422F-43DA-A1FA-85CBE2EDD9C9.ekl (STRICO~1.EKL)
    Orphaned long file name part "StrLwr_Func_0_0_81CD6598-8530-4765-866C-CD674904642A.log"
      Auto-deleting.
    Checking file /Log/StringServiceTest/UnicodeCollation2ProtocolTest0/StrLwr_Func_0_0_81CD6598-8530-4765-866C-CD674904642A.log (STRLWR~1.LOG)
    Orphaned long file name part "StrLwr_Func_0_0_81CD6598-8530-4765-866C-CD674904642A.ekl"
      Auto-deleting.
    Checking file /Log/StringServiceTest/UnicodeCollation2ProtocolTest0/StrLwr_Func_0_0_81CD6598-8530-4765-866C-CD674904642A.ekl (STRLWR~1.EKL)
    Orphaned long file name part "StrToFat_Func_0_0_089376CC-6530-4653-8052-606B8D5F564F.log"
      Auto-deleting.
    Checking file /Log/StringServiceTest/UnicodeCollation2ProtocolTest0/StrToFat_Func_0_0_089376CC-6530-4653-8052-606B8D5F564F.log (STRTOF~1.LOG)
    Orphaned long file name part "StrToFat_Func_0_0_089376CC-6530-4653-8052-606B8D5F564F.ekl"
      Auto-deleting.
    Checking file /Log/StringServiceTest/UnicodeCollation2ProtocolTest0/StrToFat_Func_0_0_089376CC-6530-4653-8052-606B8D5F564F.ekl (STRTOF~1.EKL)
    Orphaned long file name part "StrUpr_Func_0_0_5A3A67B4-812D-4B1B-B303-3C3AC87B9718.log"
      Auto-deleting.
    Checking file /Log/StringServiceTest/UnicodeCollation2ProtocolTest0/StrUpr_Func_0_0_5A3A67B4-812D-4B1B-B303-3C3AC87B9718.log (STRUPR~1.LOG)
    Orphaned long file name part "StrUpr_Func_0_0_5A3A67B4-812D-4B1B-B303-3C3AC87B9718.ekl"
      Auto-deleting.
    Checking file /Log/StringServiceTest/UnicodeCollation2ProtocolTest0/StrUpr_Func_0_0_5A3A67B4-812D-4B1B-B303-3C3AC87B9718.ekl (STRUPR~1.EKL)
    Checking file /Log/ConsoleSupportTest/.
    Checking file /Log/ConsoleSupportTest/..
    Checking file /Log/ConsoleSupportTest/SimpleTextInputExProtocolTest0 (SIMPLE~1)
    Checking file /Log/ConsoleSupportTest/SimpleInputProtocolTest0 (SIMPLE~1)
    Checking file /Log/ConsoleSupportTest/SimpleOutputProtocolTest0 (SIMPLE~1)
    /Log/ConsoleSupportTest/SimpleTextInputExProtocolTest0
      Duplicate directory entry.
      First    Size 0 bytes, date 01:00:00 Dec 31 1979
      Second   Size 0 bytes, date 01:00:00 Dec 31 1979
      Auto-renaming second.
      Renamed to FSCK0000.000
    /Log/ConsoleSupportTest/SimpleTextInputExProtocolTest0
      Duplicate directory entry.
      First    Size 0 bytes, date 01:00:00 Dec 31 1979
      Second   Size 0 bytes, date 01:00:00 Dec 31 1979
      Auto-renaming second.
      Renamed to FSCK0000.001
    Checking file /Log/ConsoleSupportTest/SimpleTextInputExProtocolTest0/.
    Checking file /Log/ConsoleSupportTest/SimpleTextInputExProtocolTest0/..
    Orphaned long file name part "ReadKeyStrokeExConformance_0_0_BF81459A-C896-4E68-A33C-41CAE1106108.log"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleTextInputExProtocolTest0/ReadKeyStrokeExConformance_0_0_BF81459A-C896-4E68-A33C-41CAE1106108.log (READKE~1.LOG)
    Orphaned long file name part "ReadKeyStrokeExConformance_0_0_BF81459A-C896-4E68-A33C-41CAE1106108.ekl"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleTextInputExProtocolTest0/ReadKeyStrokeExConformance_0_0_BF81459A-C896-4E68-A33C-41CAE1106108.ekl (READKE~1.EKL)
    Orphaned long file name part "RegisterKeyNotifyConformance_0_0_4CFF3A2D-9DD0-485B-83D7-4EC2DA93C0B9.log"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleTextInputExProtocolTest0/RegisterKeyNotifyConformance_0_0_4CFF3A2D-9DD0-485B-83D7-4EC2DA93C0B9.log (REGIST~1.LOG)
    Orphaned long file name part "RegisterKeyNotifyConformance_0_0_4CFF3A2D-9DD0-485B-83D7-4EC2DA93C0B9.ekl"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleTextInputExProtocolTest0/RegisterKeyNotifyConformance_0_0_4CFF3A2D-9DD0-485B-83D7-4EC2DA93C0B9.ekl (REGIST~1.EKL)
    Orphaned long file name part "ResetFunctionAuto_0_0_50EFBF91-EA77-468B-A5DA-C9813D99AC04.log"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleTextInputExProtocolTest0/ResetFunctionAuto_0_0_50EFBF91-EA77-468B-A5DA-C9813D99AC04.log (RESETF~1.LOG)
    Orphaned long file name part "ResetFunctionAuto_0_0_50EFBF91-EA77-468B-A5DA-C9813D99AC04.ekl"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleTextInputExProtocolTest0/ResetFunctionAuto_0_0_50EFBF91-EA77-468B-A5DA-C9813D99AC04.ekl (RESETF~1.EKL)
    Orphaned long file name part "SetStateConformance_0_0_5B40A8A9-F77A-4134-9FF1-417720B765B4.log"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleTextInputExProtocolTest0/SetStateConformance_0_0_5B40A8A9-F77A-4134-9FF1-417720B765B4.log (SETSTA~1.LOG)
    Orphaned long file name part "SetStateConformance_0_0_5B40A8A9-F77A-4134-9FF1-417720B765B4.ekl"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleTextInputExProtocolTest0/SetStateConformance_0_0_5B40A8A9-F77A-4134-9FF1-417720B765B4.ekl (SETSTA~1.EKL)
    Orphaned long file name part "UnregisterKeyNotifyConformance_0_0_4A1ED648-8328-4E1C-B64A-AFC3F4066FAF.log"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleTextInputExProtocolTest0/UnregisterKeyNotifyConformance_0_0_4A1ED648-8328-4E1C-B64A-AFC3F4066FAF.log (UNREGI~1.LOG)
    Orphaned long file name part "UnregisterKeyNotifyConformance_0_0_4A1ED648-8328-4E1C-B64A-AFC3F4066FAF.ekl"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleTextInputExProtocolTest0/UnregisterKeyNotifyConformance_0_0_4A1ED648-8328-4E1C-B64A-AFC3F4066FAF.ekl (UNREGI~1.EKL)
    Checking file /Log/ConsoleSupportTest/SimpleInputProtocolTest0/.
    Checking file /Log/ConsoleSupportTest/SimpleInputProtocolTest0/..
    Orphaned long file name part "Reset_Func_0_0_156A250F-D164-4305-BDFB-1E62B97F6D88.log"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleInputProtocolTest0/Reset_Func_0_0_156A250F-D164-4305-BDFB-1E62B97F6D88.log (RESET_~1.LOG)
    Orphaned long file name part "Reset_Func_0_0_156A250F-D164-4305-BDFB-1E62B97F6D88.ekl"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleInputProtocolTest0/Reset_Func_0_0_156A250F-D164-4305-BDFB-1E62B97F6D88.ekl (RESET_~1.EKL)
    Checking file /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/.
    Checking file /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/..
    Orphaned long file name part "ClearScreen_Func_0_0_D3533D69-75A9-46E0-9F50-A556232F4390.log"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/ClearScreen_Func_0_0_D3533D69-75A9-46E0-9F50-A556232F4390.log (CLEARS~1.LOG)
    Orphaned long file name part "ClearScreen_Func_0_0_D3533D69-75A9-46E0-9F50-A556232F4390.ekl"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/ClearScreen_Func_0_0_D3533D69-75A9-46E0-9F50-A556232F4390.ekl (CLEARS~1.EKL)
    Orphaned long file name part "ClearScreen_Func_1_0_D3533D69-75A9-46E0-9F50-A556232F4390.log"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/ClearScreen_Func_1_0_D3533D69-75A9-46E0-9F50-A556232F4390.log (CLEARS~1.LOG)
    Orphaned long file name part "ClearScreen_Func_1_0_D3533D69-75A9-46E0-9F50-A556232F4390.ekl"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/ClearScreen_Func_1_0_D3533D69-75A9-46E0-9F50-A556232F4390.ekl (CLEARS~1.EKL)
    Orphaned long file name part "EnableCursor_Func_0_0_4558978E-F938-424E-B3A4-48D4EFA522A5.log"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/EnableCursor_Func_0_0_4558978E-F938-424E-B3A4-48D4EFA522A5.log (ENABLE~1.LOG)
    Orphaned long file name part "EnableCursor_Func_0_0_4558978E-F938-424E-B3A4-48D4EFA522A5.ekl"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/EnableCursor_Func_0_0_4558978E-F938-424E-B3A4-48D4EFA522A5.ekl (ENABLE~1.EKL)
    Orphaned long file name part "EnableCursor_Func_1_0_4558978E-F938-424E-B3A4-48D4EFA522A5.log"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/EnableCursor_Func_1_0_4558978E-F938-424E-B3A4-48D4EFA522A5.log (ENABLE~1.LOG)
    Orphaned long file name part "EnableCursor_Func_1_0_4558978E-F938-424E-B3A4-48D4EFA522A5.ekl"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/EnableCursor_Func_1_0_4558978E-F938-424E-B3A4-48D4EFA522A5.ekl (ENABLE~1.EKL)
    Orphaned long file name part "OutputString_Func_0_0_A50A89D5-89C1-4214-8096-08C87910976F.log"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/OutputString_Func_0_0_A50A89D5-89C1-4214-8096-08C87910976F.log (OUTPUT~1.LOG)
    Orphaned long file name part "OutputString_Func_0_0_A50A89D5-89C1-4214-8096-08C87910976F.ekl"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/OutputString_Func_0_0_A50A89D5-89C1-4214-8096-08C87910976F.ekl (OUTPUT~1.EKL)
    Orphaned long file name part "OutputString_Func_1_0_A50A89D5-89C1-4214-8096-08C87910976F.log"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/OutputString_Func_1_0_A50A89D5-89C1-4214-8096-08C87910976F.log (OUTPUT~1.LOG)
    Orphaned long file name part "OutputString_Func_1_0_A50A89D5-89C1-4214-8096-08C87910976F.ekl"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/OutputString_Func_1_0_A50A89D5-89C1-4214-8096-08C87910976F.ekl (OUTPUT~1.EKL)
    Orphaned long file name part "QueryMode_Conf_0_0_64F2E0F9-87C6-4D4E-BB04-2D4E60FA29A5.log"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/QueryMode_Conf_0_0_64F2E0F9-87C6-4D4E-BB04-2D4E60FA29A5.log (QUERYM~1.LOG)
    Orphaned long file name part "QueryMode_Conf_0_0_64F2E0F9-87C6-4D4E-BB04-2D4E60FA29A5.ekl"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/QueryMode_Conf_0_0_64F2E0F9-87C6-4D4E-BB04-2D4E60FA29A5.ekl (QUERYM~1.EKL)
    Orphaned long file name part "QueryMode_Conf_1_0_64F2E0F9-87C6-4D4E-BB04-2D4E60FA29A5.log"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/QueryMode_Conf_1_0_64F2E0F9-87C6-4D4E-BB04-2D4E60FA29A5.log (QUERYM~1.LOG)
    Orphaned long file name part "QueryMode_Conf_1_0_64F2E0F9-87C6-4D4E-BB04-2D4E60FA29A5.ekl"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/QueryMode_Conf_1_0_64F2E0F9-87C6-4D4E-BB04-2D4E60FA29A5.ekl (QUERYM~1.EKL)
    Orphaned long file name part "QueryMode_Func_0_0_D493E3FD-6B56-4F8E-BA45-606D0E8F5671.log"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/QueryMode_Func_0_0_D493E3FD-6B56-4F8E-BA45-606D0E8F5671.log (QUERYM~1.LOG)
    Orphaned long file name part "QueryMode_Func_0_0_D493E3FD-6B56-4F8E-BA45-606D0E8F5671.ekl"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/QueryMode_Func_0_0_D493E3FD-6B56-4F8E-BA45-606D0E8F5671.ekl (QUERYM~1.EKL)
    Orphaned long file name part "QueryMode_Func_1_0_D493E3FD-6B56-4F8E-BA45-606D0E8F5671.log"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/QueryMode_Func_1_0_D493E3FD-6B56-4F8E-BA45-606D0E8F5671.log (QUERYM~1.LOG)
    Orphaned long file name part "QueryMode_Func_1_0_D493E3FD-6B56-4F8E-BA45-606D0E8F5671.ekl"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/QueryMode_Func_1_0_D493E3FD-6B56-4F8E-BA45-606D0E8F5671.ekl (QUERYM~1.EKL)
    Orphaned long file name part "Reset_Func_0_0_36BDBF05-2759-49CA-B128-BE19BE46EF6F.log"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/Reset_Func_0_0_36BDBF05-2759-49CA-B128-BE19BE46EF6F.log (RESET_~1.LOG)
    Orphaned long file name part "Reset_Func_0_0_36BDBF05-2759-49CA-B128-BE19BE46EF6F.ekl"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/Reset_Func_0_0_36BDBF05-2759-49CA-B128-BE19BE46EF6F.ekl (RESET_~1.EKL)
    Orphaned long file name part "Reset_Func_1_0_36BDBF05-2759-49CA-B128-BE19BE46EF6F.log"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/Reset_Func_1_0_36BDBF05-2759-49CA-B128-BE19BE46EF6F.log (RESET_~1.LOG)
    Orphaned long file name part "Reset_Func_1_0_36BDBF05-2759-49CA-B128-BE19BE46EF6F.ekl"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/Reset_Func_1_0_36BDBF05-2759-49CA-B128-BE19BE46EF6F.ekl (RESET_~1.EKL)
    Orphaned long file name part "SetAttribute_Func_0_0_07937289-8337-4B7B-ACE9-9182704FCBE8.log"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/SetAttribute_Func_0_0_07937289-8337-4B7B-ACE9-9182704FCBE8.log (SETATT~1.LOG)
    Orphaned long file name part "SetAttribute_Func_0_0_07937289-8337-4B7B-ACE9-9182704FCBE8.ekl"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/SetAttribute_Func_0_0_07937289-8337-4B7B-ACE9-9182704FCBE8.ekl (SETATT~1.EKL)
    Orphaned long file name part "SetAttribute_Func_1_0_07937289-8337-4B7B-ACE9-9182704FCBE8.log"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/SetAttribute_Func_1_0_07937289-8337-4B7B-ACE9-9182704FCBE8.log (SETATT~1.LOG)
    Orphaned long file name part "SetAttribute_Func_1_0_07937289-8337-4B7B-ACE9-9182704FCBE8.ekl"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/SetAttribute_Func_1_0_07937289-8337-4B7B-ACE9-9182704FCBE8.ekl (SETATT~1.EKL)
    Orphaned long file name part "SetCursorPosition_Conf_0_0_B07194F2-E025-42EB-B9E4-964A4FA64C8C.log"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/SetCursorPosition_Conf_0_0_B07194F2-E025-42EB-B9E4-964A4FA64C8C.log (SETCUR~1.LOG)
    Orphaned long file name part "SetCursorPosition_Conf_0_0_B07194F2-E025-42EB-B9E4-964A4FA64C8C.ekl"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/SetCursorPosition_Conf_0_0_B07194F2-E025-42EB-B9E4-964A4FA64C8C.ekl (SETCUR~1.EKL)
    Orphaned long file name part "SetCursorPosition_Conf_1_0_B07194F2-E025-42EB-B9E4-964A4FA64C8C.log"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/SetCursorPosition_Conf_1_0_B07194F2-E025-42EB-B9E4-964A4FA64C8C.log (SETCUR~1.LOG)
    Orphaned long file name part "SetCursorPosition_Conf_1_0_B07194F2-E025-42EB-B9E4-964A4FA64C8C.ekl"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/SetCursorPosition_Conf_1_0_B07194F2-E025-42EB-B9E4-964A4FA64C8C.ekl (SETCUR~1.EKL)
    Orphaned long file name part "SetCursorPosition_Func_0_0_87F03E4B-37DE-4C91-A6DE-3356E245E2C5.log"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/SetCursorPosition_Func_0_0_87F03E4B-37DE-4C91-A6DE-3356E245E2C5.log (SETCUR~1.LOG)
    Orphaned long file name part "SetCursorPosition_Func_0_0_87F03E4B-37DE-4C91-A6DE-3356E245E2C5.ekl"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/SetCursorPosition_Func_0_0_87F03E4B-37DE-4C91-A6DE-3356E245E2C5.ekl (SETCUR~1.EKL)
    Orphaned long file name part "SetCursorPosition_Func_1_0_87F03E4B-37DE-4C91-A6DE-3356E245E2C5.log"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/SetCursorPosition_Func_1_0_87F03E4B-37DE-4C91-A6DE-3356E245E2C5.log (SETCUR~1.LOG)
    Orphaned long file name part "SetCursorPosition_Func_1_0_87F03E4B-37DE-4C91-A6DE-3356E245E2C5.ekl"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/SetCursorPosition_Func_1_0_87F03E4B-37DE-4C91-A6DE-3356E245E2C5.ekl (SETCUR~1.EKL)
    Orphaned long file name part "SetMode_Conf_0_0_37F5C015-E5A2-4089-A94B-CC9721A81C2D.log"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/SetMode_Conf_0_0_37F5C015-E5A2-4089-A94B-CC9721A81C2D.log (SETMOD~1.LOG)
    Orphaned long file name part "SetMode_Conf_0_0_37F5C015-E5A2-4089-A94B-CC9721A81C2D.ekl"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/SetMode_Conf_0_0_37F5C015-E5A2-4089-A94B-CC9721A81C2D.ekl (SETMOD~1.EKL)
    Orphaned long file name part "SetMode_Conf_1_0_37F5C015-E5A2-4089-A94B-CC9721A81C2D.log"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/SetMode_Conf_1_0_37F5C015-E5A2-4089-A94B-CC9721A81C2D.log (SETMOD~1.LOG)
    Orphaned long file name part "SetMode_Conf_1_0_37F5C015-E5A2-4089-A94B-CC9721A81C2D.ekl"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/SetMode_Conf_1_0_37F5C015-E5A2-4089-A94B-CC9721A81C2D.ekl (SETMOD~1.EKL)
    Orphaned long file name part "SetMode_Func_0_0_6FA016C7-0428-4997-86FA-8F05A1265DC8.log"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/SetMode_Func_0_0_6FA016C7-0428-4997-86FA-8F05A1265DC8.log (SETMOD~1.LOG)
    Orphaned long file name part "SetMode_Func_0_0_6FA016C7-0428-4997-86FA-8F05A1265DC8.ekl"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/SetMode_Func_0_0_6FA016C7-0428-4997-86FA-8F05A1265DC8.ekl (SETMOD~1.EKL)
    Orphaned long file name part "SetMode_Func_1_0_6FA016C7-0428-4997-86FA-8F05A1265DC8.log"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/SetMode_Func_1_0_6FA016C7-0428-4997-86FA-8F05A1265DC8.log (SETMOD~1.LOG)
    Orphaned long file name part "SetMode_Func_1_0_6FA016C7-0428-4997-86FA-8F05A1265DC8.ekl"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/SetMode_Func_1_0_6FA016C7-0428-4997-86FA-8F05A1265DC8.ekl (SETMOD~1.EKL)
    Orphaned long file name part "TestString_Func_0_0_C6A4F228-E80A-42F9-B878-413F0F996C11.log"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/TestString_Func_0_0_C6A4F228-E80A-42F9-B878-413F0F996C11.log (TESTST~1.LOG)
    Orphaned long file name part "TestString_Func_0_0_C6A4F228-E80A-42F9-B878-413F0F996C11.ekl"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/TestString_Func_0_0_C6A4F228-E80A-42F9-B878-413F0F996C11.ekl (TESTST~1.EKL)
    Orphaned long file name part "TestString_Func_1_0_C6A4F228-E80A-42F9-B878-413F0F996C11.log"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/TestString_Func_1_0_C6A4F228-E80A-42F9-B878-413F0F996C11.log (TESTST~1.LOG)
    Orphaned long file name part "TestString_Func_1_0_C6A4F228-E80A-42F9-B878-413F0F996C11.ekl"
      Auto-deleting.
    Checking file /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/TestString_Func_1_0_C6A4F228-E80A-42F9-B878-413F0F996C11.ekl (TESTST~1.EKL)
    /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/ClearScreen_Func_0_0_D3533D69-75A9-46E0-9F50-A556232F4390.log
      Duplicate directory entry.
      First    Size 6120 bytes, date 01:00:00 Jan 01 1980
      Second   Size 6120 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.000
    /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/ClearScreen_Func_0_0_D3533D69-75A9-46E0-9F50-A556232F4390.ekl
      Duplicate directory entry.
      First    Size 4004 bytes, date 01:00:00 Jan 01 1980
      Second   Size 4004 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.001
    /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/EnableCursor_Func_0_0_4558978E-F938-424E-B3A4-48D4EFA522A5.log
      Duplicate directory entry.
      First    Size 9354 bytes, date 01:00:00 Jan 01 1980
      Second   Size 9354 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.002
    /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/EnableCursor_Func_0_0_4558978E-F938-424E-B3A4-48D4EFA522A5.ekl
      Duplicate directory entry.
      First    Size 7190 bytes, date 01:00:00 Jan 01 1980
      Second   Size 7190 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.003
    /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/OutputString_Func_0_0_A50A89D5-89C1-4214-8096-08C87910976F.log
      Duplicate directory entry.
      First    Size 8872 bytes, date 01:00:00 Jan 01 1980
      Second   Size 8872 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.004
    /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/OutputString_Func_0_0_A50A89D5-89C1-4214-8096-08C87910976F.ekl
      Duplicate directory entry.
      First    Size 6718 bytes, date 01:00:00 Jan 01 1980
      Second   Size 6718 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.005
    /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/QueryMode_Conf_0_0_64F2E0F9-87C6-4D4E-BB04-2D4E60FA29A5.log
      Duplicate directory entry.
      First    Size 9106 bytes, date 01:00:00 Jan 01 1980
      Second   Size 9106 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.006
    /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/QueryMode_Conf_0_0_64F2E0F9-87C6-4D4E-BB04-2D4E60FA29A5.log
      Duplicate directory entry.
      First    Size 9106 bytes, date 01:00:00 Jan 01 1980
      Second   Size 7190 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.007
    /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/QueryMode_Conf_0_0_64F2E0F9-87C6-4D4E-BB04-2D4E60FA29A5.log
      Duplicate directory entry.
      First    Size 9106 bytes, date 01:00:00 Jan 01 1980
      Second   Size 7190 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.008
    /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/QueryMode_Conf_0_0_64F2E0F9-87C6-4D4E-BB04-2D4E60FA29A5.ekl
      Duplicate directory entry.
      First    Size 6986 bytes, date 01:00:00 Jan 01 1980
      Second   Size 6986 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.009
    /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/QueryMode_Conf_0_0_64F2E0F9-87C6-4D4E-BB04-2D4E60FA29A5.ekl
      Duplicate directory entry.
      First    Size 6986 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5062 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.010
    /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/QueryMode_Conf_0_0_64F2E0F9-87C6-4D4E-BB04-2D4E60FA29A5.ekl
      Duplicate directory entry.
      First    Size 6986 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5062 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.011
    /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/Reset_Func_0_0_36BDBF05-2759-49CA-B128-BE19BE46EF6F.log
      Duplicate directory entry.
      First    Size 8800 bytes, date 01:00:00 Jan 01 1980
      Second   Size 8800 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.012
    /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/Reset_Func_0_0_36BDBF05-2759-49CA-B128-BE19BE46EF6F.ekl
      Duplicate directory entry.
      First    Size 6674 bytes, date 01:00:00 Jan 01 1980
      Second   Size 6674 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.013
    /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/SetAttribute_Func_0_0_07937289-8337-4B7B-ACE9-9182704FCBE8.log
      Duplicate directory entry.
      First    Size 4592 bytes, date 01:00:00 Jan 01 1980
      Second   Size 4592 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.014
    /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/SetAttribute_Func_0_0_07937289-8337-4B7B-ACE9-9182704FCBE8.ekl
      Duplicate directory entry.
      First    Size 2488 bytes, date 01:00:00 Jan 01 1980
      Second   Size 2488 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.015
    /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/SetCursorPosition_Conf_0_0_B07194F2-E025-42EB-B9E4-964A4FA64C8C.log
      Duplicate directory entry.
      First    Size 30214 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30214 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.016
    /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/SetCursorPosition_Conf_0_0_B07194F2-E025-42EB-B9E4-964A4FA64C8C.log
      Duplicate directory entry.
      First    Size 30214 bytes, date 01:00:00 Jan 01 1980
      Second   Size 4674 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.017
    /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/SetCursorPosition_Conf_0_0_B07194F2-E025-42EB-B9E4-964A4FA64C8C.log
      Duplicate directory entry.
      First    Size 30214 bytes, date 01:00:00 Jan 01 1980
      Second   Size 4674 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.018
    /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/SetCursorPosition_Conf_0_0_B07194F2-E025-42EB-B9E4-964A4FA64C8C.ekl
      Duplicate directory entry.
      First    Size 27946 bytes, date 01:00:00 Jan 01 1980
      Second   Size 27946 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.019
    /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/SetCursorPosition_Conf_0_0_B07194F2-E025-42EB-B9E4-964A4FA64C8C.ekl
      Duplicate directory entry.
      First    Size 27946 bytes, date 01:00:00 Jan 01 1980
      Second   Size 2530 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.020
    /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/SetCursorPosition_Conf_0_0_B07194F2-E025-42EB-B9E4-964A4FA64C8C.ekl
      Duplicate directory entry.
      First    Size 27946 bytes, date 01:00:00 Jan 01 1980
      Second   Size 2530 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.021
    /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/SetMode_Conf_0_0_37F5C015-E5A2-4089-A94B-CC9721A81C2D.log
      Duplicate directory entry.
      First    Size 20086 bytes, date 01:00:00 Jan 01 1980
      Second   Size 20086 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.022
    /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/SetMode_Conf_0_0_37F5C015-E5A2-4089-A94B-CC9721A81C2D.log
      Duplicate directory entry.
      First    Size 20086 bytes, date 01:00:00 Jan 01 1980
      Second   Size 6048 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.023
    /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/SetMode_Conf_0_0_37F5C015-E5A2-4089-A94B-CC9721A81C2D.log
      Duplicate directory entry.
      First    Size 20086 bytes, date 01:00:00 Jan 01 1980
      Second   Size 6048 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.024
    /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/SetMode_Conf_0_0_37F5C015-E5A2-4089-A94B-CC9721A81C2D.ekl
      Duplicate directory entry.
      First    Size 17842 bytes, date 01:00:00 Jan 01 1980
      Second   Size 17842 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.025
    /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/SetMode_Conf_0_0_37F5C015-E5A2-4089-A94B-CC9721A81C2D.ekl
      Duplicate directory entry.
      First    Size 17842 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3964 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.026
    /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/SetMode_Conf_0_0_37F5C015-E5A2-4089-A94B-CC9721A81C2D.ekl
      Duplicate directory entry.
      First    Size 17842 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3964 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.027
    /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/TestString_Func_0_0_C6A4F228-E80A-42F9-B878-413F0F996C11.log
      Duplicate directory entry.
      First    Size 4232 bytes, date 01:00:00 Jan 01 1980
      Second   Size 4232 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.028
    /Log/ConsoleSupportTest/SimpleOutputProtocolTest0/TestString_Func_0_0_C6A4F228-E80A-42F9-B878-413F0F996C11.ekl
      Duplicate directory entry.
      First    Size 2136 bytes, date 01:00:00 Jan 01 1980
      Second   Size 2136 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.029
    Checking file /Log/GenericTest/.
    Checking file /Log/GenericTest/..
    Checking file /Log/GenericTest/EFICompliantTest0 (EFICOM~1)
    Checking file /Log/GenericTest/EFICompliantTest0/.
    Checking file /Log/GenericTest/EFICompliantTest0/..
    Orphaned long file name part "PlatformSpecificElements_0_0_A0A8BED3-3D6F-4AD8-907A-84D52EE1543B.log"
      Auto-deleting.
    Checking file /Log/GenericTest/EFICompliantTest0/PlatformSpecificElements_0_0_A0A8BED3-3D6F-4AD8-907A-84D52EE1543B.log (PLATFO~1.LOG)
    Orphaned long file name part "PlatformSpecificElements_0_0_A0A8BED3-3D6F-4AD8-907A-84D52EE1543B.ekl"
      Auto-deleting.
    Checking file /Log/GenericTest/EFICompliantTest0/PlatformSpecificElements_0_0_A0A8BED3-3D6F-4AD8-907A-84D52EE1543B.ekl (PLATFO~1.EKL)
    Orphaned long file name part "RequiredElements_0_0_117C9ABC-489D-4504-ACDB-12AACE8F505B.log"
      Auto-deleting.
    Checking file /Log/GenericTest/EFICompliantTest0/RequiredElements_0_0_117C9ABC-489D-4504-ACDB-12AACE8F505B.log (REQUIR~1.LOG)
    Orphaned long file name part "RequiredElements_0_0_117C9ABC-489D-4504-ACDB-12AACE8F505B.ekl"
      Auto-deleting.
    Checking file /Log/GenericTest/EFICompliantTest0/RequiredElements_0_0_117C9ABC-489D-4504-ACDB-12AACE8F505B.ekl (REQUIR~1.EKL)
    Checking file /Log/MediaAccessTest/.
    Checking file /Log/MediaAccessTest/..
    Checking file /Log/MediaAccessTest/SimpleFileSystemProtocolTest0 (SIMPLE~1)
    Checking file /Log/MediaAccessTest/BlockIOProtocolTest0 (BLOCKI~1)
    Checking file /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/.
    Checking file /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/..
    Orphaned long file name part "Close_Func_0_0_3EAEA622-0167-4213-B6D9-0AD3D0066679.log"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/Close_Func_0_0_3EAEA622-0167-4213-B6D9-0AD3D0066679.log (CLOSE_~1.LOG)
    Orphaned long file name part "Close_Func_0_0_3EAEA622-0167-4213-B6D9-0AD3D0066679.ekl"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/Close_Func_0_0_3EAEA622-0167-4213-B6D9-0AD3D0066679.ekl (CLOSE_~1.EKL)
    Orphaned long file name part "Delete_Conf_0_0_77CFB820-D535-4A9C-B88B-6EF3DC217346.log"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/Delete_Conf_0_0_77CFB820-D535-4A9C-B88B-6EF3DC217346.log (DELETE~1.LOG)
    Orphaned long file name part "Delete_Conf_0_0_77CFB820-D535-4A9C-B88B-6EF3DC217346.ekl"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/Delete_Conf_0_0_77CFB820-D535-4A9C-B88B-6EF3DC217346.ekl (DELETE~1.EKL)
    Orphaned long file name part "Delete_Func_0_0_B709D88F-18F0-4DBA-A53C-7C4D81C496D8.log"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/Delete_Func_0_0_B709D88F-18F0-4DBA-A53C-7C4D81C496D8.log (DELETE~1.LOG)
    Orphaned long file name part "Delete_Func_0_0_B709D88F-18F0-4DBA-A53C-7C4D81C496D8.ekl"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/Delete_Func_0_0_B709D88F-18F0-4DBA-A53C-7C4D81C496D8.ekl (DELETE~1.EKL)
    Orphaned long file name part "FlushEx_Conf_0_0_B2EF8D8C-3662-462F-9011-CDDD5DC03C6B.log"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/FlushEx_Conf_0_0_B2EF8D8C-3662-462F-9011-CDDD5DC03C6B.log (FLUSHE~1.LOG)
    Orphaned long file name part "FlushEx_Conf_0_0_B2EF8D8C-3662-462F-9011-CDDD5DC03C6B.ekl"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/FlushEx_Conf_0_0_B2EF8D8C-3662-462F-9011-CDDD5DC03C6B.ekl (FLUSHE~1.EKL)
    Orphaned long file name part "FlushEx_Func_0_0_B2AF35D8-8E2B-48B1-A3FC-B4C67D80F99D.log"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/FlushEx_Func_0_0_B2AF35D8-8E2B-48B1-A3FC-B4C67D80F99D.log (FLUSHE~1.LOG)
    Orphaned long file name part "FlushEx_Func_0_0_B2AF35D8-8E2B-48B1-A3FC-B4C67D80F99D.ekl"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/FlushEx_Func_0_0_B2AF35D8-8E2B-48B1-A3FC-B4C67D80F99D.ekl (FLUSHE~1.EKL)
    Orphaned long file name part "Flush_Conf_0_0_41E00D7C-E0F7-455F-A617-FC6356182414.log"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/Flush_Conf_0_0_41E00D7C-E0F7-455F-A617-FC6356182414.log (FLUSH_~1.LOG)
    Orphaned long file name part "Flush_Conf_0_0_41E00D7C-E0F7-455F-A617-FC6356182414.ekl"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/Flush_Conf_0_0_41E00D7C-E0F7-455F-A617-FC6356182414.ekl (FLUSH_~1.EKL)
    Orphaned long file name part "Flush_Func_0_0_11F22AEB-5FA8-412A-A12A-E3D46015368C.log"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/Flush_Func_0_0_11F22AEB-5FA8-412A-A12A-E3D46015368C.log (FLUSH_~1.LOG)
    Orphaned long file name part "Flush_Func_0_0_11F22AEB-5FA8-412A-A12A-E3D46015368C.ekl"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/Flush_Func_0_0_11F22AEB-5FA8-412A-A12A-E3D46015368C.ekl (FLUSH_~1.EKL)
    Orphaned long file name part "GetInfo_Conf_0_0_8B16C09D-5321-4A63-B168-8E59590A436D.log"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/GetInfo_Conf_0_0_8B16C09D-5321-4A63-B168-8E59590A436D.log (GETINF~1.LOG)
    Orphaned long file name part "GetInfo_Conf_0_0_8B16C09D-5321-4A63-B168-8E59590A436D.ekl"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/GetInfo_Conf_0_0_8B16C09D-5321-4A63-B168-8E59590A436D.ekl (GETINF~1.EKL)
    Orphaned long file name part "GetInfo_Func_0_0_EE14A4DB-BC9F-49EB-8C72-4BC655427D97.log"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/GetInfo_Func_0_0_EE14A4DB-BC9F-49EB-8C72-4BC655427D97.log (GETINF~1.LOG)
    Orphaned long file name part "GetInfo_Func_0_0_EE14A4DB-BC9F-49EB-8C72-4BC655427D97.ekl"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/GetInfo_Func_0_0_EE14A4DB-BC9F-49EB-8C72-4BC655427D97.ekl (GETINF~1.EKL)
    Orphaned long file name part "GetPosition_Conf_0_0_8A2F13C7-A01C-4949-81C9-46B3FF349F92.log"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/GetPosition_Conf_0_0_8A2F13C7-A01C-4949-81C9-46B3FF349F92.log (GETPOS~1.LOG)
    Orphaned long file name part "GetPosition_Conf_0_0_8A2F13C7-A01C-4949-81C9-46B3FF349F92.ekl"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/GetPosition_Conf_0_0_8A2F13C7-A01C-4949-81C9-46B3FF349F92.ekl (GETPOS~1.EKL)
    Orphaned long file name part "GetPosition_Func_0_0_38150EBD-8835-46C5-B085-6A6C626EA972.log"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/GetPosition_Func_0_0_38150EBD-8835-46C5-B085-6A6C626EA972.log (GETPOS~1.LOG)
    Orphaned long file name part "GetPosition_Func_0_0_38150EBD-8835-46C5-B085-6A6C626EA972.ekl"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/GetPosition_Func_0_0_38150EBD-8835-46C5-B085-6A6C626EA972.ekl (GETPOS~1.EKL)
    Orphaned long file name part "OpenEx_Conf_0_0_614CF090-E3A6-49B6-AF93-31BABA0761B4.log"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/OpenEx_Conf_0_0_614CF090-E3A6-49B6-AF93-31BABA0761B4.log (OPENEX~1.LOG)
    Orphaned long file name part "OpenEx_Conf_0_0_614CF090-E3A6-49B6-AF93-31BABA0761B4.ekl"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/OpenEx_Conf_0_0_614CF090-E3A6-49B6-AF93-31BABA0761B4.ekl (OPENEX~1.EKL)
    Orphaned long file name part "OpenEx_Func_0_0_7E68498E-343B-4B61-8E3F-FAE285D919F5.log"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/OpenEx_Func_0_0_7E68498E-343B-4B61-8E3F-FAE285D919F5.log (OPENEX~1.LOG)
    Orphaned long file name part "OpenEx_Func_0_0_7E68498E-343B-4B61-8E3F-FAE285D919F5.ekl"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/OpenEx_Func_0_0_7E68498E-343B-4B61-8E3F-FAE285D919F5.ekl (OPENEX~1.EKL)
    Orphaned long file name part "OpenVolume_Func_0_0_3E59FED4-426A-4E00-8787-68A20F80B0B7.log"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/OpenVolume_Func_0_0_3E59FED4-426A-4E00-8787-68A20F80B0B7.log (OPENVO~1.LOG)
    Orphaned long file name part "OpenVolume_Func_0_0_3E59FED4-426A-4E00-8787-68A20F80B0B7.ekl"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/OpenVolume_Func_0_0_3E59FED4-426A-4E00-8787-68A20F80B0B7.ekl (OPENVO~1.EKL)
    Orphaned long file name part "Open_Conf_0_0_0BA666CB-B43A-4691-82E8-B2241EB9A9F9.log"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/Open_Conf_0_0_0BA666CB-B43A-4691-82E8-B2241EB9A9F9.log (OPEN_C~1.LOG)
    Orphaned long file name part "Open_Conf_0_0_0BA666CB-B43A-4691-82E8-B2241EB9A9F9.ekl"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/Open_Conf_0_0_0BA666CB-B43A-4691-82E8-B2241EB9A9F9.ekl (OPEN_C~1.EKL)
    Orphaned long file name part "Open_Func_0_0_A6B309B3-A0AD-409D-A500-FF343E490740.log"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/Open_Func_0_0_A6B309B3-A0AD-409D-A500-FF343E490740.log (OPEN_F~1.LOG)
    Orphaned long file name part "Open_Func_0_0_A6B309B3-A0AD-409D-A500-FF343E490740.ekl"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/Open_Func_0_0_A6B309B3-A0AD-409D-A500-FF343E490740.ekl (OPEN_F~1.EKL)
    Orphaned long file name part "ReadEx_Conf_0_0_B877944F-7D05-427F-BB9C-BCCF78073488.log"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/ReadEx_Conf_0_0_B877944F-7D05-427F-BB9C-BCCF78073488.log (READEX~1.LOG)
    Orphaned long file name part "ReadEx_Conf_0_0_B877944F-7D05-427F-BB9C-BCCF78073488.ekl"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/ReadEx_Conf_0_0_B877944F-7D05-427F-BB9C-BCCF78073488.ekl (READEX~1.EKL)
    Orphaned long file name part "ReadEx_Func_0_0_C54B642D-4D3E-4897-9DD5-1F722165E00E.log"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/ReadEx_Func_0_0_C54B642D-4D3E-4897-9DD5-1F722165E00E.log (READEX~1.LOG)
    Orphaned long file name part "ReadEx_Func_0_0_C54B642D-4D3E-4897-9DD5-1F722165E00E.ekl"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/ReadEx_Func_0_0_C54B642D-4D3E-4897-9DD5-1F722165E00E.ekl (READEX~1.EKL)
    Orphaned long file name part "Read_Func_0_0_2582C031-21E7-4A7B-AF80-8A67B3E1D7D8.log"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/Read_Func_0_0_2582C031-21E7-4A7B-AF80-8A67B3E1D7D8.log (READ_F~1.LOG)
    Orphaned long file name part "Read_Func_0_0_2582C031-21E7-4A7B-AF80-8A67B3E1D7D8.ekl"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/Read_Func_0_0_2582C031-21E7-4A7B-AF80-8A67B3E1D7D8.ekl (READ_F~1.EKL)
    Orphaned long file name part "SetInfo_Conf_0_0_44BEC963-DABD-43E1-B38A-955ABA3B18FF.log"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/SetInfo_Conf_0_0_44BEC963-DABD-43E1-B38A-955ABA3B18FF.log (SETINF~1.LOG)
    Orphaned long file name part "SetInfo_Conf_0_0_44BEC963-DABD-43E1-B38A-955ABA3B18FF.ekl"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/SetInfo_Conf_0_0_44BEC963-DABD-43E1-B38A-955ABA3B18FF.ekl (SETINF~1.EKL)
    Orphaned long file name part "SetInfo_Func_0_0_EBA448E7-59E6-474A-875E-56DDEE9E3BFE.log"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/SetInfo_Func_0_0_EBA448E7-59E6-474A-875E-56DDEE9E3BFE.log (SETINF~1.LOG)
    Orphaned long file name part "SetInfo_Func_0_0_EBA448E7-59E6-474A-875E-56DDEE9E3BFE.ekl"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/SetInfo_Func_0_0_EBA448E7-59E6-474A-875E-56DDEE9E3BFE.ekl (SETINF~1.EKL)
    Orphaned long file name part "SetPosition_Conf_0_0_A2FDC63E-2D01-4AAB-8880-E62C1E08D930.log"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/SetPosition_Conf_0_0_A2FDC63E-2D01-4AAB-8880-E62C1E08D930.log (SETPOS~1.LOG)
    Orphaned long file name part "SetPosition_Conf_0_0_A2FDC63E-2D01-4AAB-8880-E62C1E08D930.ekl"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/SetPosition_Conf_0_0_A2FDC63E-2D01-4AAB-8880-E62C1E08D930.ekl (SETPOS~1.EKL)
    Orphaned long file name part "SetPosition_Func_0_0_4867091F-5988-4A0C-9F21-440755479A1B.log"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/SetPosition_Func_0_0_4867091F-5988-4A0C-9F21-440755479A1B.log (SETPOS~1.LOG)
    Orphaned long file name part "SetPosition_Func_0_0_4867091F-5988-4A0C-9F21-440755479A1B.ekl"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/SetPosition_Func_0_0_4867091F-5988-4A0C-9F21-440755479A1B.ekl (SETPOS~1.EKL)
    Orphaned long file name part "WriteEx_Conf_0_0_BFFE42D6-CE26-4B63-8609-51E69A1668A1.log"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/WriteEx_Conf_0_0_BFFE42D6-CE26-4B63-8609-51E69A1668A1.log (WRITEE~1.LOG)
    Orphaned long file name part "WriteEx_Conf_0_0_BFFE42D6-CE26-4B63-8609-51E69A1668A1.ekl"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/WriteEx_Conf_0_0_BFFE42D6-CE26-4B63-8609-51E69A1668A1.ekl (WRITEE~1.EKL)
    Orphaned long file name part "WriteEx_Func_0_0_44B63E71-6A74-4A23-9C2D-ED333DD5DDE2.log"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/WriteEx_Func_0_0_44B63E71-6A74-4A23-9C2D-ED333DD5DDE2.log (WRITEE~1.LOG)
    Orphaned long file name part "WriteEx_Func_0_0_44B63E71-6A74-4A23-9C2D-ED333DD5DDE2.ekl"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/WriteEx_Func_0_0_44B63E71-6A74-4A23-9C2D-ED333DD5DDE2.ekl (WRITEE~1.EKL)
    Orphaned long file name part "Write_Conf_0_0_AEC76679-3A6E-4347-BBE4-FC9BBC3FDD5C.log"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/Write_Conf_0_0_AEC76679-3A6E-4347-BBE4-FC9BBC3FDD5C.log (WRITE_~1.LOG)
    Orphaned long file name part "Write_Conf_0_0_AEC76679-3A6E-4347-BBE4-FC9BBC3FDD5C.ekl"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/Write_Conf_0_0_AEC76679-3A6E-4347-BBE4-FC9BBC3FDD5C.ekl (WRITE_~1.EKL)
    Orphaned long file name part "Write_Func_0_0_22372DD8-AA00-4EDA-99E8-6FC14AB1FB3C.log"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/Write_Func_0_0_22372DD8-AA00-4EDA-99E8-6FC14AB1FB3C.log (WRITE_~1.LOG)
    Orphaned long file name part "Write_Func_0_0_22372DD8-AA00-4EDA-99E8-6FC14AB1FB3C.ekl"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/Write_Func_0_0_22372DD8-AA00-4EDA-99E8-6FC14AB1FB3C.ekl (WRITE_~1.EKL)
    /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/Delete_Conf_0_0_77CFB820-D535-4A9C-B88B-6EF3DC217346.log
      Duplicate directory entry.
      First    Size 3622 bytes, date 01:00:00 Jan 01 1980
      Second   Size 8384 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.000
    /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/Delete_Conf_0_0_77CFB820-D535-4A9C-B88B-6EF3DC217346.ekl
      Duplicate directory entry.
      First    Size 1958 bytes, date 01:00:00 Jan 01 1980
      Second   Size 6580 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.001
    /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/FlushEx_Conf_0_0_B2EF8D8C-3662-462F-9011-CDDD5DC03C6B.log
      Duplicate directory entry.
      First    Size 3758 bytes, date 01:00:00 Jan 01 1980
      Second   Size 6848 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.002
    /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/FlushEx_Conf_0_0_B2EF8D8C-3662-462F-9011-CDDD5DC03C6B.ekl
      Duplicate directory entry.
      First    Size 1942 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5120 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.003
    /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/Flush_Conf_0_0_41E00D7C-E0F7-455F-A617-FC6356182414.log
      Duplicate directory entry.
      First    Size 3050 bytes, date 01:00:00 Jan 01 1980
      Second   Size 4462 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.004
    /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/Flush_Conf_0_0_41E00D7C-E0F7-455F-A617-FC6356182414.ekl
      Duplicate directory entry.
      First    Size 1404 bytes, date 01:00:00 Jan 01 1980
      Second   Size 2788 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.005
    /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/GetInfo_Conf_0_0_8B16C09D-5321-4A63-B168-8E59590A436D.log
      Duplicate directory entry.
      First    Size 5124 bytes, date 01:00:00 Jan 01 1980
      Second   Size 10628 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.006
    /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/GetInfo_Conf_0_0_8B16C09D-5321-4A63-B168-8E59590A436D.ekl
      Duplicate directory entry.
      First    Size 3422 bytes, date 01:00:00 Jan 01 1980
      Second   Size 8324 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.007
    /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/GetPosition_Conf_0_0_8A2F13C7-A01C-4949-81C9-46B3FF349F92.log
      Duplicate directory entry.
      First    Size 3124 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5536 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.008
    /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/GetPosition_Conf_0_0_8A2F13C7-A01C-4949-81C9-46B3FF349F92.ekl
      Duplicate directory entry.
      First    Size 1432 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3638 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.009
    /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/OpenEx_Conf_0_0_614CF090-E3A6-49B6-AF93-31BABA0761B4.log
      Duplicate directory entry.
      First    Size 13170 bytes, date 01:00:00 Jan 01 1980
      Second   Size 33350 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.010
    /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/OpenEx_Conf_0_0_614CF090-E3A6-49B6-AF93-31BABA0761B4.ekl
      Duplicate directory entry.
      First    Size 11164 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30736 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.011
    /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/ReadEx_Conf_0_0_B877944F-7D05-427F-BB9C-BCCF78073488.log
      Duplicate directory entry.
      First    Size 4316 bytes, date 01:00:00 Jan 01 1980
      Second   Size 48344 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.012
    /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/ReadEx_Conf_0_0_B877944F-7D05-427F-BB9C-BCCF78073488.ekl
      Duplicate directory entry.
      First    Size 2604 bytes, date 01:00:00 Jan 01 1980
      Second   Size 45824 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.013
    /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/SetInfo_Conf_0_0_44BEC963-DABD-43E1-B38A-955ABA3B18FF.log
      Duplicate directory entry.
      First    Size 10376 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5516 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.014
    /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/SetInfo_Conf_0_0_44BEC963-DABD-43E1-B38A-955ABA3B18FF.ekl
      Duplicate directory entry.
      First    Size 8580 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3812 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.015
    /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/SetPosition_Conf_0_0_A2FDC63E-2D01-4AAB-8880-E62C1E08D930.log
      Duplicate directory entry.
      First    Size 3124 bytes, date 01:00:00 Jan 01 1980
      Second   Size 5040 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.016
    /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/SetPosition_Conf_0_0_A2FDC63E-2D01-4AAB-8880-E62C1E08D930.ekl
      Duplicate directory entry.
      First    Size 1432 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3312 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.017
    /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/WriteEx_Conf_0_0_BFFE42D6-CE26-4B63-8609-51E69A1668A1.log
      Duplicate directory entry.
      First    Size 5364 bytes, date 01:00:00 Jan 01 1980
      Second   Size 4566 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.018
    /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/WriteEx_Conf_0_0_BFFE42D6-CE26-4B63-8609-51E69A1668A1.ekl
      Duplicate directory entry.
      First    Size 3624 bytes, date 01:00:00 Jan 01 1980
      Second   Size 2720 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.019
    /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/Write_Conf_0_0_AEC76679-3A6E-4347-BBE4-FC9BBC3FDD5C.log
      Duplicate directory entry.
      First    Size 3570 bytes, date 01:00:00 Jan 01 1980
      Second   Size 2998 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.020
    /Log/MediaAccessTest/SimpleFileSystemProtocolTest0/Write_Conf_0_0_AEC76679-3A6E-4347-BBE4-FC9BBC3FDD5C.ekl
      Duplicate directory entry.
      First    Size 1826 bytes, date 01:00:00 Jan 01 1980
      Second   Size 1108 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.021
    Checking file /Log/MediaAccessTest/BlockIOProtocolTest0/.
    Checking file /Log/MediaAccessTest/BlockIOProtocolTest0/..
    Orphaned long file name part "FlushBlocks_Conf_0_0_759C5229-272A-45AA-A616-B5622619EB06.log"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/BlockIOProtocolTest0/FlushBlocks_Conf_0_0_759C5229-272A-45AA-A616-B5622619EB06.log (FLUSHB~1.LOG)
    Orphaned long file name part "FlushBlocks_Conf_0_0_759C5229-272A-45AA-A616-B5622619EB06.ekl"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/BlockIOProtocolTest0/FlushBlocks_Conf_0_0_759C5229-272A-45AA-A616-B5622619EB06.ekl (FLUSHB~1.EKL)
    Orphaned long file name part "FlushBlocks_Conf_1_0_759C5229-272A-45AA-A616-B5622619EB06.log"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/BlockIOProtocolTest0/FlushBlocks_Conf_1_0_759C5229-272A-45AA-A616-B5622619EB06.log (FLUSHB~1.LOG)
    Orphaned long file name part "FlushBlocks_Conf_1_0_759C5229-272A-45AA-A616-B5622619EB06.ekl"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/BlockIOProtocolTest0/FlushBlocks_Conf_1_0_759C5229-272A-45AA-A616-B5622619EB06.ekl (FLUSHB~1.EKL)
    Orphaned long file name part "FlushBlocks_Func_0_0_7C947313-C8A3-4ABD-A1F2-8670EE574BE5.log"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/BlockIOProtocolTest0/FlushBlocks_Func_0_0_7C947313-C8A3-4ABD-A1F2-8670EE574BE5.log (FLUSHB~1.LOG)
    Orphaned long file name part "FlushBlocks_Func_0_0_7C947313-C8A3-4ABD-A1F2-8670EE574BE5.ekl"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/BlockIOProtocolTest0/FlushBlocks_Func_0_0_7C947313-C8A3-4ABD-A1F2-8670EE574BE5.ekl (FLUSHB~1.EKL)
    Orphaned long file name part "FlushBlocks_Func_1_0_7C947313-C8A3-4ABD-A1F2-8670EE574BE5.log"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/BlockIOProtocolTest0/FlushBlocks_Func_1_0_7C947313-C8A3-4ABD-A1F2-8670EE574BE5.log (FLUSHB~1.LOG)
    Orphaned long file name part "FlushBlocks_Func_1_0_7C947313-C8A3-4ABD-A1F2-8670EE574BE5.ekl"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/BlockIOProtocolTest0/FlushBlocks_Func_1_0_7C947313-C8A3-4ABD-A1F2-8670EE574BE5.ekl (FLUSHB~1.EKL)
    Orphaned long file name part "MediaInfo_Integrity_0_0_EABBFA97-314D-49D2-9019-0DFF5212062F.log"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/BlockIOProtocolTest0/MediaInfo_Integrity_0_0_EABBFA97-314D-49D2-9019-0DFF5212062F.log (MEDIAI~1.LOG)
    Orphaned long file name part "MediaInfo_Integrity_0_0_EABBFA97-314D-49D2-9019-0DFF5212062F.ekl"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/BlockIOProtocolTest0/MediaInfo_Integrity_0_0_EABBFA97-314D-49D2-9019-0DFF5212062F.ekl (MEDIAI~1.EKL)
    Orphaned long file name part "MediaInfo_Integrity_1_0_EABBFA97-314D-49D2-9019-0DFF5212062F.log"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/BlockIOProtocolTest0/MediaInfo_Integrity_1_0_EABBFA97-314D-49D2-9019-0DFF5212062F.log (MEDIAI~1.LOG)
    Orphaned long file name part "MediaInfo_Integrity_1_0_EABBFA97-314D-49D2-9019-0DFF5212062F.ekl"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/BlockIOProtocolTest0/MediaInfo_Integrity_1_0_EABBFA97-314D-49D2-9019-0DFF5212062F.ekl (MEDIAI~1.EKL)
    Orphaned long file name part "ReadBlocks_Conf_0_0_826159D3-04A5-4CCE-8431-344707A8B57A.log"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/BlockIOProtocolTest0/ReadBlocks_Conf_0_0_826159D3-04A5-4CCE-8431-344707A8B57A.log (READBL~1.LOG)
    Orphaned long file name part "ReadBlocks_Conf_0_0_826159D3-04A5-4CCE-8431-344707A8B57A.ekl"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/BlockIOProtocolTest0/ReadBlocks_Conf_0_0_826159D3-04A5-4CCE-8431-344707A8B57A.ekl (READBL~1.EKL)
    Orphaned long file name part "ReadBlocks_Conf_1_0_826159D3-04A5-4CCE-8431-344707A8B57A.log"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/BlockIOProtocolTest0/ReadBlocks_Conf_1_0_826159D3-04A5-4CCE-8431-344707A8B57A.log (READBL~1.LOG)
    Orphaned long file name part "ReadBlocks_Conf_1_0_826159D3-04A5-4CCE-8431-344707A8B57A.ekl"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/BlockIOProtocolTest0/ReadBlocks_Conf_1_0_826159D3-04A5-4CCE-8431-344707A8B57A.ekl (READBL~1.EKL)
    Orphaned long file name part "ReadBlocks_Func_0_0_A4284AE9-C988-4230-973A-5C19398C8254.log"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/BlockIOProtocolTest0/ReadBlocks_Func_0_0_A4284AE9-C988-4230-973A-5C19398C8254.log (READBL~1.LOG)
    Orphaned long file name part "ReadBlocks_Func_0_0_A4284AE9-C988-4230-973A-5C19398C8254.ekl"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/BlockIOProtocolTest0/ReadBlocks_Func_0_0_A4284AE9-C988-4230-973A-5C19398C8254.ekl (READBL~1.EKL)
    Orphaned long file name part "ReadBlocks_Func_1_0_A4284AE9-C988-4230-973A-5C19398C8254.log"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/BlockIOProtocolTest0/ReadBlocks_Func_1_0_A4284AE9-C988-4230-973A-5C19398C8254.log (READBL~1.LOG)
    Orphaned long file name part "ReadBlocks_Func_1_0_A4284AE9-C988-4230-973A-5C19398C8254.ekl"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/BlockIOProtocolTest0/ReadBlocks_Func_1_0_A4284AE9-C988-4230-973A-5C19398C8254.ekl (READBL~1.EKL)
    Orphaned long file name part "Reset_Func_0_0_B0501C52-1564-4945-B57B-1FD2C882FF91.log"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/BlockIOProtocolTest0/Reset_Func_0_0_B0501C52-1564-4945-B57B-1FD2C882FF91.log (RESET_~1.LOG)
    Orphaned long file name part "Reset_Func_0_0_B0501C52-1564-4945-B57B-1FD2C882FF91.ekl"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/BlockIOProtocolTest0/Reset_Func_0_0_B0501C52-1564-4945-B57B-1FD2C882FF91.ekl (RESET_~1.EKL)
    Orphaned long file name part "Reset_Func_1_0_B0501C52-1564-4945-B57B-1FD2C882FF91.log"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/BlockIOProtocolTest0/Reset_Func_1_0_B0501C52-1564-4945-B57B-1FD2C882FF91.log (RESET_~1.LOG)
    Orphaned long file name part "Reset_Func_1_0_B0501C52-1564-4945-B57B-1FD2C882FF91.ekl"
      Auto-deleting.
    Checking file /Log/MediaAccessTest/BlockIOProtocolTest0/Reset_Func_1_0_B0501C52-1564-4945-B57B-1FD2C882FF91.ekl (RESET_~1.EKL)
    /Log/MediaAccessTest/BlockIOProtocolTest0/FlushBlocks_Conf_0_0_759C5229-272A-45AA-A616-B5622619EB06.log
      Duplicate directory entry.
      First    Size 2650 bytes, date 01:00:00 Jan 01 1980
      Second   Size 2650 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.000
    /Log/MediaAccessTest/BlockIOProtocolTest0/FlushBlocks_Conf_0_0_759C5229-272A-45AA-A616-B5622619EB06.log
      Duplicate directory entry.
      First    Size 2650 bytes, date 01:00:00 Jan 01 1980
      Second   Size 2664 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.001
    /Log/MediaAccessTest/BlockIOProtocolTest0/FlushBlocks_Conf_0_0_759C5229-272A-45AA-A616-B5622619EB06.log
      Duplicate directory entry.
      First    Size 2650 bytes, date 01:00:00 Jan 01 1980
      Second   Size 2664 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.002
    /Log/MediaAccessTest/BlockIOProtocolTest0/FlushBlocks_Conf_0_0_759C5229-272A-45AA-A616-B5622619EB06.ekl
      Duplicate directory entry.
      First    Size 542 bytes, date 01:00:00 Jan 01 1980
      Second   Size 586 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.003
    /Log/MediaAccessTest/BlockIOProtocolTest0/FlushBlocks_Conf_0_0_759C5229-272A-45AA-A616-B5622619EB06.ekl
      Duplicate directory entry.
      First    Size 542 bytes, date 01:00:00 Jan 01 1980
      Second   Size 542 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.004
    /Log/MediaAccessTest/BlockIOProtocolTest0/FlushBlocks_Conf_0_0_759C5229-272A-45AA-A616-B5622619EB06.ekl
      Duplicate directory entry.
      First    Size 542 bytes, date 01:00:00 Jan 01 1980
      Second   Size 586 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.005
    /Log/MediaAccessTest/BlockIOProtocolTest0/MediaInfo_Integrity_0_0_EABBFA97-314D-49D2-9019-0DFF5212062F.log
      Duplicate directory entry.
      First    Size 2654 bytes, date 01:00:00 Jan 01 1980
      Second   Size 2654 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.006
    /Log/MediaAccessTest/BlockIOProtocolTest0/MediaInfo_Integrity_0_0_EABBFA97-314D-49D2-9019-0DFF5212062F.ekl
      Duplicate directory entry.
      First    Size 548 bytes, date 01:00:00 Jan 01 1980
      Second   Size 592 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.007
    /Log/MediaAccessTest/BlockIOProtocolTest0/ReadBlocks_Conf_0_0_826159D3-04A5-4CCE-8431-344707A8B57A.log
      Duplicate directory entry.
      First    Size 19010 bytes, date 01:00:00 Jan 01 1980
      Second   Size 19054 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.008
    /Log/MediaAccessTest/BlockIOProtocolTest0/ReadBlocks_Conf_0_0_826159D3-04A5-4CCE-8431-344707A8B57A.log
      Duplicate directory entry.
      First    Size 19010 bytes, date 01:00:00 Jan 01 1980
      Second   Size 30988 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.009
    /Log/MediaAccessTest/BlockIOProtocolTest0/ReadBlocks_Conf_0_0_826159D3-04A5-4CCE-8431-344707A8B57A.log
      Duplicate directory entry.
      First    Size 19010 bytes, date 01:00:00 Jan 01 1980
      Second   Size 31032 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.010
    /Log/MediaAccessTest/BlockIOProtocolTest0/ReadBlocks_Conf_0_0_826159D3-04A5-4CCE-8431-344707A8B57A.ekl
      Duplicate directory entry.
      First    Size 16690 bytes, date 01:00:00 Jan 01 1980
      Second   Size 16734 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.011
    /Log/MediaAccessTest/BlockIOProtocolTest0/ReadBlocks_Conf_0_0_826159D3-04A5-4CCE-8431-344707A8B57A.ekl
      Duplicate directory entry.
      First    Size 16690 bytes, date 01:00:00 Jan 01 1980
      Second   Size 28414 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.012
    /Log/MediaAccessTest/BlockIOProtocolTest0/ReadBlocks_Conf_0_0_826159D3-04A5-4CCE-8431-344707A8B57A.ekl
      Duplicate directory entry.
      First    Size 16690 bytes, date 01:00:00 Jan 01 1980
      Second   Size 28458 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.013
    /Log/MediaAccessTest/BlockIOProtocolTest0/Reset_Func_0_0_B0501C52-1564-4945-B57B-1FD2C882FF91.log
      Duplicate directory entry.
      First    Size 3640 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3640 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.014
    /Log/MediaAccessTest/BlockIOProtocolTest0/Reset_Func_0_0_B0501C52-1564-4945-B57B-1FD2C882FF91.ekl
      Duplicate directory entry.
      First    Size 1722 bytes, date 01:00:00 Jan 01 1980
      Second   Size 1766 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.015
    Checking file /Log/HIITest/.
    Checking file /Log/HIITest/..
    Checking file /Log/HIITest/HIIDatabaseProtocolTest0 (HIIDAT~1)
    Checking file /Log/HIITest/HIIStringProtocolTest0 (HIISTR~1)
    Checking file /Log/HIITest/HIIDatabaseProtocolTest0/.
    Checking file /Log/HIITest/HIIDatabaseProtocolTest0/..
    Orphaned long file name part "ExportPackageListsConformance_0_0_B6DCE569-0A0E-4FCE-9EE0-868730F50C4D.log"
      Auto-deleting.
    Checking file /Log/HIITest/HIIDatabaseProtocolTest0/ExportPackageListsConformance_0_0_B6DCE569-0A0E-4FCE-9EE0-868730F50C4D.log (EXPORT~1.LOG)
    Orphaned long file name part "ExportPackageListsConformance_0_0_B6DCE569-0A0E-4FCE-9EE0-868730F50C4D.ekl"
      Auto-deleting.
    Checking file /Log/HIITest/HIIDatabaseProtocolTest0/ExportPackageListsConformance_0_0_B6DCE569-0A0E-4FCE-9EE0-868730F50C4D.ekl (EXPORT~1.EKL)
    Orphaned long file name part "ExportPackageListsFunction_0_0_0F8BA647-1F74-4D62-AB91-F1526B507DA6.log"
      Auto-deleting.
    Checking file /Log/HIITest/HIIDatabaseProtocolTest0/ExportPackageListsFunction_0_0_0F8BA647-1F74-4D62-AB91-F1526B507DA6.log (EXPORT~1.LOG)
    Orphaned long file name part "ExportPackageListsFunction_0_0_0F8BA647-1F74-4D62-AB91-F1526B507DA6.ekl"
      Auto-deleting.
    Checking file /Log/HIITest/HIIDatabaseProtocolTest0/ExportPackageListsFunction_0_0_0F8BA647-1F74-4D62-AB91-F1526B507DA6.ekl (EXPORT~1.EKL)
    Orphaned long file name part "FindKeyboardLayoutsConformance_0_0_3952E6C7-3B3C-4B24-9320-E2C53CC55025.log"
      Auto-deleting.
    Checking file /Log/HIITest/HIIDatabaseProtocolTest0/FindKeyboardLayoutsConformance_0_0_3952E6C7-3B3C-4B24-9320-E2C53CC55025.log (FINDKE~1.LOG)
    Orphaned long file name part "FindKeyboardLayoutsConformance_0_0_3952E6C7-3B3C-4B24-9320-E2C53CC55025.ekl"
      Auto-deleting.
    Checking file /Log/HIITest/HIIDatabaseProtocolTest0/FindKeyboardLayoutsConformance_0_0_3952E6C7-3B3C-4B24-9320-E2C53CC55025.ekl (FINDKE~1.EKL)
    Orphaned long file name part "FindKeyboardLayoutsFunction_0_0_11D5958C-BBE7-4851-A05C-E0059A0A8D3A.log"
      Auto-deleting.
    Checking file /Log/HIITest/HIIDatabaseProtocolTest0/FindKeyboardLayoutsFunction_0_0_11D5958C-BBE7-4851-A05C-E0059A0A8D3A.log (FINDKE~1.LOG)
    Orphaned long file name part "FindKeyboardLayoutsFunction_0_0_11D5958C-BBE7-4851-A05C-E0059A0A8D3A.ekl"
      Auto-deleting.
    Checking file /Log/HIITest/HIIDatabaseProtocolTest0/FindKeyboardLayoutsFunction_0_0_11D5958C-BBE7-4851-A05C-E0059A0A8D3A.ekl (FINDKE~1.EKL)
    Orphaned long file name part "GetKeyboardLayoutConformance_0_0_E8683EEB-56A0-401C-89C8-D8BA672F40F0.log"
      Auto-deleting.
    Checking file /Log/HIITest/HIIDatabaseProtocolTest0/GetKeyboardLayoutConformance_0_0_E8683EEB-56A0-401C-89C8-D8BA672F40F0.log (GETKEY~1.LOG)
    Orphaned long file name part "GetKeyboardLayoutConformance_0_0_E8683EEB-56A0-401C-89C8-D8BA672F40F0.ekl"
      Auto-deleting.
    Checking file /Log/HIITest/HIIDatabaseProtocolTest0/GetKeyboardLayoutConformance_0_0_E8683EEB-56A0-401C-89C8-D8BA672F40F0.ekl (GETKEY~1.EKL)
    Orphaned long file name part "GetKeyboardLayoutFunction_0_0_73332B8C-AF68-4E12-913D-5D89E8FB8925.log"
      Auto-deleting.
    Checking file /Log/HIITest/HIIDatabaseProtocolTest0/GetKeyboardLayoutFunction_0_0_73332B8C-AF68-4E12-913D-5D89E8FB8925.log (GETKEY~1.LOG)
    Orphaned long file name part "GetKeyboardLayoutFunction_0_0_73332B8C-AF68-4E12-913D-5D89E8FB8925.ekl"
      Auto-deleting.
    Checking file /Log/HIITest/HIIDatabaseProtocolTest0/GetKeyboardLayoutFunction_0_0_73332B8C-AF68-4E12-913D-5D89E8FB8925.ekl (GETKEY~1.EKL)
    Orphaned long file name part "GetPackageListHandleConformance_0_0_D51EBDA6-391B-49BC-A4CB-0EAF1A0E3A05.log"
      Auto-deleting.
    Checking file /Log/HIITest/HIIDatabaseProtocolTest0/GetPackageListHandleConformance_0_0_D51EBDA6-391B-49BC-A4CB-0EAF1A0E3A05.log (GETPAC~1.LOG)
    Orphaned long file name part "GetPackageListHandleConformance_0_0_D51EBDA6-391B-49BC-A4CB-0EAF1A0E3A05.ekl"
      Auto-deleting.
    Checking file /Log/HIITest/HIIDatabaseProtocolTest0/GetPackageListHandleConformance_0_0_D51EBDA6-391B-49BC-A4CB-0EAF1A0E3A05.ekl (GETPAC~1.EKL)
    Orphaned long file name part "GetPackageListHandleFunction_0_0_B54B29F4-B2A5-49E8-BCA6-F6929733DD11.log"
      Auto-deleting.
    Checking file /Log/HIITest/HIIDatabaseProtocolTest0/GetPackageListHandleFunction_0_0_B54B29F4-B2A5-49E8-BCA6-F6929733DD11.log (GETPAC~1.LOG)
    Orphaned long file name part "GetPackageListHandleFunction_0_0_B54B29F4-B2A5-49E8-BCA6-F6929733DD11.ekl"
      Auto-deleting.
    Checking file /Log/HIITest/HIIDatabaseProtocolTest0/GetPackageListHandleFunction_0_0_B54B29F4-B2A5-49E8-BCA6-F6929733DD11.ekl (GETPAC~1.EKL)
    Orphaned long file name part "ListPackageListsConformance_0_0_3DF6360E-AB9A-4CB6-BC43-1CDBC8FF50E9.log"
      Auto-deleting.
    Checking file /Log/HIITest/HIIDatabaseProtocolTest0/ListPackageListsConformance_0_0_3DF6360E-AB9A-4CB6-BC43-1CDBC8FF50E9.log (LISTPA~1.LOG)
    Orphaned long file name part "ListPackageListsConformance_0_0_3DF6360E-AB9A-4CB6-BC43-1CDBC8FF50E9.ekl"
      Auto-deleting.
    Checking file /Log/HIITest/HIIDatabaseProtocolTest0/ListPackageListsConformance_0_0_3DF6360E-AB9A-4CB6-BC43-1CDBC8FF50E9.ekl (LISTPA~1.EKL)
    Orphaned long file name part "ListPackageListsFunction_0_0_31338003-325E-45DA-9CA9-427303EEFC67.log"
      Auto-deleting.
    Checking file /Log/HIITest/HIIDatabaseProtocolTest0/ListPackageListsFunction_0_0_31338003-325E-45DA-9CA9-427303EEFC67.log (LISTPA~1.LOG)
    Orphaned long file name part "ListPackageListsFunction_0_0_31338003-325E-45DA-9CA9-427303EEFC67.ekl"
      Auto-deleting.
    Checking file /Log/HIITest/HIIDatabaseProtocolTest0/ListPackageListsFunction_0_0_31338003-325E-45DA-9CA9-427303EEFC67.ekl (LISTPA~1.EKL)
    Orphaned long file name part "NewPackageListConformance_0_0_33F9B795-7169-4E51-B9C8-67FD6B6B1A89.log"
      Auto-deleting.
    Checking file /Log/HIITest/HIIDatabaseProtocolTest0/NewPackageListConformance_0_0_33F9B795-7169-4E51-B9C8-67FD6B6B1A89.log (NEWPAC~1.LOG)
    Orphaned long file name part "NewPackageListConformance_0_0_33F9B795-7169-4E51-B9C8-67FD6B6B1A89.ekl"
      Auto-deleting.
    Checking file /Log/HIITest/HIIDatabaseProtocolTest0/NewPackageListConformance_0_0_33F9B795-7169-4E51-B9C8-67FD6B6B1A89.ekl (NEWPAC~1.EKL)
    Orphaned long file name part "NewPackageListFunction_0_0_A631C5F5-0991-4265-9757-1050AA9668D0.log"
      Auto-deleting.
    Checking file /Log/HIITest/HIIDatabaseProtocolTest0/NewPackageListFunction_0_0_A631C5F5-0991-4265-9757-1050AA9668D0.log (NEWPAC~1.LOG)
    Orphaned long file name part "NewPackageListFunction_0_0_A631C5F5-0991-4265-9757-1050AA9668D0.ekl"
      Auto-deleting.
    Checking file /Log/HIITest/HIIDatabaseProtocolTest0/NewPackageListFunction_0_0_A631C5F5-0991-4265-9757-1050AA9668D0.ekl (NEWPAC~1.EKL)
    Orphaned long file name part "RegisterPackageNotifyConformance_0_0_771A6282-B330-45DB-A4C0-4D801429ED1D.log"
      Auto-deleting.
    Checking file /Log/HIITest/HIIDatabaseProtocolTest0/RegisterPackageNotifyConformance_0_0_771A6282-B330-45DB-A4C0-4D801429ED1D.log (REGIST~1.LOG)
    Orphaned long file name part "RegisterPackageNotifyConformance_0_0_771A6282-B330-45DB-A4C0-4D801429ED1D.ekl"
      Auto-deleting.
    Checking file /Log/HIITest/HIIDatabaseProtocolTest0/RegisterPackageNotifyConformance_0_0_771A6282-B330-45DB-A4C0-4D801429ED1D.ekl (REGIST~1.EKL)
    Orphaned long file name part "RemovePackageListConformance_0_0_FEA8FDC7-7F40-41E0-A84B-A70BE6869ACF.log"
      Auto-deleting.
    Checking file /Log/HIITest/HIIDatabaseProtocolTest0/RemovePackageListConformance_0_0_FEA8FDC7-7F40-41E0-A84B-A70BE6869ACF.log (REMOVE~1.LOG)
    Orphaned long file name part "RemovePackageListConformance_0_0_FEA8FDC7-7F40-41E0-A84B-A70BE6869ACF.ekl"
      Auto-deleting.
    Checking file /Log/HIITest/HIIDatabaseProtocolTest0/RemovePackageListConformance_0_0_FEA8FDC7-7F40-41E0-A84B-A70BE6869ACF.ekl (REMOVE~1.EKL)
    Orphaned long file name part "RemovePackageListFunction_0_0_C35DFC8E-B7C9-413D-A316-C43CAF654C26.log"
      Auto-deleting.
    Checking file /Log/HIITest/HIIDatabaseProtocolTest0/RemovePackageListFunction_0_0_C35DFC8E-B7C9-413D-A316-C43CAF654C26.log (REMOVE~1.LOG)
    Orphaned long file name part "RemovePackageListFunction_0_0_C35DFC8E-B7C9-413D-A316-C43CAF654C26.ekl"
      Auto-deleting.
    Checking file /Log/HIITest/HIIDatabaseProtocolTest0/RemovePackageListFunction_0_0_C35DFC8E-B7C9-413D-A316-C43CAF654C26.ekl (REMOVE~1.EKL)
    Orphaned long file name part "SetKeyboardLayoutConformance_0_0_BA3F895D-E76E-4C43-8A38-D94E95D69F42.log"
      Auto-deleting.
    Checking file /Log/HIITest/HIIDatabaseProtocolTest0/SetKeyboardLayoutConformance_0_0_BA3F895D-E76E-4C43-8A38-D94E95D69F42.log (SETKEY~1.LOG)
    Orphaned long file name part "SetKeyboardLayoutConformance_0_0_BA3F895D-E76E-4C43-8A38-D94E95D69F42.ekl"
      Auto-deleting.
    Checking file /Log/HIITest/HIIDatabaseProtocolTest0/SetKeyboardLayoutConformance_0_0_BA3F895D-E76E-4C43-8A38-D94E95D69F42.ekl (SETKEY~1.EKL)
    Orphaned long file name part "SetKeyboardLayoutFunction_0_0_D0126067-99CD-46C5-839F-43B0A90B79C5.log"
      Auto-deleting.
    Checking file /Log/HIITest/HIIDatabaseProtocolTest0/SetKeyboardLayoutFunction_0_0_D0126067-99CD-46C5-839F-43B0A90B79C5.log (SETKEY~1.LOG)
    Orphaned long file name part "SetKeyboardLayoutFunction_0_0_D0126067-99CD-46C5-839F-43B0A90B79C5.ekl"
      Auto-deleting.
    Checking file /Log/HIITest/HIIDatabaseProtocolTest0/SetKeyboardLayoutFunction_0_0_D0126067-99CD-46C5-839F-43B0A90B79C5.ekl (SETKEY~1.EKL)
    Orphaned long file name part "UnregisterPackageNotifyConformance_0_0_206BB846-46B6-481E-A484-121C8D72FE60.log"
      Auto-deleting.
    Checking file /Log/HIITest/HIIDatabaseProtocolTest0/UnregisterPackageNotifyConformance_0_0_206BB846-46B6-481E-A484-121C8D72FE60.log (UNREGI~1.LOG)
    Orphaned long file name part "UnregisterPackageNotifyConformance_0_0_206BB846-46B6-481E-A484-121C8D72FE60.ekl"
      Auto-deleting.
    Checking file /Log/HIITest/HIIDatabaseProtocolTest0/UnregisterPackageNotifyConformance_0_0_206BB846-46B6-481E-A484-121C8D72FE60.ekl (UNREGI~1.EKL)
    Orphaned long file name part "UpdatePackageListConformance_0_0_C8A7EFF2-A281-4F3D-85CC-BA9CB4E5F6D2.log"
      Auto-deleting.
    Checking file /Log/HIITest/HIIDatabaseProtocolTest0/UpdatePackageListConformance_0_0_C8A7EFF2-A281-4F3D-85CC-BA9CB4E5F6D2.log (UPDATE~1.LOG)
    Orphaned long file name part "UpdatePackageListConformance_0_0_C8A7EFF2-A281-4F3D-85CC-BA9CB4E5F6D2.ekl"
      Auto-deleting.
    Checking file /Log/HIITest/HIIDatabaseProtocolTest0/UpdatePackageListConformance_0_0_C8A7EFF2-A281-4F3D-85CC-BA9CB4E5F6D2.ekl (UPDATE~1.EKL)
    Orphaned long file name part "UpdatePackageListFunction_0_0_00C3A3A0-1A1E-4609-9B0F-F2835301432E.log"
      Auto-deleting.
    Checking file /Log/HIITest/HIIDatabaseProtocolTest0/UpdatePackageListFunction_0_0_00C3A3A0-1A1E-4609-9B0F-F2835301432E.log (UPDATE~1.LOG)
    Orphaned long file name part "UpdatePackageListFunction_0_0_00C3A3A0-1A1E-4609-9B0F-F2835301432E.ekl"
      Auto-deleting.
    Checking file /Log/HIITest/HIIDatabaseProtocolTest0/UpdatePackageListFunction_0_0_00C3A3A0-1A1E-4609-9B0F-F2835301432E.ekl (UPDATE~1.EKL)
    /Log/HIITest/HIIDatabaseProtocolTest0/ExportPackageListsConformance_0_0_B6DCE569-0A0E-4FCE-9EE0-868730F50C4D.log
      Duplicate directory entry.
      First    Size 5352 bytes, date 01:00:00 Jan 01 1980
      Second   Size 2724 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.000
    /Log/HIITest/HIIDatabaseProtocolTest0/ExportPackageListsConformance_0_0_B6DCE569-0A0E-4FCE-9EE0-868730F50C4D.ekl
      Duplicate directory entry.
      First    Size 3268 bytes, date 01:00:00 Jan 01 1980
      Second   Size 528 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.001
    /Log/HIITest/HIIDatabaseProtocolTest0/FindKeyboardLayoutsConformance_0_0_3952E6C7-3B3C-4B24-9320-E2C53CC55025.log
      Duplicate directory entry.
      First    Size 4090 bytes, date 01:00:00 Jan 01 1980
      Second   Size 2734 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.002
    /Log/HIITest/HIIDatabaseProtocolTest0/FindKeyboardLayoutsConformance_0_0_3952E6C7-3B3C-4B24-9320-E2C53CC55025.ekl
      Duplicate directory entry.
      First    Size 2018 bytes, date 01:00:00 Jan 01 1980
      Second   Size 530 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.003
    /Log/HIITest/HIIDatabaseProtocolTest0/GetKeyboardLayoutConformance_0_0_E8683EEB-56A0-401C-89C8-D8BA672F40F0.log
      Duplicate directory entry.
      First    Size 4058 bytes, date 01:00:00 Jan 01 1980
      Second   Size 2714 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.004
    /Log/HIITest/HIIDatabaseProtocolTest0/GetKeyboardLayoutConformance_0_0_E8683EEB-56A0-401C-89C8-D8BA672F40F0.ekl
      Duplicate directory entry.
      First    Size 2002 bytes, date 01:00:00 Jan 01 1980
      Second   Size 526 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.005
    /Log/HIITest/HIIDatabaseProtocolTest0/GetPackageListHandleConformance_0_0_D51EBDA6-391B-49BC-A4CB-0EAF1A0E3A05.log
      Duplicate directory entry.
      First    Size 3436 bytes, date 01:00:00 Jan 01 1980
      Second   Size 2744 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.006
    /Log/HIITest/HIIDatabaseProtocolTest0/GetPackageListHandleConformance_0_0_D51EBDA6-391B-49BC-A4CB-0EAF1A0E3A05.ekl
      Duplicate directory entry.
      First    Size 1366 bytes, date 01:00:00 Jan 01 1980
      Second   Size 532 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.007
    /Log/HIITest/HIIDatabaseProtocolTest0/ListPackageListsConformance_0_0_3DF6360E-AB9A-4CB6-BC43-1CDBC8FF50E9.log
      Duplicate directory entry.
      First    Size 4800 bytes, date 01:00:00 Jan 01 1980
      Second   Size 2704 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.008
    /Log/HIITest/HIIDatabaseProtocolTest0/ListPackageListsConformance_0_0_3DF6360E-AB9A-4CB6-BC43-1CDBC8FF50E9.ekl
      Duplicate directory entry.
      First    Size 2742 bytes, date 01:00:00 Jan 01 1980
      Second   Size 524 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.009
    /Log/HIITest/HIIDatabaseProtocolTest0/NewPackageListConformance_0_0_33F9B795-7169-4E51-B9C8-67FD6B6B1A89.log
      Duplicate directory entry.
      First    Size 3970 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3270 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.010
    /Log/HIITest/HIIDatabaseProtocolTest0/NewPackageListConformance_0_0_33F9B795-7169-4E51-B9C8-67FD6B6B1A89.ekl
      Duplicate directory entry.
      First    Size 1938 bytes, date 01:00:00 Jan 01 1980
      Second   Size 1234 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.011
    /Log/HIITest/HIIDatabaseProtocolTest0/RemovePackageListConformance_0_0_FEA8FDC7-7F40-41E0-A84B-A70BE6869ACF.log
      Duplicate directory entry.
      First    Size 3340 bytes, date 01:00:00 Jan 01 1980
      Second   Size 2714 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.012
    /Log/HIITest/HIIDatabaseProtocolTest0/RemovePackageListConformance_0_0_FEA8FDC7-7F40-41E0-A84B-A70BE6869ACF.ekl
      Duplicate directory entry.
      First    Size 1294 bytes, date 01:00:00 Jan 01 1980
      Second   Size 526 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.013
    /Log/HIITest/HIIDatabaseProtocolTest0/SetKeyboardLayoutConformance_0_0_BA3F895D-E76E-4C43-8A38-D94E95D69F42.log
      Duplicate directory entry.
      First    Size 3374 bytes, date 01:00:00 Jan 01 1980
      Second   Size 2714 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.014
    /Log/HIITest/HIIDatabaseProtocolTest0/SetKeyboardLayoutConformance_0_0_BA3F895D-E76E-4C43-8A38-D94E95D69F42.ekl
      Duplicate directory entry.
      First    Size 1328 bytes, date 01:00:00 Jan 01 1980
      Second   Size 526 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.015
    /Log/HIITest/HIIDatabaseProtocolTest0/UpdatePackageListConformance_0_0_C8A7EFF2-A281-4F3D-85CC-BA9CB4E5F6D2.log
      Duplicate directory entry.
      First    Size 3342 bytes, date 01:00:00 Jan 01 1980
      Second   Size 2714 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.016
    /Log/HIITest/HIIDatabaseProtocolTest0/UpdatePackageListConformance_0_0_C8A7EFF2-A281-4F3D-85CC-BA9CB4E5F6D2.ekl
      Duplicate directory entry.
      First    Size 1296 bytes, date 01:00:00 Jan 01 1980
      Second   Size 526 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.017
    Checking file /Log/HIITest/HIIStringProtocolTest0/.
    Checking file /Log/HIITest/HIIStringProtocolTest0/..
    Orphaned long file name part "GetLanguagesConformance_0_0_24E0CCA8-80F0-4391-8816-3BCC21616E54.log"
      Auto-deleting.
    Checking file /Log/HIITest/HIIStringProtocolTest0/GetLanguagesConformance_0_0_24E0CCA8-80F0-4391-8816-3BCC21616E54.log (GETLAN~1.LOG)
    Orphaned long file name part "GetLanguagesConformance_0_0_24E0CCA8-80F0-4391-8816-3BCC21616E54.ekl"
      Auto-deleting.
    Checking file /Log/HIITest/HIIStringProtocolTest0/GetLanguagesConformance_0_0_24E0CCA8-80F0-4391-8816-3BCC21616E54.ekl (GETLAN~1.EKL)
    Orphaned long file name part "GetLanguagesFunction_0_0_5CE20B3C-CB59-412F-A137-BBE59422F860.log"
      Auto-deleting.
    Checking file /Log/HIITest/HIIStringProtocolTest0/GetLanguagesFunction_0_0_5CE20B3C-CB59-412F-A137-BBE59422F860.log (GETLAN~1.LOG)
    Orphaned long file name part "GetLanguagesFunction_0_0_5CE20B3C-CB59-412F-A137-BBE59422F860.ekl"
      Auto-deleting.
    Checking file /Log/HIITest/HIIStringProtocolTest0/GetLanguagesFunction_0_0_5CE20B3C-CB59-412F-A137-BBE59422F860.ekl (GETLAN~1.EKL)
    Orphaned long file name part "GetSecondaryLanguagesConformance_0_0_AA37EDDC-68EE-4D69-8D0B-A431F1E7B80F.log"
      Auto-deleting.
    Checking file /Log/HIITest/HIIStringProtocolTest0/GetSecondaryLanguagesConformance_0_0_AA37EDDC-68EE-4D69-8D0B-A431F1E7B80F.log (GETSEC~1.LOG)
    Orphaned long file name part "GetSecondaryLanguagesConformance_0_0_AA37EDDC-68EE-4D69-8D0B-A431F1E7B80F.ekl"
      Auto-deleting.
    Checking file /Log/HIITest/HIIStringProtocolTest0/GetSecondaryLanguagesConformance_0_0_AA37EDDC-68EE-4D69-8D0B-A431F1E7B80F.ekl (GETSEC~1.EKL)
    Orphaned long file name part "GetSecondaryLanguagesFunction_0_0_75A47073-8BA9-4B56-8DF1-54A10063F6A1.log"
      Auto-deleting.
    Checking file /Log/HIITest/HIIStringProtocolTest0/GetSecondaryLanguagesFunction_0_0_75A47073-8BA9-4B56-8DF1-54A10063F6A1.log (GETSEC~1.LOG)
    Orphaned long file name part "GetSecondaryLanguagesFunction_0_0_75A47073-8BA9-4B56-8DF1-54A10063F6A1.ekl"
      Auto-deleting.
    Checking file /Log/HIITest/HIIStringProtocolTest0/GetSecondaryLanguagesFunction_0_0_75A47073-8BA9-4B56-8DF1-54A10063F6A1.ekl (GETSEC~1.EKL)
    Orphaned long file name part "GetStringConformance_0_0_9D28A801-49D8-4A7F-895E-732E436BDF3C.log"
      Auto-deleting.
    Checking file /Log/HIITest/HIIStringProtocolTest0/GetStringConformance_0_0_9D28A801-49D8-4A7F-895E-732E436BDF3C.log (GETSTR~1.LOG)
    Orphaned long file name part "GetStringConformance_0_0_9D28A801-49D8-4A7F-895E-732E436BDF3C.ekl"
      Auto-deleting.
    Checking file /Log/HIITest/HIIStringProtocolTest0/GetStringConformance_0_0_9D28A801-49D8-4A7F-895E-732E436BDF3C.ekl (GETSTR~1.EKL)
    Orphaned long file name part "GetStringFunction_0_0_4DFDBDFC-B23F-49DB-9170-7D69FDF88868.log"
      Auto-deleting.
    Checking file /Log/HIITest/HIIStringProtocolTest0/GetStringFunction_0_0_4DFDBDFC-B23F-49DB-9170-7D69FDF88868.log (GETSTR~1.LOG)
    Orphaned long file name part "GetStringFunction_0_0_4DFDBDFC-B23F-49DB-9170-7D69FDF88868.ekl"
      Auto-deleting.
    Checking file /Log/HIITest/HIIStringProtocolTest0/GetStringFunction_0_0_4DFDBDFC-B23F-49DB-9170-7D69FDF88868.ekl (GETSTR~1.EKL)
    Orphaned long file name part "NewStringConformance_0_0_94971A6A-B0EB-4C86-B34A-866886801DF9.log"
      Auto-deleting.
    Checking file /Log/HIITest/HIIStringProtocolTest0/NewStringConformance_0_0_94971A6A-B0EB-4C86-B34A-866886801DF9.log (NEWSTR~1.LOG)
    Orphaned long file name part "NewStringConformance_0_0_94971A6A-B0EB-4C86-B34A-866886801DF9.ekl"
      Auto-deleting.
    Checking file /Log/HIITest/HIIStringProtocolTest0/NewStringConformance_0_0_94971A6A-B0EB-4C86-B34A-866886801DF9.ekl (NEWSTR~1.EKL)
    Orphaned long file name part "NewStringFunction_0_0_F5050750-8E84-46DB-A3E3-62073413A569.log"
      Auto-deleting.
    Checking file /Log/HIITest/HIIStringProtocolTest0/NewStringFunction_0_0_F5050750-8E84-46DB-A3E3-62073413A569.log (NEWSTR~1.LOG)
    Orphaned long file name part "NewStringFunction_0_0_F5050750-8E84-46DB-A3E3-62073413A569.ekl"
      Auto-deleting.
    Checking file /Log/HIITest/HIIStringProtocolTest0/NewStringFunction_0_0_F5050750-8E84-46DB-A3E3-62073413A569.ekl (NEWSTR~1.EKL)
    Orphaned long file name part "SetStringConformance_0_0_69DDDDBB-DCE4-4AFC-9060-26B4998E7DC1.log"
      Auto-deleting.
    Checking file /Log/HIITest/HIIStringProtocolTest0/SetStringConformance_0_0_69DDDDBB-DCE4-4AFC-9060-26B4998E7DC1.log (SETSTR~1.LOG)
    Orphaned long file name part "SetStringConformance_0_0_69DDDDBB-DCE4-4AFC-9060-26B4998E7DC1.ekl"
      Auto-deleting.
    Checking file /Log/HIITest/HIIStringProtocolTest0/SetStringConformance_0_0_69DDDDBB-DCE4-4AFC-9060-26B4998E7DC1.ekl (SETSTR~1.EKL)
    Orphaned long file name part "SetStringFunction_0_0_2EC82B5D-49F7-4B3E-B884-A5EB171E2369.log"
      Auto-deleting.
    Checking file /Log/HIITest/HIIStringProtocolTest0/SetStringFunction_0_0_2EC82B5D-49F7-4B3E-B884-A5EB171E2369.log (SETSTR~1.LOG)
    Orphaned long file name part "SetStringFunction_0_0_2EC82B5D-49F7-4B3E-B884-A5EB171E2369.ekl"
      Auto-deleting.
    Checking file /Log/HIITest/HIIStringProtocolTest0/SetStringFunction_0_0_2EC82B5D-49F7-4B3E-B884-A5EB171E2369.ekl (SETSTR~1.EKL)
    /Log/HIITest/HIIStringProtocolTest0/GetLanguagesConformance_0_0_24E0CCA8-80F0-4391-8816-3BCC21616E54.log
      Duplicate directory entry.
      First    Size 2682 bytes, date 01:00:00 Jan 01 1980
      Second   Size 2652 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.000
    /Log/HIITest/HIIStringProtocolTest0/GetLanguagesConformance_0_0_24E0CCA8-80F0-4391-8816-3BCC21616E54.ekl
      Duplicate directory entry.
      First    Size 514 bytes, date 01:00:00 Jan 01 1980
      Second   Size 508 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.001
    /Log/HIITest/HIIStringProtocolTest0/GetSecondaryLanguagesConformance_0_0_AA37EDDC-68EE-4D69-8D0B-A431F1E7B80F.log
      Duplicate directory entry.
      First    Size 2772 bytes, date 01:00:00 Jan 01 1980
      Second   Size 2742 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.002
    /Log/HIITest/HIIStringProtocolTest0/GetSecondaryLanguagesConformance_0_0_AA37EDDC-68EE-4D69-8D0B-A431F1E7B80F.ekl
      Duplicate directory entry.
      First    Size 532 bytes, date 01:00:00 Jan 01 1980
      Second   Size 526 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.003
    /Log/HIITest/HIIStringProtocolTest0/GetStringConformance_0_0_9D28A801-49D8-4A7F-895E-732E436BDF3C.log
      Duplicate directory entry.
      First    Size 2652 bytes, date 01:00:00 Jan 01 1980
      Second   Size 2622 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.004
    /Log/HIITest/HIIStringProtocolTest0/GetStringConformance_0_0_9D28A801-49D8-4A7F-895E-732E436BDF3C.ekl
      Duplicate directory entry.
      First    Size 508 bytes, date 01:00:00 Jan 01 1980
      Second   Size 502 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.005
    /Log/HIITest/HIIStringProtocolTest0/NewStringConformance_0_0_94971A6A-B0EB-4C86-B34A-866886801DF9.log
      Duplicate directory entry.
      First    Size 2652 bytes, date 01:00:00 Jan 01 1980
      Second   Size 2622 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.006
    /Log/HIITest/HIIStringProtocolTest0/NewStringConformance_0_0_94971A6A-B0EB-4C86-B34A-866886801DF9.ekl
      Duplicate directory entry.
      First    Size 508 bytes, date 01:00:00 Jan 01 1980
      Second   Size 502 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.007
    /Log/HIITest/HIIStringProtocolTest0/SetStringConformance_0_0_69DDDDBB-DCE4-4AFC-9060-26B4998E7DC1.log
      Duplicate directory entry.
      First    Size 2652 bytes, date 01:00:00 Jan 01 1980
      Second   Size 2622 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.008
    /Log/HIITest/HIIStringProtocolTest0/SetStringConformance_0_0_69DDDDBB-DCE4-4AFC-9060-26B4998E7DC1.ekl
      Duplicate directory entry.
      First    Size 508 bytes, date 01:00:00 Jan 01 1980
      Second   Size 502 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.009
    Checking file /Log/SecureTechTest/.
    Checking file /Log/SecureTechTest/..
    Checking file /Log/SecureTechTest/RNGProtocolTest0 (RNGPRO~1)
    Checking file /Log/SecureTechTest/RNGProtocolTest0/.
    Checking file /Log/SecureTechTest/RNGProtocolTest0/..
    Orphaned long file name part "GetInfo_Conf_0_0_861F4A3B-8125-4A5A-99CC-DA7779C2B020.log"
      Auto-deleting.
    Checking file /Log/SecureTechTest/RNGProtocolTest0/GetInfo_Conf_0_0_861F4A3B-8125-4A5A-99CC-DA7779C2B020.log (GETINF~1.LOG)
    Orphaned long file name part "GetInfo_Conf_0_0_861F4A3B-8125-4A5A-99CC-DA7779C2B020.ekl"
      Auto-deleting.
    Checking file /Log/SecureTechTest/RNGProtocolTest0/GetInfo_Conf_0_0_861F4A3B-8125-4A5A-99CC-DA7779C2B020.ekl (GETINF~1.EKL)
    Orphaned long file name part "GetInfo_Func_0_0_39FF9C71-4B41-4E5B-AED7-87C794187D66.log"
      Auto-deleting.
    Checking file /Log/SecureTechTest/RNGProtocolTest0/GetInfo_Func_0_0_39FF9C71-4B41-4E5B-AED7-87C794187D66.log (GETINF~1.LOG)
    Orphaned long file name part "GetInfo_Func_0_0_39FF9C71-4B41-4E5B-AED7-87C794187D66.ekl"
      Auto-deleting.
    Checking file /Log/SecureTechTest/RNGProtocolTest0/GetInfo_Func_0_0_39FF9C71-4B41-4E5B-AED7-87C794187D66.ekl (GETINF~1.EKL)
    Orphaned long file name part "GetRNG_Conf_0_0_DDBBE5AB-206E-4F35-9556-186DA87C2A86.log"
      Auto-deleting.
    Checking file /Log/SecureTechTest/RNGProtocolTest0/GetRNG_Conf_0_0_DDBBE5AB-206E-4F35-9556-186DA87C2A86.log (GETRNG~1.LOG)
    Orphaned long file name part "GetRNG_Conf_0_0_DDBBE5AB-206E-4F35-9556-186DA87C2A86.ekl"
      Auto-deleting.
    Checking file /Log/SecureTechTest/RNGProtocolTest0/GetRNG_Conf_0_0_DDBBE5AB-206E-4F35-9556-186DA87C2A86.ekl (GETRNG~1.EKL)
    Orphaned long file name part "GetRNG_Func_0_0_DC5B2884-EDFB-4078-A288-4DFDA849A08D.log"
      Auto-deleting.
    Checking file /Log/SecureTechTest/RNGProtocolTest0/GetRNG_Func_0_0_DC5B2884-EDFB-4078-A288-4DFDA849A08D.log (GETRNG~1.LOG)
    Orphaned long file name part "GetRNG_Func_0_0_DC5B2884-EDFB-4078-A288-4DFDA849A08D.ekl"
      Auto-deleting.
    Checking file /Log/SecureTechTest/RNGProtocolTest0/GetRNG_Func_0_0_DC5B2884-EDFB-4078-A288-4DFDA849A08D.ekl (GETRNG~1.EKL)
    /Log/SecureTechTest/RNGProtocolTest0/GetInfo_Conf_0_0_861F4A3B-8125-4A5A-99CC-DA7779C2B020.log
      Duplicate directory entry.
      First    Size 3234 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3608 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.000
    /Log/SecureTechTest/RNGProtocolTest0/GetInfo_Conf_0_0_861F4A3B-8125-4A5A-99CC-DA7779C2B020.ekl
      Duplicate directory entry.
      First    Size 1390 bytes, date 01:00:00 Jan 01 1980
      Second   Size 1760 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.001
    /Log/SecureTechTest/RNGProtocolTest0/GetRNG_Conf_0_0_DDBBE5AB-206E-4F35-9556-186DA87C2A86.log
      Duplicate directory entry.
      First    Size 5482 bytes, date 01:00:00 Jan 01 1980
      Second   Size 3612 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.002
    /Log/SecureTechTest/RNGProtocolTest0/GetRNG_Conf_0_0_DDBBE5AB-206E-4F35-9556-186DA87C2A86.ekl
      Duplicate directory entry.
      First    Size 3606 bytes, date 01:00:00 Jan 01 1980
      Second   Size 1668 bytes, date 01:00:00 Jan 01 1980
      Auto-renaming second.
      Renamed to FSCK0000.003
    Checking for bad clusters.
    Reclaiming unconnected clusters.
    Performing changes.
    /dev/loop0: 1141 files, 17263/65398 clusters
