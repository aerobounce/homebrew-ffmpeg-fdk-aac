# homebrew-ffmpeg-fdk-aac
Default ffmpeg formula with fdk-aac.

# Changes from the original formula
This formula adds these arguments:

- `--enable-libfdk-aac`
- `--enable-nonfree`
- `--extra-cflags="-fno-stack-check"`

The last one is workaround for building on macOS Catalina: https://trac.ffmpeg.org/ticket/8073#comment:12

# Install
`brew install aerobounce/ffmpeg-fdk-aac/ffmpeg`

# Why
homebrew vanilla ffmpeg formula is missing `libfdk-aac` – 'highest-quality AAC encoder available with ffmpeg', due to license issues.

> The Fraunhofer FDK AAC codec library. This is currently the highest-quality AAC encoder available with ffmpeg. Requires ffmpeg to be configured with --enable-libfdk-aac (and additionally --enable-nonfree if you're also using --enable-gpl).

https://trac.ffmpeg.org/wiki/Encode/AAC
