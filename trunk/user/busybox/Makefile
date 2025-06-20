include $(ROOTDIR)/rules.mk

PKG_NAME:=busybox
PKG_VERSION:=1.34.1

include $(INCLUDE_DIR)/package.mk

SRC_DIR=./busybox-1.34.1

$(eval $(call BuildPackage,busybox))

romfs:
	$(MAKE) -C $(PKG_BUILD_DIR) \
		$(MAKE_FLAGS) \
		CONFIG_PREFIX=$(ROMFSDIR) \
		install
