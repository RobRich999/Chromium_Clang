**Chromium_Clang:**

The Chromium web browser for Windows and Linux built with the open source Clang compiler and LLD linker.

Additional features of the builds include modified compiler and linker optimizations via build configuration modifications.

Implementation of various options are subject to change depending upon performance, stability, and similar paramaters.

****

**Links to latest Linux build releases in deb package format:**

https://github.com/RobRich999/Chromium_Clang/releases/tag/v123.0.6269.0-r1253277-linux64-deb-avx2

https://github.com/RobRich999/Chromium_Clang/releases/tag/v123.0.6269.0-r1253277-linux64-deb-avx

https://github.com/RobRich999/Chromium_Clang/releases/tag/v123.0.6269.0-r1253277-linux64-deb-znver2

****

**Links to latest Windows build releases:**

https://github.com/RobRich999/Chromium_Clang/releases/tag/v123.0.6269.0-r1253277-win64-avx2

https://github.com/RobRich999/Chromium_Clang/releases/tag/v123.0.6269.0-r1253277-win64-avx

<sub>*Chromium_Clang for Windows builds are cross-compiled under Linux.*</sub>

****

**Links to discontinued, paused, etc. builds:**

n/a

****

**Optimization-related build tags:**

Builds marked with the "+fulllto" tag utilize whole-program analysis and cross-module optimization using "full" link time optimization.

Builds marked with the "+thinlto" tag utilize whole-program analysis and cross-module optimization using "thin" link time optimization.

Builds marked with the "+pgo" tag utilize profile-guided optimization.

Builds marked with the "+polly" tag utilize the Polly "high-level loop and data-locality optimizer and optimization infrastructure for LLVM."

Builds marked with the "+fast-math" tag utilize aggressive floating-point optimizations for various hot code paths.

Builds marked with the "+avx" tag require processors with AVX instruction set support.

Builds marked with the "+avx2" tag require processors with AVX2 instruction set support.

Builds marked with the "+amd_znver" tag are AVX2 builds tuned for the AMD Zen 2 processor microarchitecture.

Builds marked with the "+fma" tag require processors with FMA instruction set support.

Builds marked with the "+sse2" tag (deprecated) require processors with SSE2 instruction set support. AVX support is not required.

Builds marked with the "+sse3" tag (deprecated) require processors with SSE3 instruction set support. AVX support is not required.

*SSE3 support is the Chromium project's own minimum SIMD requirement on x86 platforms as of v89 builds.*

****

**Primary reason for AVX/AVX2 build recommendation:**

https://johnk.dev/blogs/generated/vex-transition-penalties.html


****

**Note regarding FFmpeg:**

Use the javascript patcher from here...

https://github.com/StaZhu/enable-chromium-hevc-hardware-decoding

...then proceed with the Chromium_Clang patches and build arguments.

****

**Note regarding LLVM:**

A Linux64 AVX2 optimized build script and resulting external binary builds of LLVM for building Chromium are available here:

https://github.com/RobRich999/LLVM_Optimized_AVX2

****

<sub>*Typical third-party build disclaimer. No warranties. No guarantees. Your mileage may vary. Use at your own risk.*</sub>
