# Chromium_Clang

The Chromium web browser for Windows built with the open source Clang compiler and LLD linker.

Additional features of the build include modified compiler optimizations, including profile-guided optimization of performance-targeted code paths, plus whole-program analysis and cross-module optimization using "thin" link time optimization (ThinLTO), via build configuration modifications. A processor with AVX support is required.

Builds marked with the "+npm" tag utilize the LLVM "new pass manager" for building.

Implementation of various options are subject to change depending upon performance, stability, and similar paramaters.

Links to latest build releases:

https://github.com/RobRich999/Chromium_Clang/releases/tag/v73.0.3660.0-r619562-win64

https://github.com/RobRich999/Chromium_Clang/releases/tag/v73.0.3651.0-r618847-win32
