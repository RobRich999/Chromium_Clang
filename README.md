# Chromium_Clang

The Chromium web browser for Windows built with the open source Clang compiler and LLD linker.

Builds starting at r499551 now feature whole-program analysis and cross-module optimization using ThinLTO link time optimization via build configuration modifications.

https://clang.llvm.org/docs/ThinLTO.html

Builds starting at r506010 now feature modified compiler optimizations via build configuration modifications.

https://github.com/RobRich999/Chromium_Clang/releases/tag/v66.0.3354.0-r538960-win64ing testing of build configuration modifications. The compiler notes will indicate which, if any of these features are enabled.

Builds starting at r530764 now feature increased inline expansion optimization of select code targets.

Implementation of various options are subject to change depending upon performance, stability, and similar paramaters.

Link to latest build release:

https://github.com/RobRich999/Chromium_Clang/releases/tag/v66.0.3354.0-r538960-win64
