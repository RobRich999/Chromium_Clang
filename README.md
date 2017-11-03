# Chromium_Clang

The Chromium web browser for Windows built with the open source Clang compiler and LLD linker.

Builds starting at r499551 now feature whole-program analysis, cross-module optimization, and "full_wpo_on_official" building using ThinLTO link time optimization via build configuration modifications.

https://clang.llvm.org/docs/ThinLTO.html

Builds starting at r506010 now feature modified compiler optimizations via build configuration modifications.

Builds starting at rr513698 now feature LLVM's new pass maanager, NewGVN, and partial inlining features.

Link to latest build release:

https://github.com/RobRich999/Chromium_Clang/releases/tag/v64.0.3258.0-r513698-win64
