#
# This file and its contents are supplied under the terms of the
# Common Development and Distribution License ("CDDL"), version 1.0.
# You may only use this file in accordance with the terms of version
# 1.0 of the CDDL.
#
# A full copy of the text of the CDDL should have accompanied this
# source.  A copy of the CDDL is also available via the Internet at
# http://www.illumos.org/license/CDDL.
#

#
# This file was automatically generated using the following command:
#   $WS_TOOLS/python-integrate-project ansible
#

BUILD_STYLE = pyproject

include ../../../make-rules/shared-macros.mk

COMPONENT_NAME =		ansible
HUMAN_VERSION =			8.6.1
COMPONENT_SUMMARY =		ansible - Radically simple IT automation
COMPONENT_PROJECT_URL =		https://ansible.com/
COMPONENT_ARCHIVE_URL =		\
	https://files.pythonhosted.org/packages/f9/41/714d5a1e4d46e522df144b6745fa2002760114fd586eea8538b6e42be26c/ansible-8.6.1.tar.gz
COMPONENT_ARCHIVE_HASH =	\
	sha256:18b397580c1f05ce5de1fe238508dd81218d278667956d2f7709320176c3ed4a
COMPONENT_LICENSE =		GPL-3.0-only
COMPONENT_LICENSE_FILE =	COPYING

COMPONENT_FMRI =		system/management/ansible
COMPONENT_CLASSIFICATION =	System/Administration and Configuration

# This project is a collection of other projects (see tags.yaml), each with its
# own test requirements.  We do not support testing of that (yet).
TEST_STYLE = none

# This is a standalone application.  Since no other Python project depends on
# it we just provide single unversioned package.
SINGLE_PYTHON_VERSION = yes

include $(WS_MAKE_RULES)/common.mk

# Auto-generated dependencies
PYTHON_REQUIRED_PACKAGES += library/python/ansible-core
PYTHON_REQUIRED_PACKAGES += library/python/setuptools
PYTHON_REQUIRED_PACKAGES += library/python/wheel
PYTHON_REQUIRED_PACKAGES += runtime/python
