# k2p-openwrt-mt7615_5.0.2.0
For [openwrt R9.6.1](https://github.com/coolsnowwolf/lede/)

## Install

```bash
cd lede
git clone https://github.com/WingLim/k2p-openwrt-mt7615.git
mv k2p-openwrt-mt7615_5.0.2.0/mtk package/mtk
```

## Configure

```bash
make menuconfig
MTK Properties-->Drivers-->kmod-mt_wifi
	Choose First WiFi Interface-->MT7615E
	MT WIFI Driver-->WiFi Operation Modes-->AP
MTK Properties-->Drivers-->wifi-l1-profile-->1st card
MTK Properties-->Misc-->mtk-luci-plugin-->luci-app-mtk-wifi
```


编译时遇到的错误参考了hanwckf的patch https://github.com/hanwckf/openwrt-mt7615
