# Upgrade CSW-WR246 from ZBT OS to OpenWrt (19.07.7)

**Disclaimer**: This is created as a memo for myself, I take responsibility for nothing that might happen fellowing these instructions.

Tested with: CSW-WR246 (ZBT WE-1326) , 16MB Rom, 256MB RAM, (V1 Eco3)

## ZBT OS To Openwrt

1. Disconnect AC
2. Press and hold Reset button while connecting the AC - Hold 20s
3. Enter http://192.168.1.1 (If needed setup manual IP: 192.168.1.100 with subnet 255.255.255.0)
4. Recovery mode site should go up in chinese use google translate and find Upgrade buttons.
5. Use attached bin file [lede_openwrt](lede-ramips-mt7621-zbt-we1326-20210301_142937.bin) or download from [here](http://mte.f3322.net:10180/new-openwrt/mt7621/lede-ramips-mt7621-zbt-we1326-20210301_142937.bin)
6. Wait for burn to finish
7. Go again to http://192.168.1.1 
8. Login with User:root Password:admin
9. You'll see red message saying something like **Unauthorized**
10. Once the router have access to the internet, visit http://192.168.1.1/cgi-bin/auth.cgi
11. Now flash you can flash OpenWrt updated Firmware
12. Either use [Firmware Selector](https://firmware-selector.openwrt.org/?version=19.07.7&target=ramips%2Fmt7621&id=zbt-we1326) or use attached [OpenWrt-19.07.7.bin](openwrt-19.07.7-ramips-mt7621-zbt-we1326-squashfs-sysupgrade.bin)
13. Wait for burn to finish and that's it!


## Resources:

1. Lede-OpenWrt images for various Mediatech Devices: http://mte.f3322.net:10180/new-openwrt/
2. Translated Changlog (Google Translate) - [Changelog.txt](lede_openwrt_changlog_google_translated.txt)

