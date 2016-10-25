include $(TOPDIR)/rules.mk

PKG_NAME:=ffe-autoupdater-wifi-fallback
PKG_VERSION:=2
PKG_RELEASE:=$(GLUON_VERSION).$(GLUON_SITE_CODE)-$(GLUON_RELEASE).$(GLUON_CONFIG_VERSION)

PKG_BUILD_DIR := $(BUILD_DIR)/$(PKG_NAME)

include $(GLUONDIR)/include/package.mk

define Package/ffe-autoupdater-wifi-fallback
  SECTION:=ffe
  CATEGORY:=FFE
  TITLE:=Implements switching to fallback mode if we are cut off from the mesh
  DEPENDS:=+gluon-autoupdater +libiwinfo-lua +iw
  MAINTAINER:=Freifunk Essen <kontakt@freifunk-essen.de>
  URL:=https://github.com/ffessen/packages
endef

define Build/Prepare
	mkdir -p $(PKG_BUILD_DIR)
endef

define Build/Configure
endef

define Build/Compile
endef

define Package/ffe-autoupdater-wifi-fallback/install
	$(CP) ./files/* $(1)/
endef

$(eval $(call BuildPackage,ffe-autoupdater-wifi-fallback))
