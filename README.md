# Merlin-WIFI-Boost
此程式为旧AC5300固件所提取的无线网络调节程式而备份，华硕更新了新的wl程式后，导致无法对功率进行查询和调节，在新的AC5300上运行此程式可以对无法对功率进行查询和调节。

```shell
wget -O /koolshare/bin/wl1 http://firmware.koolshare.cn/binary/wl_for_sdk7/wl
chmod +x /koolshare/bin/wl1
# 查询2.4G功率
wl1 -i eth1 txpwr_target_max
# 查询5G1功率
wl1 -i eth2 txpwr_target_max
# 修改2.4G功率为500mw
wl1 -i eth1 txpwr 500
# 修改5G功率为500mw
wl1 -i eth2 txpwr 500
```
