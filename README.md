# Chromium_Clang

The Chromium web browser for Windows built with the open source Clang compiler and LLD linker.

Builds starting at r499551 now feature whole-program analysis and cross-module optimization using ThinLTO link time optimization via build configuration modifications.

https://clang.llvm.org/docs/ThinLTO.html

Builds starting at r506010 now feature modified compiler optimizations via build configuration modifications.

Builds starting at r513698 could feature LLVM's new pass manager, NewGVN, and partial inlining as part of ongoing testing of build configuration modifications. The compiler notes will indicate which, if any of these features are enabled.

Builds start at r525689 feature Control Flow Integrity (CFI) exploit mitigtation enhancement.

https://clang.llvm.org/docs/ControlFlowIntegrity.html

Implementation of various compiler options are subject to change depending upon performance, code size, and similar paramaters.

Link to latest build release:

https://github.com/RobRich999/Chromium_Clang/releases/tag/v65.0.3301.0-r525689-win64
