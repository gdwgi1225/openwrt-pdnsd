Pdnsd for OpenWrt/LEDE
===

简介
---

 本项目是 [pdnsd][1] 在 OpenWrt/LEDE 上的移植

编译
---

 - 从 OpenWrt 的 [SDK][S] 编译

   ```bash
   # 以 ar71xx 平台为例
   tar xjf OpenWrt-SDK-ar71xx-for-linux-x86_64-gcc-4.8-linaro_uClibc-0.9.33.2.tar.bz2
   cd OpenWrt-SDK-ar71xx-*
   git clone https://github.com/Hill-98/openwrt-pdnsd package/pdnsd
   # 选择要编译的包 Network -> pdnsd
   make menuconfig
   # 开始编译
   make package/pdnsd/compile V=99
   ```

[1]: https://github.com/wongsyrone/pdnsd
[S]: https://wiki.openwrt.org/doc/howto/obtain.firmware.sdk