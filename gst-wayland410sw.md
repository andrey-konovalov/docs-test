## gst-wayland1 test

```
gst-launch-1.0 filesrc location=ToS-4k-1920.mov ! qtdemux name=d d. ! h264parse ! avdec_h264 ! videoconvert ! waylandsink d. ! queue ! aacparse ! avdec_aac ! audioconvert ! audio/x-raw,format=S16LE ! alsasink
```

Test video: [ToS-4k-1920.mov](http://ftp.nluug.nl/pub/graphics/blender/demo/movies/ToS/ToS-4k-1920.mov)

CPU load is estimated by CPU idle numbers shown by 'top' running on serial console.
