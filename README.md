# sdat2img
Convert sparse Android data images (.dat) into filesystem images (.img)

## Requirements
This binary requires Python 2.7 or newer installed on your system.

## Usage
```
sdat2img <transfer_list> <new_dat> [-o OUT]
```
- `<transfer_list>` = input transfer list
- `<new_dat>` = input data image
- `[-o out]` = output file path (partition.img in the current directory by default)

## Example
This is a simple example on a Linux system: 
```
~$ ./sdat2img system.transfer.list system.new.dat -o tmp/system.img
```
It will create `system.img` in the `tmp` directory.

## OTAs
If you are looking into decompressing `.patch.dat` file or `.p` files, therefore reproduce the patching system on your PC, check out [imgpatchtools](https://github.com/erfanoabdi/imgpatchtools) by @erfanoabdi.

## Info
For more information about this binary, visit it's [XDA page](http://forum.xda-developers.com/android/software-hacking/how-to-conver-lollipop-dat-files-to-t2978952).
