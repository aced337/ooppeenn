openwrt
=
Version:19.07.7

update logs : https://openwrt.org/releases/19.07/changelog-19.07.7

Compilation steps:

1 sudo apt install subversion g++ zlib1g-dev build-essential git python python3 flex libz-dev uglifyjs gcc-multilib msmtp texinfo autoconf automake libtool autopoint device-tree-compiler

sudo apt install libncurses5-dev gawk gettext unzip file libssl-dev wget asciidoc binutils g++-multilib antlr3 gperf swig rsync

sudo apt install libelf-dev ecj fastjar java-propose-classpath bzip2 patch lib32gcc1 libc6-dev-i386 libglib2.0-dev xmlto qemu-utils upx curl

sudo apt install build-essential libncursesw5-dev python unzip

2 mkdir openwrt

3 sudo chmod 777 openwrt

4 cd openwrt

5 git clone https://github.com/Tonkercke/openwrt.git

6 cd openwrt

7 ./scripts/feeds update -a

8 ./scripts/feeds install -a

9 make menuconfig

10 make V=99

