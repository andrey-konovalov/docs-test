## Board Three
[Pre-built images at snapshots.l.o](http://snapshots.linaro.org/openembedded/pre-built/lhg/morty/hikey/rpb-wayland/106/)

This board has no sound.

### Tests description
* weston1 - OK if weston starts on boot
* simple-egl1 - `weston-simple-egl -f`
* simple-egl2 - `weston-simple-egl -f -b`
* [gst-wayland1](gst-wayland1.md) - play a video file with playbin and waylandsink
* [chromium1](chromium1.md) - start chromium w/o URI specified in the command line
* [chromium2](chromium2.md) - play a video from youtube
* [chromium3](chromium3.md) - `webgl_morphtargets_horse` example from threejs.org
* [chromium4](chromium4.md) - Clearkey OPTEE test
* optee-generic - `xtest` (OPTEE test to verify all the generic features)
* optee-sdp - `xtest --sdp-basic` (basic SecureDataPlane OPTEE test)

| Build no. | weston1 | simple-egl1 | simple-egl2 | gst-wayland1 | chromium1 | chromium2 | chromium3 | chromium4 | optee-generic | optee-sdp |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 106 | OK | 53..56 fps | 166..206 fps | 61..64% CPU idle | OK | 63..72% CPU idle | 50..57 fps, 73..81% CPU idle | OK | OK | OK |
