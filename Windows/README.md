Chromium_Clang for Windows builds are cross-compiled under Linux; currently Ubuntu Server 24.04 LTS (Noble Numbat).

https://chromium.googlesource.com/chromium/src/+/master/docs/win_cross.md

The diff patches should work for native Chromium for Windows builds, though they are untested so "your mileage my vary."

Note the win64-avx512.patch currently cross-compiles Windows AVX-512 core browser binaries on a Linux AVX2-class build server.
