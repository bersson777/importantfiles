# importantfiles
I am presently living in Pittsburgh. I am a retired man of 65 years old
using Debian 9.9 with research that takes the time of my said retirement.
I joined the github to gain insight and technique with my Debian Kernel
firstly tending to the issues of USB configs. I am sucessfully done the make,
make install and modprobe for rtl8192cu.

Observe these basic steps:

sudo apt-get install linux-headers-generic build-essential dkms

Clone this repository:

git clone https://github.com/pvaret/rtl8192cu-fixes.git

Set it up as a DKMS module:

sudo dkms add ./rtl8192cu-fixes

Build and install it

sudo dkms install 8192cu/1.10

Refresh the module list:

sudo depmod -a
