# The Calibrator, a Cache-Memory and TLB Calibration Tool.
This tool was originally developed by [Stefan Manegold](https://homepages.cwi.nl/~manegold/) and has not been updated for many years. I manage to make some adaptions to make it compatible on newly released Linux kernels. 

## Environment
Linux kernel version >= 4.11.0  
CMake version >= 3.5.2

## Usage
### Build
```
mkdir build
cd build/
cmake ..
make
cd ../
```
###
```
cd bin/
./calibrator [MHz] [size] [filename], e.g., ./calibrator 1900 10G stdout

	[MHz] 
		gives the CPU's clock speed in Mega Hertz (MHz).
	[size] 
		gives the amount of memory to be used. [size] should be smaller than the total amount of main memory, but it should be significantly bigger than the maximum cache size expected. 
		[size] is interpreted as bytes; suffixes "k" ("kilo" = 1024), "M" ("Mega" = 10242), and "G" ("Giga" = 10243) may be used.
	[filename] 
		gives the filename for the result files.
```

## Contact
This repo is maintained by Huang Wentao. Please contact huangwentao@u.nus.edu for the further support.