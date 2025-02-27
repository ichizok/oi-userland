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
# Copyright 2020 Aurelien Larcher
# Copyright 2023 Friedrich Kink
#

BUILD_BITS= 64
BUILD_STYLE= justmake
include ../../../make-rules/shared-macros.mk

COMPONENT_NAME=	ocamlbuild
COMPONENT_VERSION=	0.14.2
COMPONENT_SUMMARY=	ocamlbuild - OCaml build tool
COMPONENT_PROJECT_URL=	https://github.com/ocaml/ocamlbuild
COMPONENT_FMRI=	library/ocaml/ocamlbuild
COMPONENT_CLASSIFICATION= Development/Other Languages
COMPONENT_SRC=		$(COMPONENT_NAME)-$(COMPONENT_VERSION)
COMPONENT_ARCHIVE=	$(COMPONENT_NAME)-$(COMPONENT_VERSION).tar.gz
COMPONENT_ARCHIVE_URL=	https://github.com/ocaml/ocamlbuild/archive/$(COMPONENT_VERSION).tar.gz
COMPONENT_ARCHIVE_HASH=	sha256:62d2dab6037794c702a83ac584a7066d018cf1645370d1f3d5764c2b458791b1
COMPONENT_LICENSE= GPLv2

TEST_TARGET=$(NO_TESTS)
include $(WS_MAKE_RULES)/common.mk
include $(WS_MAKE_RULES)/ocaml.mk

PATH=$(PATH.gnu)

COMPONENT_PRE_CONFIGURE_ACTION  +=  $(CLONEY) $(SOURCE_DIR) $(@D) ;

COMPONENT_BUILD_ARGS+= PREFIX=$(USRDIR) MANDIR=$(USRSHAREMANDIR)
COMPONENT_INSTALL_ARGS+= CHECK_IF_PREINSTALLED=false

# Auto-generated dependencies
REQUIRED_PACKAGES += runtime/ocaml
REQUIRED_PACKAGES += system/library
REQUIRED_PACKAGES += system/library/math
