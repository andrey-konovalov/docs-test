## Board Two
[Pre-built images at snapshots.l.o](http://snapshots.linaro.org/openembedded/pre-built/lhg/morty/dragonboard-410c/latest/rpb-wayland/)

### Tests description
* weston1 - OK if weston starts on boot
* simple-egl1 - `weston-simple-egl -f`
* simple-egl2 - `weston-simple-egl -f -b`
* [gst-wayland410sw](gst-wayland410sw.md) - play a video file with waylandsink on DragonBoard-410c using sw decoding
* [gst-wayland410hw](gst-wayland410hw.md) - play a video file with waylandsink on DragonBoard-410c using hw decoding (venus engine)
* [chromium1](chromium1.md) - start chromium w/o URI specified in the command line
* [chromium2](chromium2.md) - play a video from youtube
* [chromium3](chromium3.md) - `webgl_morphtargets_horse` example from threejs.org

| Build no. | weston1 | simple-egl1 | simple-egl2 | gst-waylandsw | gst-waylandhw  | chromium1 | chromium2 | chromium3 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 234 | OK | 60 fps | 144..149 fps | 34..49% CPU idle | 77% CPU idle, 60 venus ints/sec | OK | 11..55% CPU idle | NG: "Rats! WebGL hit a snag"  |
| 215 | OK | 60 fps | 148..149 fps | 33..51% CPU idle | 76..77% CPU idle, 60 venus ints/sec | OK | 16..34% CPU idle | NG: "Rats! WebGL hit a snag"  |
| 189 | OK | 60 fps | 144..149 fps | 34..39% CPU idle | 76..77% CPU idle, 60 venus ints/sec | OK | 19..47% CPU idle | NG: "Rats! WebGL hit a snag"  |
| 182 | OK | 60 fps | 144..149 fps | 31..38% CPU idle | 76..77% CPU idle, 60 venus ints/sec | OK | 26..56% CPU idle | NG: "Rats! WebGL hit a snag"  |
| 176 | OK | 60 fps | 140..150 fps | 33..38% CPU idle | 76..77% CPU idle, 60 venus ints/sec | OK | 19..53% CPU idle | NG: GPU process silently crashes |
| 146 | OK | 60 fps | 145..148 fps | 33..49% CPU idle | 76..77% CPU idle, 60 venus ints/sec | OK | 16..50% CPU idle | NG: "Rats! WebGL hit a snag" |
| 143 | OK | 60 fps | 136..149 fps | 33..51% CPU idle | 76..78% CPU idle, 60 venus ints/sec | OK | 35..49% CPU idle | NG: "Rats! WebGL hit a snag" |
| 138 | OK | 60 fps | 150..151 fps | 33..50% CPU idle | 76..77% CPU idle, 60 venus ints/sec | OK | 17..34% CPU idle | 18..20 fps, 74..83% CPU idle |
| 117 | OK | 60 fps | 152..153 fps | 32..48% CPU idle | | OK | 35..57% CPU idle | 18..20 fps, 52..84% CPU idle |
| 116 | OK | 60 fps | 151..153 fps | 31..48% CPU idle | | OK | 37..62% CPU idle | 18..20 fps, 62..83% CPU idle |
