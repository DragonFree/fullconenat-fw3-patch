## FULLCONENAT target patch for OpenWrt firewall3

Depends: https://github.com/LGA1150/openwrt-fullconenat


Compile
```
# Download fullconenat.patch to package/network/config/firewall/patches/
mkdir package/network/config/firewall/patches
wget -O package/network/config/firewall/patches/ https://github.com/LGA1150/fullconenat-fw3-patch/raw/master/fullconenat.patch
# Compile firewall3 only
make package/firewall/compile V=s
# or compile the whole image
make V=s
```
