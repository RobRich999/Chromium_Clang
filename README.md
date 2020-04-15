# Chromium_Clang

The Chromium web browser for Windows built with the open source Clang compiler and LLD linker.

Additional features of the build include modified compiler and linker optimizations via build configuration modifications.

Build marked withe "+fulllto" tag utilize whole-program analysis and cross-module optimization using "full" link time optimization.

Build marked withe "+thinlto" tag utilize whole-program analysis and cross-module optimization using "thin" link time optimization.

Builds marked with the "+npm" tag utilize the LLVM "new pass manager" for building.

Builds marked with the "+pgo" tag utilize profile-guided optimization.

Builld marked with the "+polly" tag utilize the Polly "high-level loop and data-locality optimizer and optimization infrastructure for LLVM."

Builds marked with the "+avx" tag require processors with AVX instruction set support.

Builds marked with the "+avx2" tag require processors with AVX2 instruction set support.

Builds marked with the "+fma" tag require processors with FMA instruction set support.

Builds marked with the "+sse2" tag require processors with SSE2 instruction set support. AVX support is not required.

Implementation of various options are subject to change depending upon performance, stability, and similar paramaters.

Links to latest build releases:

https://github.com/RobRich999/Chromium_Clang/releases/tag/v84.0.4116.0-r759268-win64 (avx | Win64 recommended)

https://github.com/RobRich999/Chromium_Clang/releases/tag/v83.0.4102.0-r755245-win64-sse2 (sse2 | Win64 legacy)

https://github.com/RobRich999/Chromium_Clang/releases/tag/v83.0.4102.0-r755245-win32 (sse2 | Win32 legacy)

Intel Haswell or later processors with AVX2, FMA, etc. instruction set support required for special AVX2 build releases:

https://github.com/RobRich999/Chromium_Clang/releases/tag/v83.0.4102.0-r755616-win64-avx2 (avx2+fma | Win64 experimental)
