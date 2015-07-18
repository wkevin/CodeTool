# CodeTool
some tools for read code

## howmany

This tool can count the file number with the given filename extension.
It can help you to understand the file layout in a new source code project.

**Usage**

* copy the `howmany` to /usr/bin or ~/bin/
* chown a+x howmany
* cd the code folder
* `howmany [extension] [find depth]`
    * extension: file extension without '.'
    * find depth: list the folders with this number, and this number can be anywhere

**Comments**

* ignore the .svn and .git forlder and files
 
**example**

```
aosp-5.0$ howmany mk java aidl cpp h  xml 

     All       mk     java     aidl      cpp        h      xml 
  375318     4765    36308      716    24599   111074    25558  - .
      19        2        0        0        0        1        0  - abi
    1340       21      372        0        0      405        0  - art
    3481       33        1        0      276     1204        0  - bionic
     191       13        0        0       12       39        0  - bootable
    1196      230       31        0        6       15        0  - build
    8435      282     3859        8      156      102      814  - cts
    1104       14      690        0       19       19        0  - dalvik
    6018        0     1024        0        0        0     2023  - developers
    9874      160     1755        4       71     2399     2803  - development
    2862      423       27        0      206      424     1118  - device
     259        2        0        0        0        0        1  - docs
  172843     1563    11327       15    17484    40263     1933  - external
   34610      694     7150      645     1972     2082     5369  - frameworks
    4869      444       13        0      579     2254        4  - hardware
    4732        9     4241        0       55       15       30  - libcore
      24        2        0        0        5       14        0  - libnativehelper
    6282      386        1        0     3200      527        2  - ndk
       2        2        0        0        0        0        0  - out
   27386      223     5584       21      202      430    10477  - packages
     159        6       39        0        1        0       34  - pdk
   87155       76       17       19        3    60328      714  - prebuilts
    1058       46      132        4      107      131      235  - sdk
    1361      132        6        0      245      422        1  - system
      56        2       39        0        0        0        0  - tools
```

```
aosp-5.0/bionic$ howmany mk java aidl cpp h  2

     All       mk     java     aidl      cpp        h 
    3481       33        1        0      276     1204  - .
      11        1        0        0        9        1  - benchmarks
    3090       22        1        0      185     1175  - libc
     264        8        0        0        0        6  ------ arch-arm
     226        4        0        0        0        5  ------ arch-arm64
       8        0        0        0        0        4  ------ arch-common
     222        1        0        0        1       10  ------ arch-mips
     215        1        0        0        0       10  ------ arch-mips64
       3        1        0        0        0        0  ------ zoneinfo
       4        1        0        0        0        0  - libdl
     245        1        0        0        0       18  - libm
       1        0        0        0        0        0  ------ amd64
       1        0        0        0        0        0  ------ arm
       1        0        0        0        0        0  ------ arm64
       2        0        0        0        0        1  ------ i387
       8        0        0        0        0        8  ------ include
       1        0        0        0        0        0  ------ mips
     221        0        0        0        0        7  ------ upstream-freebsd
      22        0        0        0        0        1  - libstdc++
      20        0        0        0        0        1  ----------- include
      26        3        0        0        9        6  - linker
       6        0        0        0        0        0  -------- arch
       3        1        0        0        2        0  -------- tests
      80        3        0        0       73        3  - tests
       6        1        0        0        5        0  ------- libs
```

## howheavy

wait...


