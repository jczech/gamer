## ###########################################################################
## File:    Makefile.am
##
## Purpose: Automatically generate Makefile.in for autoconf using automake.
##
## Notes:   The final makefile produced by autoconf will use the following:
##
##     COMPILE = $(CC) $(DEFS) $(INCLUDES) $(CPPFLAGS) $(CFLAGS)
##     LINK = $(CC) $(CFLAGS) $(LDFLAGS) -o $@
##
## Author:  Michael Holst
## ###########################################################################

AUTOMAKE_OPTIONS = no-dependencies
SUFFIXES = .y .l .H .h .m .cpp .C .cc .c .f .java .o
always_built_SUBDIRS =
SUBDIRS = $(always_built_SUBDIRS) .
THISLIB = triangle

noinst_LTLIBRARIES = libtriangle.la
libtriangle_la_SOURCES = triangle.c
INCLUDES           = @maloc_inc@
AM_CFLAGS          = @profile@ @wall_pedantic_ansi@

all-local:
	-cp -p ${top_srcdir}/src/${THISLIB}/gamer/*.h ../aaa_inc/gamer/.

