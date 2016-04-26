
http://ljdelight.com/compiling-openwrt-from-source/

vagrant@debian-8:~$ history
 1  cd openwrt.git/
 2  ls
 3  grep error build.log
 4  grep -i error build.log  | tail -100
 5  cd openwrt.git/
 6  make -j1 V=s
 7  make target/linux/{clean,prepare} V=s QUILT=1
 8  make defconfig
 9  less .config
 10  ls -altr target/linux/ar71xx/patches-3.18/
 11  ls /vagrant_data/patches/
 12  cat /vagrant_data/patches/OpenWrt-Devel-PATCHv3-kernel-Support-for-new-Archer-C7-with-gd25q128-chip-in-15.05.1.patch
 13  ls -altr generic/linux/patches-3.18/004
 14  ls -altr target/linux/generic/patches-3.18/
 15  cat /vagrant_data/patches/OpenWrt-Devel-PATCHv3-kernel-Support-for-new-Archer-C7-with-gd25q128-chip-in-15.05.1.patch
 16  ls -altr target/linux/generic/patches-3.18/
 17  cat target/linux/generic/patches-3.18/043-mtd_GD25Q128B_support_backport_from_3.19.patch
 18  make defconfig
 19  make prereq
 20  time make -j8 V=s
 21  time make -j1 V=s
