# wifi driver for rtl8821ce


# steps for installation:

1. You need to have git and dkms installed:
    `sudo apt install build-essential git dkms`

- optional: 

You should be able to install the kernel header files for the currently running kernel by running the following in a terminal:

    `sudo apt-get install linux-headers-$(uname -r)`
In general, the kernel header packages are named linux-header-* where "*" indicates the version & variant (generic, server, etc.).

2. clone this repository:
    `git clone --depth=1 https://github.com/lulzx/rtl8821ce.git rtl8821ce`
    
3. enter into the directory and begin installation:
    `cd rtl8821ce && sudo bash ./dkms-install.sh`
    
4. start the wifi dkms module:
    `sudo modprobe 8821ce`
    
That's all.
