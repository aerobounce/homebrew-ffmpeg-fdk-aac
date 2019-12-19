# homebrew-ffmpeg-fdk-aac
Default ffmpeg formula with fdk-aac.

# Install
```
brew install aerobounce/ffmpeg-fdk-aac/ffmpeg
```

# Changes from the original Formula
This formula adds these arguments:

```
--enable-libfdk-aac
--enable-nonfree
--disable-htmlpages
-fno-stack-check
```

`fno-stack-check` is a bug workaround when building with newer toolchains on macOS: https://trac.ffmpeg.org/ticket/8073#comment:12


# Why
homebrew-core ffmpeg Formula removed all the options and is missing `libfdk-aac` – "highest-quality AAC encoder available with ffmpeg".

> The Fraunhofer FDK AAC codec library. This is currently the highest-quality AAC encoder available with ffmpeg. Requires ffmpeg to be configured with --enable-libfdk-aac (and additionally --enable-nonfree if you're also using --enable-gpl).

https://trac.ffmpeg.org/wiki/Encode/AAC
