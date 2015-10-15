# **root-pi**
A simple shell based OS for Raspberry Pi using Buildroot.

## **What is Buildroot**
From Wikipedia, [Buildroot](https://en.wikipedia.org/wiki/Buildroot) is a set of Makefiles and patches that simplifies and automates the process of building a complete and bootable Linux environment for an embedded system. It uses [**cross-compilation**](https://en.wikipedia.org/wiki/Cross_compiler), ie you can generate binaries for the ARM based Raspberry Pi by building them on your Intel x86 machine. You can download the latest version of Buildroot [here](http://buildroot.uclibc.org/).

## Building root-pi
```
git clone https://github.com/1337ninja/root-pi/
cd root-pi
cp custom_configs/glibc_2.21.config .config
make
```
The above commands would start building your OS for Raspberry Pi. Depending on your processor and network connectivity it could take a minimum of one hour. After the build completes, the required files would be available in the **output/packages** folder.
