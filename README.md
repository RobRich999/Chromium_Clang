# Chromium_Clang

The Chromium web browser for Windows built with the open source Clang compiler and LLD linker.

Additional features of the build include modified compiler and linker optimizations via build configuration modifications.

Build marked withe "+fulllto" tag utilize whole-program analysis and cross-module optimization using "full" link time optimization.

Build marked withe "+thinlto" tag utilize whole-program analysis and cross-module optimization using "thin" link time optimization.

Builds marked with the "+pgo" tag utilize profile-guided optimization.

Builld marked with the "+polly" tag utilize the Polly "high-level loop and data-locality optimizer and optimization infrastructure for LLVM."

Builds marked with the "+avx" tag require processors with AVX instruction set support.

Builds marked with the "+avx2" tag require processors with AVX2 instruction set support.

Builds marked with the "+fma" tag require processors with FMA instruction set support.

Builds marked with the "+npm" tag utilize the LLVM "new pass manager" for building.

Implementation of various options are subject to change depending upon performance, stability, and similar paramaters.

Links to latest build releases:

https://github.com/RobRich999/Chromium_Clang/releases/tag/v80.0.3947.0-r707674-win64

https://github.com/RobRich999/Chromium_Clang/releases/tag/v80.0.3952.0-r709764-win32

Intel Haswell or later processors with AVX2, FMA, etc. instruction set support required for special AVX2 test build releases:

https://github.com/RobRich999/Chromium_Clang/releases/tag/v79.0.3943.0-r705874-win64-avx2
