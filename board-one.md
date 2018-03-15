## Board One
[Pre-built images at snapshots.l.o](http://snapshots.linaro.org/openembedded/pre-built/lhg/morty/am57xx-evm/234/rpb-wayland/)

### Tests description
* weston1 - OK if weston starts on boot
* simple-egl1 - `weston-simple-egl -f`
* simple-egl2 - `weston-simple-egl -f -b`
* [gst-wayland1](gst-waylandX15sw.md) - play a video file with playbin and waylandsink using sw decoding
* [gst-wayland2](gst-waylandX15hw.md) - play a video file with ducatih264dec and waylandsink
* [chromium1](chromium1.md) - start chromium w/o URI specified in the command line
* [chromium2](chromium2.md) - play a video from youtube
* [chromium3](chromium3.md) - `webgl_morphtargets_horse` example from threejs.org

| Build no. | weston1 | simple-egl1 | simple-egl2 | gst-wayland1 | gst-wayland2 | chromium1 | chromium2 | chromium3 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 234 | OK | 59 fps | 59..60 fps | 1..15% CPU idle | 93..99% CPU idle | OK | 20..44% CPU idle | 58..60 fps, 71-82% CPU idle |
