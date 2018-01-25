## gst-waylandX15hw test

Hardware decoding test for X15. Must be run as root.


```
gst-launch-1.0 -v filesrc location=/home/linaro/ToS-4k-1920.mov ! qtdemux name=d d. ! h264parse ! queue ! ducatih264dec ! video/x-raw, format=NV12 ! waylandsink d. ! aacparse ! avdec_aac ! queue ! audioconvert ! alsasink
```

Test video: [ToS-4k-1920.mov](http://ftp.nluug.nl/pub/graphics/blender/demo/movies/ToS/ToS-4k-1920.mov)

CPU load is estimated by CPU idle numbers shown by 'top' running on serial console.
