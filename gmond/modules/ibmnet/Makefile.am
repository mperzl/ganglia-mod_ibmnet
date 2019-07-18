AM_CFLAGS  = -I$(top_builddir)/include -I$(top_builddir)/lib -I$(top_builddir)/libmetrics

if STATIC_BUILD
noinst_LTLIBRARIES    = libmodibmnet.la
libmodibmnet_la_SOURCES = mod_ibmnet.c 
else
pkglib_LTLIBRARIES    = modibmnet.la
modibmnet_la_SOURCES = mod_ibmnet.c 
modibmnet_la_LDFLAGS = -module -avoid-version
modibmnet_la_LIBADD = $(top_builddir)/libmetrics/libmetrics.la

EXTRA_DIST = ../conf.d/ibmnet.conf
endif

INCLUDES = @APR_INCLUDES@

