GO_EASY_ON_ME=1

include $(THEOS)/makefiles/common.mk

BUNDLE_NAME = CustomSiri
CustomSiri_FILES = CTSRootListController.m
CustomSiri_INSTALL_PATH = /Library/PreferenceBundles
CustomSiri_FRAMEWORKS = UIKit
CustomSiri_PRIVATE_FRAMEWORKS = Preferences
CustomSiri_CFLAGS = -fobjc-arc

include $(THEOS_MAKE_PATH)/bundle.mk

internal-stage::
	$(ECHO_NOTHING)mkdir -p $(THEOS_STAGING_DIR)/Library/PreferenceLoader/Preferences$(ECHO_END)
	$(ECHO_NOTHING)cp entry.plist $(THEOS_STAGING_DIR)/Library/PreferenceLoader/Preferences/CustomSiri.plist$(ECHO_END)
