# OpenWrt firmware for the Newland NL-WR8103

OpenWrt firmware for the Newland NL-WR8103 router (China Unicom model, MT7981B, 256 MB RAM).

## Firmware

- `openwrt-mediatek-filogic-newland_nl-wr8103-squashfs-sysupgrade.bin` — sysupgrade image for the NL-WR8103.

## Build

Built from OpenWrt main (hanimeia/openwrt) with PR #19006 device support plus a fixed device tree.

## Management

This image has no LuCI. Manage the router over SSH / CLI.

## Flashing via U-Boot

1. Set your PC to IP address 192.168.1.2.
2. Connect your PC to the router's WAN port.
3. Hold the reset button until the LED blinks 5 times.
4. Open http://192.168.1.1/ in a browser.
5. Upload the sysupgrade file (`openwrt-mediatek-filogic-newland_nl-wr8103-squashfs-sysupgrade.bin`).

## SHA256

```
2f6eeead2fce7caa05d05a94d984d72db3a192e58666192170fdc1789afba2a3
```

## Notes / known limitations

- LED/button GPIOs and the WAN PHY are untested.
