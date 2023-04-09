For now apply hdr10-metadata-chromium-114.patch to a checkout of the "enable-chromium-hevc-hardware-decoding" repository...

https://github.com/StaZhu/enable-chromium-hevc-hardware-decoding

...to comply with the below FFmpeg commit.

https://github.com/FFmpeg/FFmpeg/commit/6f2413a203c7dced3230f82cbc2c053872c1a713

The issue has been reported pending future "enable-chromium-hevc-hardware-decoding" updates.

https://github.com/StaZhu/enable-chromium-hevc-hardware-decoding/issues/50

Use the patched add-hevc-ffmpeg-decoder-parser.js script within the chromium/src/third_party/ffmpeg directory.

node /path/to/add-hevc-ffmpeg-decoder-parser.js

Proceed with Chromium_Clang patches and related build arguments as usual.
