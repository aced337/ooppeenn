openwrt
=
Version:19.07.7

update logs : https://openwrt.org/releases/19.07/changelog-19.07.7

Compilation steps:

1 sudo apt-get -y install gcc-6+ binutils bzip2 flex python3 perl make4.1+ find grep diff unzip gawk getopt
subversion libz-dev libc-dev rsync which

2 mkdir openwrt

3 sudo chmod 777 openwrt

4 cd openwrt

5 git clone https://github.com/Tonkercke/openwrt.git

6 cd openwrt

7 ./scripts/feeds update -a

8 ./scripts/feeds install -a

9 make menuconfig

10 make V=99

