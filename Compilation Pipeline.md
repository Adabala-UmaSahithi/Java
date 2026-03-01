Compilation Pipeline:

1. Preprocessing:

Performs text-level manipulation before actual compilation begins

* file inclusion: Includes the contents of specified header files 
* macro expansion: It replaces macro names(#define) with actual code
* Comment removal: Removes all comments and replaces them with single space

2\.	Compilation:

Compiler converts the above preprocessed file into assembly language i.e human readable conversion to low-level CPU instructions

* Analysis: lexical analysis(tokenization), syntax checking(parsing), semantic analysis(checking for logic/type errors)
* Optimization: rearranging code to make it faster or smaller by techniques like unrolling or dead code elimination
* Result: assembly file specific to target CPU architecture

3\.	Assembly:

converts assembly code to machine code

* Object Files: Produces object file(.o or .obj)
* Status: These files contain machine instructions, but they are not yet runnable because they might refer to functions (like printf) defined in other files

4\. Linking:

Stitches everything together into a single, functional program

* Symbol Resolution: matches functional calls in your object files to their actual definitions in another obj files
* Startup Code: It adds essential "boilerplate" code required by os to start and stop the program
* Result: final executable file(.exe file)

"Boilerplate code" : sections of code to be included in many places with little or no alteration to achieve minimal functionality

ex : public static void main(String args\[]),getters,setters,<!DOCTYPE  html>,<html>....

