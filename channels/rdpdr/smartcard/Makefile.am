## Process this file with automake to produce Makefile.in

# scard
scarddir = $(PLUGIN_PATH)

scard_LTLIBRARIES = scard.la

scard_la_SOURCES = \
	scard_main.c scard_main.h \
	scard_queue.c scard_queue.h \
	scard_operations.c

scard_la_CFLAGS = \
	-I$(srcdir)/.. \
	@PCSCLITE_CFLAGS@ \
	-I$(top_srcdir)/include \
	-I$(srcdir)/../../common \
	-I$(top_srcdir)/libfreerdp-core \
	-DPLUGIN_PATH=\"$(PLUGIN_PATH)\"

scard_la_LDFLAGS = -avoid-version -module

scard_la_LIBADD = \
	@PCSCLITE_LIBS@ \
	../../../libfreerdp-utils/libfreerdp-utils.la

# extra
EXTRA_DIST =

DISTCLEANFILES =
