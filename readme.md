#Homework 1
##Violet Smith
## 03/01/2022

### 1. pmap Utility

a) Libraries used:
<ul>
    <li> libnss- Name switch configuration file handles each call to a function in which it retrieves data from a system database.
    </li>
    <li> libc- Libc is used to describe the standard c libraries held in linux.
    </li>
    <li> libdl- Dynamic linking library, is used to provide dynamic linking support. It provides backward compatibility for compilation and runtime enviornments.
    </li>
    <li> libtinfo- ???
    </li>

</ul>

b) Other than the virtual page numbers the two bash programs are identical. <b> Ask others if the actual addresses are the same</b>


## output from terminal A:
pmap 1985
1985:   bash
000055fc9c642000    180K r---- bash
000055fc9c66f000    708K r-x-- bash
000055fc9c720000    220K r---- bash
000055fc9c757000     16K r---- bash
000055fc9c75b000     36K rw--- bash
000055fc9c764000     40K rw---   [ anon ]
000055fc9de65000   1432K rw---   [ anon ]
00007f791a745000     12K r---- libnss_files-2.31.so
00007f791a748000     28K r-x-- libnss_files-2.31.so
00007f791a74f000      8K r---- libnss_files-2.31.so
00007f791a751000      4K r---- libnss_files-2.31.so
00007f791a752000      4K rw--- libnss_files-2.31.so
00007f791a753000     24K rw---   [ anon ]
00007f791a76b000   5568K r---- locale-archive
00007f791acdb000     12K rw---   [ anon ]
00007f791acde000    148K r---- libc-2.31.so
00007f791ad03000   1504K r-x-- libc-2.31.so
00007f791ae7b000    296K r---- libc-2.31.so
00007f791aec5000      4K ----- libc-2.31.so
00007f791aec6000     12K r---- libc-2.31.so
00007f791aec9000     12K rw--- libc-2.31.so
00007f791aecc000     16K rw---   [ anon ]
00007f791aed0000      4K r---- libdl-2.31.so
00007f791aed1000      8K r-x-- libdl-2.31.so
00007f791aed3000      4K r---- libdl-2.31.so
00007f791aed4000      4K r---- libdl-2.31.so
00007f791aed5000      4K rw--- libdl-2.31.so
00007f791aed6000     56K r---- libtinfo.so.6.2
00007f791aee4000     60K r-x-- libtinfo.so.6.2
00007f791aef3000     56K r---- libtinfo.so.6.2
00007f791af01000     16K r---- libtinfo.so.6.2
00007f791af05000      4K rw--- libtinfo.so.6.2
00007f791af06000      8K rw---   [ anon ]
00007f791af13000     28K r--s- gconv-modules.cache
00007f791af1a000      4K r---- ld-2.31.so
00007f791af1b000    140K r-x-- ld-2.31.so
00007f791af3e000     32K r---- ld-2.31.so
00007f791af47000      4K r---- ld-2.31.so
00007f791af48000      4K rw--- ld-2.31.so
00007f791af49000      4K rw---   [ anon ]
00007fffe34aa000    132K rw---   [ stack ]
00007fffe35aa000     12K r----   [ anon ]
00007fffe35ad000      4K r-x--   [ anon ]
ffffffffff600000      4K --x--   [ anon ]
 total            10876K
## Output from Terminal B:
pmap 2499
2499:   bash
0000563a71e98000    180K r---- bash
0000563a71ec5000    708K r-x-- bash
0000563a71f76000    220K r---- bash
0000563a71fad000     16K r---- bash
0000563a71fb1000     36K rw--- bash
0000563a71fba000     40K rw---   [ anon ]
0000563a72742000   1432K rw---   [ anon ]
00007f63bef3b000     12K r---- libnss_files-2.31.so
00007f63bef3e000     28K r-x-- libnss_files-2.31.so
00007f63bef45000      8K r---- libnss_files-2.31.so
00007f63bef47000      4K r---- libnss_files-2.31.so
00007f63bef48000      4K rw--- libnss_files-2.31.so
00007f63bef49000     24K rw---   [ anon ]
00007f63bef61000   5568K r---- locale-archive
00007f63bf4d1000     12K rw---   [ anon ]
00007f63bf4d4000    148K r---- libc-2.31.so
00007f63bf4f9000   1504K r-x-- libc-2.31.so
00007f63bf671000    296K r---- libc-2.31.so
00007f63bf6bb000      4K ----- libc-2.31.so
00007f63bf6bc000     12K r---- libc-2.31.so
00007f63bf6bf000     12K rw--- libc-2.31.so
00007f63bf6c2000     16K rw---   [ anon ]
00007f63bf6c6000      4K r---- libdl-2.31.so
00007f63bf6c7000      8K r-x-- libdl-2.31.so
00007f63bf6c9000      4K r---- libdl-2.31.so
00007f63bf6ca000      4K r---- libdl-2.31.so
00007f63bf6cb000      4K rw--- libdl-2.31.so
00007f63bf6cc000     56K r---- libtinfo.so.6.2
00007f63bf6da000     60K r-x-- libtinfo.so.6.2
00007f63bf6e9000     56K r---- libtinfo.so.6.2
00007f63bf6f7000     16K r---- libtinfo.so.6.2
00007f63bf6fb000      4K rw--- libtinfo.so.6.2
00007f63bf6fc000      8K rw---   [ anon ]
00007f63bf709000     28K r--s- gconv-modules.cache
00007f63bf710000      4K r---- ld-2.31.so
00007f63bf711000    140K r-x-- ld-2.31.so
00007f63bf734000     32K r---- ld-2.31.so
00007f63bf73d000      4K r---- ld-2.31.so
00007f63bf73e000      4K rw--- ld-2.31.so
00007f63bf73f000      4K rw---   [ anon ]
00007ffebf266000    132K rw---   [ stack ]
00007ffebf2a3000     12K r----   [ anon ]
00007ffebf2a6000      4K r-x--   [ anon ]
ffffffffff600000      4K --x--   [ anon ]
 total            10876K

