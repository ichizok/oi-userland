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
#   $WS_TOOLS/python-integrate-project pylint
#

BUILD_STYLE = pyproject

include ../../../make-rules/shared-macros.mk

COMPONENT_NAME =		pylint
HUMAN_VERSION =			3.0.3
COMPONENT_SUMMARY =		pylint - python code static checker
COMPONENT_ARCHIVE_URL =		\
	https://github.com/pylint-dev/pylint/archive/refs/tags/v$(HUMAN_VERSION).tar.gz
COMPONENT_ARCHIVE_HASH =	\
	sha256:2880998fc9f3a53fab8989f373faba3f47a3097df0ff2e201ec286bdef0c3aa5
COMPONENT_LICENSE =		GPL-2.0-only
COMPONENT_LICENSE_FILE =	LICENSE

# Manifest options for developer/python/pylint package
COMPONENT_FMRI.pylint-meta =		developer/python/pylint

include $(WS_MAKE_RULES)/common.mk

# Auto-generated dependencies
PYTHON_REQUIRED_PACKAGES += library/python/astroid
PYTHON_REQUIRED_PACKAGES += library/python/dill
PYTHON_REQUIRED_PACKAGES += library/python/isort
PYTHON_REQUIRED_PACKAGES += library/python/mccabe
PYTHON_REQUIRED_PACKAGES += library/python/platformdirs
PYTHON_REQUIRED_PACKAGES += library/python/setuptools
PYTHON_REQUIRED_PACKAGES += library/python/tomli
PYTHON_REQUIRED_PACKAGES += library/python/tomlkit
PYTHON_REQUIRED_PACKAGES += library/python/typing-extensions
PYTHON_REQUIRED_PACKAGES += library/python/wheel
PYTHON_REQUIRED_PACKAGES += runtime/python
TEST_REQUIRED_PACKAGES.python += library/python/astroid
TEST_REQUIRED_PACKAGES.python += library/python/coverage
TEST_REQUIRED_PACKAGES.python += library/python/gitpython
TEST_REQUIRED_PACKAGES.python += library/python/pip
TEST_REQUIRED_PACKAGES.python += library/python/py
TEST_REQUIRED_PACKAGES.python += library/python/pytest
TEST_REQUIRED_PACKAGES.python += library/python/pytest-benchmark
TEST_REQUIRED_PACKAGES.python += library/python/pytest-cov
TEST_REQUIRED_PACKAGES.python += library/python/pytest-timeout
TEST_REQUIRED_PACKAGES.python += library/python/pytest-xdist
TEST_REQUIRED_PACKAGES.python += library/python/requests
TEST_REQUIRED_PACKAGES.python += library/python/setuptools
TEST_REQUIRED_PACKAGES.python += library/python/six
TEST_REQUIRED_PACKAGES.python += library/python/typing-extensions
