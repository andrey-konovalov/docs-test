## Board One
[Pre-built images at snapshots.l.o](http://snapshots.linaro.org/openembedded/pre-built/lhg/morty/am57xx-evm/latest/rpb-wayland/)

### Tests description
* weston1 - OK if weston starts on boot
* simple-egl1 - `weston-simple-egl -f`
* simple-egl2 - `weston-simple-egl -f -b`
* [gst-wayland1](gst-waylandX15sw.md) - play a video file with playbin and waylandsink using sw decoding
* [gst-wayland2](gst-waylandX15hw.md) - play a video file with ducatih264dec and
 waylandsink
* [chromium1](chromium1.md) - start chromium w/o URI specified in the command line
* [chromium2](chromium2.md) - play a video from youtube
* [chromium3](chromium3.md) - `webgl_morphtargets_horse` example from threejs.org

| Build no. | weston1 | simple-egl1 | simple-egl2 | gst-wayland1 | gst-wayland2 | chromium1 | chromium2 | chromium3 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 234 | OK | 59 fps | 59..60 fps | 1..15% CPU idle | 93..99% CPU idle | OK | 20..44% CPU idle | 58..60 fps, 71-82% CPU idle |
| 215 | OK | 59..60 fps | 60 fps | 1..14% CPU idle | 92..99% CPU idle | OK | 10..29% CPU idle | 58..60 fps, 66-78% CPU idle |
| 182 | OK | 59 fps | 59 fps | 0..17% CPU idle | | OK | 25..42% CPU idle | 58..60 fps, 72-85% CPU idle |
| 176 | OK | 60 fps | 60 fps | 2..25% CPU idle | | OK | 3..38% CPU idle | 58..60 fps, 68-78% CPU idle |
| 146 | OK | 60 fps | 60 fps | 7..26% CPU idle | | OK | 5..43% CPU idle | 59..60 fps, 49-78% CPU idle |
| 143 | OK | 59..60 fps | 59..60 fps | 2..23% CPU idle | | OK | 14..43% CPU idle | 58..60 fps, 56-85% CPU idle |
| 138 | OK | 60 fps | 60 fps | 7..28% CPU idle | | OK | 21..42% CPU idle | 57..60 fps, 44-71% CPU idle |
| 117 | OK | 60 fps | 60 fps | 7..34% CPU idle | | OK | 11..43% CPU idle | 58..60 fps, 59-74% CPU idle |
| 116 | OK | 60 fps | 60 fps | 6..22% CPU idle | | OK | 29..42% CPU idle | 58..60 fps, 69-73% CPU idle |
| 115 | OK | 59..60 fps | 59..60 fps | 14..31% CPU idle | | OK | 18..45% CPU idle | 56..60 fps, 66-86% CPU idle |
