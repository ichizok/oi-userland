#
# This file and its contents are supplied under the terms of the
# Common Development and Distribution License ("CDDL"). You may
# only use this file in accordance with the terms of the CDDL.
#
# A full copy of the text of the CDDL should have accompanied this
# source. A copy of the CDDL is also available via the Internet at
# http://www.illumos.org/license/CDDL.
#

#
# Copyright 2021 Alexander Pyhalov
#

BUILD_BITS=32
BUILD_STYLE=gem

include ../../../make-rules/shared-macros.mk

COMPONENT_NAME=		tomlrb
COMPONENT_VERSION=	2.0.1
COMPONENT_SUMMARY=	A Racc based TOML Ruby parser
COMPONENT_SRC=		$(COMPONENT_NAME)-$(COMPONENT_VERSION)
COMPONENT_ARCHIVE=	$(COMPONENT_SRC).gem
COMPONENT_ARCHIVE_HASH=	\
    sha256:4fcc546118fa73a556f2d8d9a4a121fa0cfc7a99d990168ac9f4fbdbcb620329
COMPONENT_ARCHIVE_URL=  https://rubygems.org/downloads/$(COMPONENT_ARCHIVE)
COMPONENT_PROJECT_URL=  https://github.com/fbernier/tomlrb
COMPONENT_FMRI=		library/ruby/tomlrb
COMPONENT_CLASSIFICATION=	Development/Ruby
COMPONENT_LICENSE=	MIT
COMPONENT_LICENSE_FILE=	LICENSE.txt

TEST_TARGET=		$(NO_TESTS)
include $(WS_MAKE_RULES)/common.mk

# No gemspec is shipped with the gem. Create one
COMPONENT_POST_UNPACK_ACTION= \
	$(GEM) spec $(USERLAND_ARCHIVES)/$(COMPONENT_ARCHIVE) --ruby > $(SOURCE_DIR)/$(GEMSPEC)

REQUIRED_PACKAGES += runtime/ruby-23
