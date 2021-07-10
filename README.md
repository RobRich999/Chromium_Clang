# Chromium_Clang

The Chromium web browser for Windows and Linux built with the open source Clang compiler and LLD linker.

Additional features of the build include modified compiler and linker optimizations via build configuration modifications.

Build marked with the "+fulllto" tag utilize whole-program analysis and cross-module optimization using "full" link time optimization.

Build marked with the "+thinlto" tag utilize whole-program analysis and cross-module optimization using "thin" link time optimization.

Builds marked with the "+pgo" tag utilize profile-guided optimization.

Builld marked with the "+polly" tag utilize the Polly "high-level loop and data-locality optimizer and optimization infrastructure for LLVM."

Builds marked with the "+avx" tag require processors with AVX instruction set support.

Builds marked with the "+avx2" tag require processors with AVX2 instruction set support.

Builds marked with the "+fma" tag require processors with FMA instruction set support.

Builds marked with the "+sse2" tag require processors with SSE2 instruction set support. AVX support is not required.

Builds marked with the "+sse3" tag require processors with SSE3 instruction set support. AVX support is not required.

*SSE3 support is the Chromium project's own minimum SIMD requirement on x86 platforms as of v89 builds.*

Implementation of various options are subject to change depending upon performance, stability, and similar paramaters.

Links to latest Windows build releases:

https://github.com/RobRich999/Chromium_Clang/releases/tag/v93.0.4571.0-r900242-win64-avx (Win64 recommended)

https://github.com/RobRich999/Chromium_Clang/releases/tag/v93.0.4571.0-r900242-win64-sse3 (Win64 legacy)

https://github.com/RobRich999/Chromium_Clang/releases/tag/v93.0.4557.0-r896373-win32-sse3 (Win32 legacy)

Intel Haswell or later processors with AVX2, FMA, etc. instruction set support required for special Windows AVX2 build releases:

https://github.com/RobRich999/Chromium_Clang/releases/tag/v93.0.4571.0-r900242-win64-avx2 (Win64 experimental)

Links to latest Linux build releases in deb package format:

https://github.com/RobRich999/Chromium_Clang/releases/tag/v93.0.4571.0-r900242-linux64-deb-avx (Linux 64 recommended)

https://github.com/RobRich999/Chromium_Clang/releases/tag/v93.0.4558.0-r896600-linux64-deb-sse3 (Linux 64 legacy)
