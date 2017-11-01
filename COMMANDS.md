    slurp [directory or git URL] - adds the source code found in the given directory or git repo URL
    slurp o [output .o filename] [list of source files] - generate an .o file
    slurp cc gcc [GCC flags and arguments] - compile the given flags and arguments with GCC, but fetch the source file from the database and pass to gcc over stdin
    slurp cc clang [CLANG flags and arguments] - same as "cc gcc", but for CLANG
    slurp exe [output filename] [list of o files or source files] - output an executable given a list of .o files or source files
    slurp cmake [directory name] - same as using cmake, but extracts the directory from the database and then gives that path to cmake
    slurp configure_make [directory name] [environment variables] [configure flags] [make flags] - same as using ./configure and make, but extracts the directory from the database and then enters that path, sets environment variables, runs configure with those flags and then runs make with those flags
    slurp sed [sed script] [filename] - runs a sed script on the given database filename, in order to change that file
    slurp setconf [args] [filename] - runs setconf on a file in the database, in order to change that file
    slurp add [filename] - adds a file
    slurp cat [filenane] - outputs a file

* C source files are as filenames ( functions, defines, variables, macros, guards, comments etc).
* All added, modified or removed source code is being used to update an index over all functions)
* FFI is generated automatically with SWIG in order to be able to call as many functions from as many languages as possible.
* There must be per-language plugins for supporting languages.

Compiling C, C++ and Go is a good start.
