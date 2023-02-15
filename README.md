**Chromium_Clang:**

The Chromium web browser for Windows and Linux built with the open source Clang compiler and LLD linker.

Additional features of the builds include modified compiler and linker optimizations via build configuration modifications.

Implementation of various options are subject to change depending upon performance, stability, and similar paramaters.

****

**Links to latest Windows build releases:**

https://github.com/RobRich999/Chromium_Clang/releases/tag/v112.0.5598.0-r1105559-win64-avx2

https://github.com/RobRich999/Chromium_Clang/releases/tag/v111.0.5561.0-r1097176-win64-avx

****

**Links to latest Linux build releases in deb package format:**

https://github.com/RobRich999/Chromium_Clang/releases/tag/v112.0.5598.0-r1105559-linux64-deb-avx2

https://github.com/RobRich999/Chromium_Clang/releases/tag/v112.0.5598.0-r1105559-linux64-deb-avx

****

**Links to discontinued, paused, etc. builds:**

n/a

****

**Optimization-related build tags:**

Builds marked with the "+fulllto" tag utilize whole-program analysis and cross-module optimization using "full" link time optimization.

Builds marked with the "+thinlto" tag utilize whole-program analysis and cross-module optimization using "thin" link time optimization.

Builds marked with the "+pgo" tag utilize profile-guided optimization.

Builds marked with the "+polly" tag utilize the Polly "high-level loop and data-locality optimizer and optimization infrastructure for LLVM."

Builds marked with the "+avx" tag require processors with AVX instruction set support.

Builds marked with the "+avx2" tag require processors with AVX2 instruction set support.

Builds marked with the "+fma" tag require processors with FMA instruction set support.

Builds marked with the "+sse2" tag (deprecated) require processors with SSE2 instruction set support. AVX support is not required.

Builds marked with the "+sse3" tag (deprecated) require processors with SSE3 instruction set support. AVX support is not required.

*SSE3 support is the Chromium project's own minimum SIMD requirement on x86 platforms as of v89 builds.*

****

**Primary reason for AVX/AVX2 build recommendation:**

https://john-h-k.github.io/VexTransitionPenalties.html


****

<sub>*Typical third-party build disclaimer. No warranties. No guarantees. Your mileage may vary. Use at your own risk.*</sub>
