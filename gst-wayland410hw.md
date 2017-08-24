## gst-wayland1 test

```
gst-launch-1.0 -v filesrc location=ToS-4k-1920.mov ! qtdemux name=d d. ! h264parse ! v4l2video0dec capture-io-mode=dmabuf ! videoconvert ! waylandsink d. ! queue ! aacparse ! avdec_aac ! audioconvert ! audio/x-raw,format=S16LE ! alsasink
```

Test video: [ToS-4k-1920.mov](http://ftp.nluug.nl/pub/graphics/blender/demo/movies/ToS/ToS-4k-1920.mov)

CPU load is estimated by CPU idle numbers shown by 'top' running on serial console. Also venus interrupts should ticks - see 'cat /proc/interrupts | grep venus' output
