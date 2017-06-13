## Board Three
[Pre-built images at snapshots.l.o](http://snapshots.linaro.org/openembedded/pre-built/lhg/morty/board-three/rpb-wayland/latest/)

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
| 104 | OK | 54..57 fps | 169..221 fps | 62..64% CPU idle | OK | 59..74% CPU idle | 49..57 fps, 80..81% CPU idle | OK | OK | OK |
| 103 | OK | 57 fps | 152..189 fps | 62% CPU idle | OK | 65..75% CPU idle | 53..57 fps, 81% CPU idle | OK | | |
