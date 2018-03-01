# OS_Design_Proj
CS630 Group Project


Setting up environments
- need to install two tools
  1. QEMU, an x86 emulator
  2. compiler toolchain
  
# 1. QEMU
# 2. Compiler toolchain
For linux machine, these should be readily available.
type command in VM Linux terminal:

objdump -i
  should print a table with 2nd line = "elf32-i386"

gcc -m32 -print-libgcc-file-name
  should print a directory start with "/user/lib" and end with "/libgcc.a"

