include $(TOPDIR)/rules.mk

PKG_NAME:=OLED
PKG_RELEASE:=1

PKG_BUILD_DIR:=$(BUILD_DIR)/$(PKG_NAME)

include $(INCLUDE_DIR)/package.mk


define Package/OLED
	SECTION:=utils
	CATEGORY:=Utilities
	TITLE:=OLED
endef

define Build/Prepare
	mkdir -p $(PKG_BUILD_DIR)
	$(CP) ./src/* $(PKG_BUILD_DIR)/
endef

define Package/OLED/install
	$(INSTALL_DIR) $(1)/bin
	$(INSTALL_BIN) $(PKG_BUILD_DIR)/OLED $(1)/bin/
endef

$(eval $(call BuildPackage,OLED))
