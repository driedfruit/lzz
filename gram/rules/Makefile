# package 
PACKAGE=gram
# current directory relative to top directory
SRCDIR=gram/parser
# subdirectories
SUBDIRS=
# include files
INCFILES=
# library lzz files
LIBLZZFILES=
# library source files
LIBCPPFILES=
# program lzz files
PRGLZZFILES=
# program source files
PRGCPPFILES=
# programs
PROGRAMS=
# common makefile
include $(PRJDIR)/maketools/Make.common
# parser
parser: run-parser gencode
# run parser
run-parser:
	time basil rules.txt -v -bc

