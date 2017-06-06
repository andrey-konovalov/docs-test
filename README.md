## LHG OE build manual test results
[Morty based builds at snapshots.l.o](http://snapshots.linaro.org/openembedded/pre-built/lhg/morty/)

### Test cases
* weston1 - OK if weston starts on boot
* simple-egl1 - `weston-simple-egl -f`
* simple-egl2 - `weston-simple-egl -f -b`
* [gst-wayland1](gst-wayland1.md) - play a video file with playbin and waylandsink
* [chromium1](chromium1.md) - start chromium w/o URI specified in the command line
* [chromium2](chromium2.md) - play a video from youtube
* [chromium3](chromium3.md) - `webgl_morphtargets_horse` example from threejs.org
* [chromium4](chromium4.md) - ClearKey OpenCDM test (for boards with OPTEE)
* optee-generic - `xtest` (OPTEE test to verify all the generic features)
* optee-sdp - `xtest --sdp-basic` (basic SecureDataPlane OPTEE test)

### Test Results per board
* [Board One results](board-one.md)
* [Board Two results](board-two.md)
