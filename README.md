# openwrt-rockchip-kernel

OpenWrt kernel patches for Rockchip devices (NanoPi R6S, etc.)

## Usage

Run `./generate-patch.sh` to generate a monolithic kernel patch file from OpenWrt patches.

This script:
1. Clones OpenWrt at the specified version (v24.10.4)
2. Downloads the vanilla Linux kernel (6.6.110)
3. Applies OpenWrt generic patches (backport, pending, hack)
4. Applies Rockchip-specific patches
5. Generates a single monolithic patch file

Output: `00001-openwrt-rockchip-kernel-6.6.110.patch`
