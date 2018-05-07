# Chromium_Clang

The Chromium web browser for Windows built with the open source Clang compiler and LLD linker and now using the Polly "high-level loop and data-locality optimizer" for LLVM, starting with build revision 551871.

About polyhedral optimization in general:

http://polyhedral.info/

About the Polly optimizer:

http://polly.llvm.org/

Additional features of the build include modified compiler optimizations including whole-program analysis and cross-module optimization using "full" link time optimization (LTO) via build configuration modifications.

Implementation of various options are subject to change depending upon performance, stability, and similar paramaters.

Link to latest build release:

https://github.com/RobRich999/Chromium_Clang/releases/tag/v68.0.3424.0-r556381-win64
