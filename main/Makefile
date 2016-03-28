# package 
PACKAGE=
# current directory relative to top directory
SRCDIR=main
# subdirectories
SUBDIRS=
# include files
INCFILES=
# library lzz files
LIBLZZFILES=
# library source files
LIBCPPFILES=
# program lzz files
PRGLZZFILES=$(wildcard *.lzz)
# program source files
PRGCPPFILES=
# programs
PROGRAMS=$(BUILD_LZZ)
# common makefile
include $(PRJDIR)/maketools/Make.common

# program libraries
PRGLIBS=smtc gram smtc gram basl msg conf util
# program library base files 
PRGLIBFILES=$(addprefix $(LIBDIR)/,$(patsubst %,lib%.a,$(PRGLIBS)))
# program link options
PRGLINKFLAGS=$(LINKOPTIONS) -L$(LIBDIR) $(addprefix -l, $(PRGLIBS))

# make basilsim
$(BUILD_LZZ): $(PRGOBJFILES) $(PRGLIBFILES)
	$(CXX) $(PRGOBJFILES) $(PRGLINKFLAGS) -o $@
ifeq ($(DEBUG_BUILD),)
	$(STRIP) $@
endif
