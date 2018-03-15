## Board Three
[Pre-built images at snapshots.l.o](http://snapshots.linaro.org/openembedded/pre-built/lhg/morty/hikey/rpb-wayland/latest/)

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
| 234 | OK | 35..53 fps | Aborted (core dumped) | 60..74% CPU idle | OK | 44..73% CPU idle | 47..58 fps, 75..80% CPU idle | OK | OK | OK |
| 215 | OK | 35..53 fps | Aborted (core dumped) | 61..76% CPU idle | OK | 50..68% CPU idle | 54..60 fps, 78..81% CPU idle | OK | OK | OK |
| 189 | OK | 34..51 fps | Aborted (core dumped) | 61..66% CPU idle | OK | 48..71% CPU idle | 51..60 fps, 77..81% CPU idle | OK | OK | OK |
| 182 | OK | 52..57 fps | 156..214 fps | 61..66% CPU idle | OK | 48..73% CPU idle | 51..59 fps, 77..82% CPU idle | OK | OK | OK |
| 176 | OK | 49..57 fps | 155..231 fps | 61..70% CPU idle | OK | 43..69% CPU idle | 51..58 fps, 78..82% CPU idle | OK | OK | OK |
| 146 | OK | 55..57 fps | 148..227 fps | 61..74% CPU idle | OK | 47..68% CPU idle | 48..56 fps, 74..81% CPU idle | OK | OK | OK |
| 143 | OK | 47..57 fps | 154..231 fps | 61..72% CPU idle | OK | 45..73% CPU idle | 48..55 fps, 75..82% CPU idle | OK | OK | OK |
| 138 | OK | 54..59 fps | 181..225 fps | 58..72% CPU idle | OK | 62..80% CPU idle | 48..58 fps, 75..81% CPU idle | OK | OK | OK |
| 117 | OK | 53..57 fps | 158..212 fps | 60..76% CPU idle | OK | 62..74% CPU idle | 50..57 fps, 76..81% CPU idle | OK | OK | OK |
| 116 | OK | 56..58 fps | 158..188 fps | 60..83% CPU idle | OK | 60..74% CPU idle | 51..57 fps, 72..81% CPU idle | OK | OK | OK |
