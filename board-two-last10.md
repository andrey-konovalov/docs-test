## Board Two
[Pre-built images at snapshots.l.o](http://snapshots.linaro.org/openembedded/pre-built/lhg/morty/board-one/rpb-wayland/latest/)

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
| 103 | OK | 60 fps | 149..151 fps | 1Hz, 71% CPU idle | OK | 40..60% CPU idle | 19..21 fps, 86% CPU idle |
