# llvmLinux
linux that is llvm-3.8.1 compilable

The code is built on v.4.17 linux stable release with a patch from sedat.dilek@gmail.com, and few patches and configuration files not merged into linux mainline kernel.

## Prerequisites:

binutils 2.26.1
replace ld in binutils with ld-gold

install llvm 3.8.1 stable http://llvm.org/releases/download.html
install clang cfe-3.8.1.src.tar.xz

## Build Instructions

make CC=clang HOSTCC=clang AS=llvm-as -j <no of processors>
