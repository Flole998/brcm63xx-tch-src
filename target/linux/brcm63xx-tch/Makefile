
# Copyright (C) 2006-2009 OpenWrt.org
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#
include $(TOPDIR)/rules.mk

ARCH:=arm
BOARD:=brcm63xx-tch
BOARDNAME:=Broadcom BCM63xx Technicolor
#chriskuo+e
CPU_TYPE:=cortex-a9
CPU_SUBTYPE:=neon
FEATURES:=squashfs jffs2 usb atm pci pcmcia

LINUX_VERSION:=3.4.11
LINUX_RELEASE:=rt19
KERNEL_PATCHVER:=3.4

include $(INCLUDE_DIR)/target.mk

#DEFAULT_PACKAGES += kmod-switch gpioctl

define Target/Description
	Build firmware images for Broadcom based xDSL/routers
	currently supports BCM6338, BCM6348 and BCM6358 based devices.
	(e.g. Inventel Livebox, Siemens SE515, Neufbox 4)
endef

$(eval $(call BuildTarget))
