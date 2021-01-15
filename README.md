# Violent-Makefile
This Makefile will compile everything inside a directory recursively (!) and generate the object files in a separated directory.

* No need to list all your code files
* No mess with object and code files together
* No slow compilation, since the object files will not be deleted

All you need to do is set the *SRCDIR* variable to the root directory of your source files

Also, you may need to set:

1. CC
   1. Your compiler
2. CFLAGS
   1. Compiler flags
3. LDFLAGS
   1. Linker flags
4. EXTENSION
   1. Extension of your source files
5. SRCDIR
   1. Root directory of your code
6. OBJDIR
   1. Directory to drop the object files
7. EXECUTABLE
   1. Name of the executable output

You can use SRCDIR to make different builds. Per example:

    release: SRCDIR = release
    release: all
   
    debug: SCRDIR = debug
    debug: all
    
    i386: SRCDIR = i386
    i386: all
    
Also, you can stop using this kind of macgyverism.
