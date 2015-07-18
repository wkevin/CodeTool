# CodeTool
some tools for read code

## howmany

This tool can count the file number with the given filename extension.
It can help you to understand the file layout in a new source code project.

**Usage**

* copy the `howmany` to /usr/bin or ~/bin/
* chown a+x howmany
* cd the code folder
* `howmany [extension]`

**Comments**

* ignore the .svn and .git forlder and files
 
**example**

```
$ howmany mk java aidl cpp h  html xml png 
     All       mk     java     aidl      cpp        h     html      xml      png 
  375318     4765    36308      716    24599   111074     9947    25558    30542  - .
      19        2        0        0        0        1        0        0        0  - abi
    1340       21      372        0        0      405        0        0        0  - art
    3481       33        1        0      276     1204        0        0        0  - bionic
     191       13        0        0       12       39        0        0       52  - bootable
    1196      230       31        0        6       15        1        0      546  - build
    8435      282     3859        8      156      102       35      814      135  - cts
    1104       14      690        0       19       19       20        0        0  - dalvik
    6018        0     1024        0        0        0        0     2023     1502  - developers
    9874      160     1755        4       71     2399       94     2803     1752  - development
    2862      423       27        0      206      424        0     1118       79  - device
     259        2        0        0        0        0        7        1       49  - docs
  172843     1563    11327       15    17484    40263     5975     1933     6937  - external
   34610      694     7150      645     1972     2082     3647     5369     9341  - frameworks
    4869      444       13        0      579     2254        1        4        0  - hardware
    4732        9     4241        0       55       15       18       30        0  - libcore
      24        2        0        0        5       14        0        0        0  - libnativehelper
    6282      386        1        0     3200      527       66        2       31  - ndk
       2        2        0        0        0        0        0        0        0  - out
   27386      223     5584       21      202      430       29    10477     9702  - packages
     159        6       39        0        1        0        0       34        6  - pdk
   87155       76       17       19        3    60328       49      714      308  - prebuilts
    1058       46      132        4      107      131        4      235       99  - sdk
    1361      132        6        0      245      422        1        1        3  - system
      56        2       39        0        0        0        0        0        0  - tools
```

## howheavy

wait...


