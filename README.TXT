Here's how to build Lzz:

  Source one of the following files to setup your environment.  You
  can choose to build a debug or an optimized version. 

    setup_gcc_debug.env
    setup_gcc_opt.env

  Then type 'make'.  This build requires lzz, so make sure you have 'lzz'
  in your path!  So the first time you'll have to download a binary.
  
When make finishes the executable will be in $CONFIGDIR ("gcc.opt" or
"gcc.debug").  The objects, libraries and executable are all under
$CONFIGDIR, so you can build both an optimized and a debug version.

Enjoy!
