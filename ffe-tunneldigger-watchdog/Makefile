include $(TOPDIR)/rules.mk

PKG_NAME:=ffe-tunneldigger-watchdog
PKG_VERSION:=3

PKG_BUILD_DIR := $(BUILD_DIR)/$(PKG_NAME)

include $(GLUONDIR)/include/package.mk

define Package/ffe-tunneldigger-watchdog
  SECTION:=gluon
  CATEGORY:=Gluon
  TITLE:=Automatically restarts tunneldigger if the client crashed
  DEPENDS:=+ffe-mesh-vpn-tunneldigger
endef

define Package/ffe-tunneldigger-watchdog/description
	Gluon community wifi mesh firmware framework: tunneldigger watchdog
endef

define Build/Prepare
	mkdir -p $(PKG_BUILD_DIR)
endef

define Build/Configure
endef

define Build/Compile
endef

define Package/ffe-tunneldigger-watchdog/install
	$(CP) ./files/* $(1)/
endef

define Package/ffe-tunneldigger-watchdog/postinst
endef

$(eval $(call BuildPackage,ffe-tunneldigger-watchdog))
