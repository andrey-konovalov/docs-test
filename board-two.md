## Board Two
[Pre-built images at snapshots.l.o](http://snapshots.linaro.org/openembedded/pre-built/lhg/morty/dragonboard-410c/176/rpb-wayland/)

### Tests description
* weston1 - OK if weston starts on boot
* simple-egl1 - `weston-simple-egl -f`
* simple-egl2 - `weston-simple-egl -f -b`
* [gst-wayland410sw](gst-wayland410sw.md) - play a video file with waylandsink
* [gst-wayland410hw](gst-wayland410hw.md) - play a video file with waylandsink using venus hw decoding
* [chromium1](chromium1.md) - start chromium w/o URI specified in the command line
* [chromium2](chromium2.md) - play a video from youtube
* [chromium3](chromium3.md) - `webgl_morphtargets_horse` example from threejs.org

| Build no. | weston1 | simple-egl1 | simple-egl2 | gst-waylandsw | gst-waylandhw  | chromium1 | chromium2 | chromium3 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 176 | OK | 60 fps | 140..150 fps | 33..38% CPU idle | 76..77% CPU idle, 60 venus ints/sec | OK | 19..53% CPU idle | NG: GPU process silently crashes |
