## Board Two
[Pre-built images at snapshots.l.o](http://snapshots.linaro.org/openembedded/pre-built/lhg/morty/dragonboard-410c/rpb-wayland/latest/)

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
| 108 | OK | 60 fps | 152..153 fps | 1Hz, 70..71% CPU idle | OK | 34..54% CPU idle | 18..20 fps, 70..82% CPU idle |
| 107 | OK | 60 fps | 150 fps | 1Hz, 69..72% CPU idle | OK | 32..60% CPU idle | 18..20 fps, 80..83% CPU idle |
| 106 | OK | 60 fps | 150 fps | 1Hz, 71% CPU idle | OK | 39..56% CPU idle | 19..22 fps, 83..85% CPU idle |
| 105 | OK | 60 fps | 149..152 fps | 1Hz, 71% CPU idle | OK | 38..52% CPU idle | 19..23 fps, 80..85% CPU idle |
| 104 | OK | 60 fps | 150..151 fps | 1Hz, 71..72% CPU idle | OK | 38..54% CPU idle | 18..21 fps, 75..84% CPU idle |
| 103 | OK | 60 fps | 149..151 fps | 1Hz, 71% CPU idle | OK | 40..60% CPU idle | 19..21 fps, 86% CPU idle |
