If anyone is using the LLVM build script, note I have made quite a few modifications.

//src/tools/clang/scripts/build.py

It works for building LLVM on Linux x64-64. No guarantees on other platforms and architectures, as I have not tested those options.

All builds are bootstrapped, so there is no need to pass the --bootstrap option. In fact it will now error.

LLVM is built with -march=native, Polly, and other optimizations. I have carried the optimizations down into the PGO, ThinLTO, and BOLT optimization options as well.

Building --without-android and --without-fuchsia now skips downloading the ARM sysroots. I set conditionals just in case those are needed, but YMMV since I did not test them. I do not target those platforms.

I added --x86-only to skip building LLVM support for various unneeded architectures.

I added --without-clang-extra to disable building extra clang tools. Again nothing I need for building Chromium.

Usage example:

vpython3 /home/robrich/depot_tools/chromium/src/tools/clang/scripts/build.py --without-android --without-fuchsia --disable-asserts --thinlto --pgo --bolt --llvm-force-head-revision --x86-only --without-clang-extra

The ThinLTO, PGO, and BOLT optimizations are optional. Even without them you will still get a LLVM build with optimizations for -O3, -march=native, Polly, extra LLVM loop passes, etc.

PGO and BOLT are not too bad on LLVM build times for a relatively fast system and/or lots of cores.

However ThinLTO can incur dramatically increased LLVM build times. I suggest plenty of fast cores and memory. It is annoying even on my 64-core build server.
