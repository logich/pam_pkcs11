# $Id$

SUBDIRS = . po doc etc src tools
DIST_SUBDIRS = . po doc etc src tools

EXTRA_DIST = config.rpath ChangeLog COPYING INSTALL \
	NEWS README TODO bootstrap pam_pkcs11.spec ChangeLog.svn

MAINTAINERCLEANFILES = \
	Makefile.in config.h.in configure \
	install-sh ltmain.sh missing mkinstalldirs \
	compile depcomp config.log config.status \
	config.guess config.sub acinclude.m4 aclocal.m4

DEPCLEANFILES = config.log configure

AUTOMAKE_OPTIONS = foreign
ACLOCAL_AMFLAGS = -I aclocal

ChangeLog.svn:
	-svn2cl --group-by-day --stdout --include-rev > $@
