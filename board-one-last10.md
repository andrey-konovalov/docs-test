## Board One
[Pre-built images at snapshots.l.o](http://snapshots.linaro.org/openembedded/pre-built/lhg/morty/am57xx-evm/rpb-wayland/latest/)

### Tests description
* weston1 - OK if weston starts on boot
* simple-egl1 - `weston-simple-egl -f`
* simple-egl2 - `weston-simple-egl -f -b`
* [gst-wayland1](gst-wayland1.md) - play a video file with playbin and waylandsink
* [chromium1](chromium1.md) - start chromium w/o URI specified in the command line
* [chromium2](chromium2.md) - play a video from youtube
* [chromium3](chromium3.md) - `webgl_morphtargets_horse` example from threejs.org

| Build no. | weston1 | simple-egl1 | simple-egl2 | gst-wayland1 | chromium1 | chromium2 | chromium3 |
| --- | --- | --- | --- | --- | --- | --- | --- |
| 117 | OK | 60 fps | 60 fps | 7..34% CPU idle | OK | 11..43% CPU idle | 58..60 fps, 59-74% CPU idle |
| 116 | OK | 60 fps | 60 fps | 6..22% CPU idle | OK | 29..42% CPU idle | 58..60 fps, 69-73% CPU idle |
| 115 | OK | 59..60 fps | 59..60 fps | 14..31% CPU idle | OK | 18..45% CPU idle | 56..60 fps, 66-86% CPU idle |
| 108 | OK | 59..60 fps | 60 fps | 4..24% CPU idle | OK | 13..43% CPU idle | 58..60 fps, 73-84% CPU idle |
| 107 | OK | 60 fps | 60 fps | 5..26% CPU idle | OK | 6..43% CPU idle | 58..60 fps, 55-76% CPU idle |
| 106 | OK | 59..60 fps | 60 fps | 5..31% CPU idle | OK | 35..43% CPU idle | 59..60 fps, 67-75% CPU idle |
| 105 | OK | 60 fps | 60 fps | 6..19% CPU idle | OK | 34..43% CPU idle | 58..60 fps, 65-83% CPU idle |
| 104 | OK | 60 fps | 60 fps | 5..17% CPU idle | OK | 37..43% CPU idle | 59..60 fps, 67-70% CPU idle |
| 103 | OK | 60 fps | 60 fps | 5..7% CPU idle | OK | 36..41% CPU idle | 59..60 fps, 64-70% CPU idle |
