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
# Copyright 2014 Josef 'Jeff' Sipek <jeffpc@josefsipek.net>
#

include ../../../make-rules/shared-macros.mk

COMPONENT_NAME=		puri
COMPONENT_VERSION=	1.5.7
COMPONENT_PROJECT_URL=	http://puri.kpe.io/
COMPONENT_FMRI=		library/common-lisp/puri
COMPONENT_CLASSIFICATION=Development/Other Languages
COMPONENT_SRC=		$(COMPONENT_NAME)-$(COMPONENT_VERSION)
COMPONENT_ARCHIVE=	$(COMPONENT_SRC).tar.gz
COMPONENT_ARCHIVE_HASH=	\
	sha256:abd6497b05b63c4f8ea69f3672c706078abf3617e3cb38823606eb1dee3e41be
COMPONENT_ARCHIVE_URL=	http://files.kpe.io/puri/$(COMPONENT_ARCHIVE)
COMPONENT_LICENSE=	LLGPL
COMPONENT_LICENSE_FILE=	$(COMPONENT_NAME).license
COMPONENT_SUMMARY=	Puri provides a Common Lisp library for manipulating Universal Resource Identifiers

include ../../../make-rules/prep.mk
include ../../../make-rules/common-lisp.mk
include ../../../make-rules/ips.mk

build:		$(BUILD_32)

install:	$(INSTALL_32)
