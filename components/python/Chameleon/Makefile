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
#   $WS_TOOLS/python-integrate-project Chameleon
#

BUILD_STYLE = setup.py

include ../../../make-rules/shared-macros.mk

COMPONENT_NAME =		Chameleon
HUMAN_VERSION =			4.3.0
COMPONENT_SUMMARY =		Chameleon - Fast HTML/XML Template Compiler.
COMPONENT_PROJECT_URL =		https://chameleon.readthedocs.io
COMPONENT_ARCHIVE_URL =		\
	https://files.pythonhosted.org/packages/0a/c7/bf24207ad79a383c8105df50f5d32e075a97fb30a85e1123810ac2326ad8/Chameleon-4.3.0.tar.gz
COMPONENT_ARCHIVE_HASH =	\
	sha256:5105991bc4f69f4f4061af5318528a6953c0427a30d7cde4cb9d94405f1aac23
COMPONENT_LICENSE =		BSD-3-Clause OR PSF-2.0
COMPONENT_LICENSE_FILE =	LICENSE.txt

include $(WS_MAKE_RULES)/common.mk

# Force no colors and more verbose output via tox posargs
COMPONENT_TEST_TARGETS += -- -vv

# Normalize timetstamps that change with every run
COMPONENT_TEST_TRANSFORMS += "-e 's|\[../../.. ..:..:..\]|[XX/XX/XX XX:XX:XX]|'"

# Auto-generated dependencies
PYTHON_REQUIRED_PACKAGES += library/python/importlib-metadata
PYTHON_REQUIRED_PACKAGES += runtime/python
TEST_REQUIRED_PACKAGES.python += library/python/build
TEST_REQUIRED_PACKAGES.python += library/python/wheel
TEST_REQUIRED_PACKAGES.python += library/python/zope-testrunner
