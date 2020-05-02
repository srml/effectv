# EffecTV

This is the last release of EffecTV from https://www.effectv.dev/ with the necessary changes to compile it on a modern Linux system.

## Requirements

Depends on SDL 1.2 and libv4l. On Debian:
```
apt install libsdl1.2-dev libv4l-dev
```

## Installation

 - Edit config.mk
 - make
 - make install

## Usage
```
$ effectv -help
EffecTV - Realtime Video Effector
Version: 0.3.10
Usage: effectv [options...]
Options:
  -device FILE     use device FILE for video4linux
  -channel NUMBER  channel number of video source
  -norm {ntsc,pal,secam,pal-nc,pal-m,pal-n,ntsc-jp}
                   set video norm
  -freqtab {us-bcast,us-cable,us-cable-hrc,japan-bcast,japan-cable,europe-west,
            europe-east,italy,newzealand,australia,ireland,france,china-bcast,
            southafrica,argentina,canada-cable,australia-optus}
                   set frequency table
  -fullscreen      set fullscreen mode
  -hardware        use direct video memory (if possible)
  -doublebuffer    enable double buffering mode (if possible)
  -fps             show frames/sec
  -size WxH        set the size of capturing image
  -geometry WxH    set the size of screen
  -scale NUMBER    scaling the screen
  -autoplay NUMBER changes effects automatically every NUMBER frames
  -palette {rgb24,rgb565,rgb555,yuv422,yuv422p,yuv420p,yuv411p,yuv410p,grey}
                   set the palette of capturing device. It is detected
                   automatically by default.
  -vloopback FILE  use device FILE for output of vloopback device
```
