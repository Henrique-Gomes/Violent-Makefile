# Violent-Makefile
This Makefile will compile everything inside a directory recursively (!) and generate the object files in a separated directory.

* No need to list all your code files
* No mess with object and code files together
* No slow compilation, since the object files will not be deleted

All you need to do is set the *SRCDIR* variable to the root directory of your source files

Also, you may have to set:

1. CC = gcc
   1. Your compiler
2. CFLAGS = -O3 -Wall
   1. Compiler flags
3. LDFLAGS = -lm
   1. Linker flags
4. EXTENSION=.c
   1. Extension of your source files
5. SRCDIR=src
   1. Root directory of your code
6. OBJDIR=obj
   1. Directory to drop the object files
7. EXECUTABLE = program
   1. Name of the executable output
