# sdat2img
Convert sparse Android data images (.dat) into filesystem images (.img)



## Requirements
This binary requires Python 2.7 or newer installed on your system. 
It currently supports Windows, Linux, MacOS & ARM architectures.

**Note:** Google's newer [Brotli](https://github.com/google/brotli) format (`partition.new.dat.br`) must be decompressed to a valid sparse data image before using `sdat2img` binary.



## Usage
```
sdat2img.py <transfer_list> <partition_new_file> [output_img]
```
- `<transfer_list>` = input, partition.transfer.list from rom zip
- `<partition_new_file>` = input, partition.new.dat from rom zip
- `[output_img]` = output, raw image file (optional)



## Example
This is a simple example on a Linux system: 
```
~$ ./sdat2img.py system.transfer.list system.new.dat system.img
```



## OTAs
If you are looking on decompressing `partition.patch.dat` file or `.p` files, therefore reproduce the patching system on your PC, check [imgpatchtools](https://github.com/erfanoabdi/imgpatchtools) out by @erfanoabdi.



## Info
For more information about this binary, visit it's [XDA page](https://forum.xda-developers.com/android/software-hacking/how-to-conver-lollipop-dat-files-to-t2978952).
