##
## SPDX-License-Identifier: BSD-3-Clause
## Copyright Contributors to the OpenEXR Project.
##

## Process this file with automake to produce Makefile.in

pyexec_LTLIBRARIES = imathnumpy.la

imathnumpy_la_SOURCES = imathnumpymodule.cpp
imathnumpy_la_LDFLAGS = -avoid-version -module
imathnumpy_la_LIBADD  = $(top_builddir)/PyImath/libPyImath.la @BOOST_PYTHON_LIBS@

noinst_HEADERS = 

AM_CPPFLAGS = @ILMBASE_CXXFLAGS@      \
              @NUMPY_CXXFLAGS@        \
              -I$(top_srcdir)/PyImath \
	      -I$(top_builddir)       \
	      -I$(top_srcdir)/config
