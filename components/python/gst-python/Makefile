#
# This file and its contents are supplied under the terms of the
# Common Development and Distribution License ("CDDL)". You may
# only use this file in accordance with the terms of the CDDL.
#
# A full copy of the text of the CDDL should have accompanied this
# source. A copy of the CDDL is also available via the Internet at
# http://www.illumos.org/license/CDDL.
#

#
# Copyright 2016 Alexander Pyhalov
# Copyright 2022-2023 Niklas Poslovski
#

BUILD_STYLE= meson

include ../../../make-rules/shared-macros.mk

COMPONENT_NAME=		gst-python
COMPONENT_VERSION=	1.22.7
COMPONENT_REVISION=	1
COMPONENT_SUMMARY=	Python bindings for the GStreamer streaming media framework
COMPONENT_PROJECT_URL=	https://gstreamer.freedesktop.org
COMPONENT_SRC=		$(COMPONENT_NAME)-$(COMPONENT_VERSION)
COMPONENT_ARCHIVE=	$(COMPONENT_SRC).tar.xz
COMPONENT_ARCHIVE_HASH= sha256:1ef8df7608012fa469329799c950ec087737a6dabad3003c230658b58c710172
COMPONENT_ARCHIVE_URL=	$(COMPONENT_PROJECT_URL)/src/$(COMPONENT_NAME)/$(COMPONENT_ARCHIVE)
COMPONENT_SIG_URL=	$(COMPONENT_ARCHIVE_URL).asc
COMPONENT_CLASSIFICATION= Development/Python
COMPONENT_FMRI=	library/python/python-gst
COMPONENT_LICENSE=	LGPL v2.1
COMPONENT_LICENSE_FILE=	COPYING

include $(WS_MAKE_RULES)/common.mk

CONFIGURE_OPTIONS += -Dpygi-overrides-dir=$(PYTHON_VENDOR_PACKAGES)/gi/overrides

# for the tests
unexport SHELLOPTS

# As test results keep only everything between the lines containing Ok: and Timeout:
COMPONENT_TEST_TRANSFORMS += \
	'-n ' \
	'-e "/^Ok:/,/^Timeout:/p" '

# Build dependencies
PYTHON_REQUIRED_PACKAGES += library/python/pygobject-3

# Auto-generated dependencies
PYTHON_REQUIRED_PACKAGES += runtime/python
REQUIRED_PACKAGES += library/audio/gstreamer1
REQUIRED_PACKAGES += library/glib2
REQUIRED_PACKAGES += system/library
