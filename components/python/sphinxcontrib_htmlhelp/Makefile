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
#   $WS_TOOLS/python-integrate-project sphinxcontrib_htmlhelp
#

BUILD_STYLE = pyproject

include ../../../make-rules/shared-macros.mk

COMPONENT_NAME =		sphinxcontrib_htmlhelp
HUMAN_VERSION =			2.0.4
COMPONENT_SUMMARY =		sphinxcontrib_htmlhelp - sphinxcontrib-htmlhelp is a sphinx extension which renders HTML help files
COMPONENT_PROJECT_URL =		https://www.sphinx-doc.org/
COMPONENT_ARCHIVE_URL =		\
	https://files.pythonhosted.org/packages/fd/2d/abf5cd4cc1d5cd9842748b15a28295e4c4a927facfa8a0e173bd3f151bc5/sphinxcontrib_htmlhelp-2.0.4.tar.gz
COMPONENT_ARCHIVE_HASH =	\
	sha256:6c26a118a05b76000738429b724a0568dbde5b72391a688577da08f11891092a
COMPONENT_LICENSE =		BSD-2-Clause
COMPONENT_LICENSE_FILE =	LICENSE

#
# Following dependency loops were detected (where 'A --> B' means 'A needs B to
# run tests', and 'A ==> B' means 'A needs B for build and/or run'):
#
# sphinxcontrib_htmlhelp --> sphinx ==> sphinxcontrib_htmlhelp
#
# To break loops we need to allow this project to integrate without testing in
# a case the required projects are not available yet (bootstrap).
#
PYTHON_TEST_BOOTSTRAP = yes

include $(WS_MAKE_RULES)/common.mk

# Auto-generated dependencies
PYTHON_REQUIRED_PACKAGES += library/python/flit-core
PYTHON_REQUIRED_PACKAGES += library/python/sphinx
PYTHON_REQUIRED_PACKAGES += runtime/python
TEST_REQUIRED_PACKAGES.python += library/python/html5lib
TEST_REQUIRED_PACKAGES.python += library/python/pytest
TEST_REQUIRED_PACKAGES.python += library/python/sphinx
