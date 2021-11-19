export SDKVERSION=13.7
DEBUG = no
ARCHS = arm64 arm64e
TARGET := iphone:clang:latest:7.0
INSTALL_TARGET_PROCESSES = Springboard


include $(THEOS)/makefiles/common.mk

TWEAK_NAME = NoDock

NoDock_FILES = Tweak.x
NoDock_CFLAGS = -fobjc-arc

include $(THEOS_MAKE_PATH)/tweak.mk


after-install::

	install.exec "sbreload"