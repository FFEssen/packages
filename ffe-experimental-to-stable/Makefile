include $(TOPDIR)/rules.mk

PKG_NAME:=ffe-experimental-to-stable
PKG_VERSION:=1
PKG_RELEASE:=1

PKG_BUILD_DIR := $(BUILD_DIR)/$(PKG_NAME)

include $(INCLUDE_DIR)/package.mk

define Package/ffe-experimental-to-stable
  SECTION:=ffe
  CATEGORY:=FFE
  TITLE:=Switches branch to stable.
  DEPENDS:=+gluon-core
  MAINTAINER:=Freifunk Essen <kontakt@freifunk-essen.de>
  URL:=https://github.com/ffessen/packages
endef

define Package/ffe-experimental-to-stable/description
	Switches branch to stable, if current image is experimental.
endef

define Build/Prepare
	mkdir -p $(PKG_BUILD_DIR)
endef

define Build/Configure
endef

define Build/Compile
endef

define Package/ffe-experimental-to-stable/install
	$(CP) ./files/* $(1)/
endef

$(eval $(call BuildPackage,ffe-experimental-to-stable))
