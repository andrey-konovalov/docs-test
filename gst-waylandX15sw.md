## gst-waylandX15sw test

Software decoding test for X15


```
gst-launch-1.0 playbin uri=file:///home/linaro/ToS-4k-1920.mov video-sink="videoconvert ! video/x-raw,format=BGRx ! waylandsink"
```

Test video: [ToS-4k-1920.mov](http://ftp.nluug.nl/pub/graphics/blender/demo/movies/ToS/ToS-4k-1920.mov)

CPU load is estimated by CPU idle numbers shown by 'top' running on serial console.
