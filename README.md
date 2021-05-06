openwrt
=
Version:19.07.7

update logs : https://openwrt.org/releases/19.07/changelog-19.07.7

Compilation steps:

1 sudo apt install -y git make gcc g++ gawk python libncurses-dev

2 mkdir openwrt

3 cd openwrt

4 git clone https://github.com/Tonkercke/openwrt.git

5 cd openwrt

6 ./scripts/feeds update -a

7 ./scripts/feeds install -a

8 make menuconfig

9 make -j1 V=s
