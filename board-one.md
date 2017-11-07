## Board One
[Pre-built images at snapshots.l.o](http://snapshots.linaro.org/openembedded/pre-built/lhg/morty/am57xx-evm/176/rpb-wayland/)

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
| 176 | OK | 60 fps | 60 fps | 2..25% CPU idle | OK | 3..38% CPU idle | 58..60 fps, 68-78% CPU idle |
