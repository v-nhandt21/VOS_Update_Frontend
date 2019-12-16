
# For Ubuntu 18.04

  - Start at folder **VOS_Update_Frontend**
  - Extract: **icu4c-64_2-Ubuntu18.04-x64.tgz** 
    then we have **icu** folder
```sh
$ tar xvzf icu4c-64_2-Ubuntu18.04-x64.tgz
```
  - Copy all folders in **icu/usr/local** to replace same-name-folders in **VOS_Update_Frontend**
    (OVERWRITE ALL FOLDERS: bin, include, lib, sbin, share)
  - Move to src
```sh
$ cd src
```
  - Set LD_LIBRARY_PATH to "lib" folder in current folder
```sh
$ export LD_LIBRARY_PATH=../lib
```
  - Run make main to compile
```sh
$ make main
```
  - Reading text from "input.txt" and print to "output.txt" (create new file input.txt to input, the input.txt must have content)
```sh
$ touch input.txt
$ ./main
```
