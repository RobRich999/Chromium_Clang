Apply the patch from the /chromium/src directory to modify the LLVM build script.

git apply /path/to/llvm.patch

The modified script builds LLVM on Linux x64-64. Other architectures and platforms have not been tested.

All builds are bootstrapped. There is no need to pass the --bootstrap option, which will now error.

LLVM is built with -march=native, Polly, and other optimizations. Optimizations have beeb carried down into the PGO, ThinLTO, and BOLT build options.

Using --without-android and --without-fuchsia now skips downloading the ARM sysroots. The options have not otherwise been tested.

I added --x86-only to skip building LLVM support for various other architectures. The options have not otherwise been tested.

Use --without-clang-extra to disable building extra clang tools. These are not required for my release builds. YMMV for other build types.

Usage example from the /chromium/src directory:

vpython3 tools/clang/scripts/build.py --without-android --without-fuchsia --disable-asserts --thinlto --pgo --bolt --llvm-force-head-revision --x86-only --without-clang-extra

Building LLVM with ThinLTO, PGO, and BOLT optimizations are optional. Regardless LLLVM still builds with optimizations for -O3, -march=native, Polly, extra LLVM loop passes, etc. PGO and BOLT are not too LLVM build time intensive for a relatively fast system and/or lots of cores. ThinLTO can incur dramatically increased LLVVM build times, even on my 64-core build server.
