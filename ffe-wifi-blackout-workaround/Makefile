include $(TOPDIR)/rules.mk

PKG_NAME:=ffe-wifi-blackout-workaround
PKG_VERSION:=2
PKG_RELEASE:=$(GLUON_VERSION).$(GLUON_SITE_CODE)-$(GLUON_RELEASE).$(GLUON_CONFIG_VERSION)

PKG_BUILD_DIR := $(BUILD_DIR)/$(PKG_NAME)

include $(INCLUDE_DIR)/package.mk

define Package/ffe-wifi-blackout-workaround
  SECTION:=ffe
  CATEGORY:=Workarounds
  TITLE:=WiFi-Blackout workaround
  DEPENDS:=+gluon-core
  MAINTAINER:=Freifunk Essen <kontakt@freifunk-essen.de>
  URL:=https://github.com/FFEssen/packages
endef

define Package/ffe-wifi-blackout-workaround/description
	Disables the ANI feature.
endef

define Build/Prepare
	mkdir -p $(PKG_BUILD_DIR)
endef

define Build/Configure
endef

define Build/Compile
endef

define Package/ffe-wifi-blackout-workaround/install
	$(CP) ./files/* $(1)/
endef

$(eval $(call BuildPackage,ffe-wifi-blackout-workaround))
