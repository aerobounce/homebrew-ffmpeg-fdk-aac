# homebrew-ffmpeg-fdk-aac
Default ffmpeg formula with fdk-aac.

# Changes from the original formula
This formula adds `--enable-libfdk-aac` and `--enable-nonfree` args.

# Why
homebrew vanilla ffmpeg formula is missing `libfdk-aac` due to license issues.

> The Fraunhofer FDK AAC codec library. This is currently the highest-quality AAC encoder available with ffmpeg. Requires ffmpeg to be configured with --enable-libfdk-aac (and additionally --enable-nonfree if you're also using --enable-gpl).

https://trac.ffmpeg.org/wiki/Encode/AAC
