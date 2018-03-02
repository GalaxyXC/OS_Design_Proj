# OS_Design_Proj
CS630 Group Project


Setting up environments
- need to install two tools
  1. QEMU, an x86 emulator
  2. compiler toolchain
  
# 1. QEMU
Need to download the MIT version of QEMU using Git

1.0 setup VM internet connection
Setup connection in VBox: https://askubuntu.com/questions/363003/no-internet-connection-on-virtualbox-windows-7-as-guest-ubuntu-13-04-as-host

Solve DNS server issue: https://askubuntu.com/questions/210063/12-04-on-virtualbox-no-internet-access-on-guest-os/248308#248308

1.1 Install Git
naive apt-get https://gist.github.com/derhuerst/1b15ff4652a867391f03#file-linux-md
install from mirror https://git-scm.com/book/en/v1/Getting-Started-Installing-Git

1.1.1 Install required lib
http://www.golinuxhub.com/2014/03/how-to-install-libraries-manually-in.html

# 2. Compiler toolchain
For linux machine, these should be readily available.
type command in VM Linux terminal:

objdump -i
  should print a table with 2nd line = "elf32-i386"

gcc -m32 -print-libgcc-file-name
  should print a directory start with "/user/lib" and end with "/libgcc.a"

