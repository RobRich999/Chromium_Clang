Chromium_Clang for Linux builds are currently compiled under CachyOS via a Ubuntu Server 24.04 LTS (Noble Numbat) chroot.

https://chromium.googlesource.com/chromium/src/+/refs/heads/main/docs/linux/build_instructions.md

Add the --unsupported option when using the build depedency script on Ubuntu 24.04 at this time.

/build/install-build-deps.sh --unsupported

Additional options listed in script:

https://chromium.googlesource.com/chromium/src/+/refs/heads/main/build/install-build-deps.sh
