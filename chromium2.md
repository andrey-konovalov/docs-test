## chromium2 test

```
/usr/bin/chromium/chrome --no-sandbox --use-gl=egl --ozone-platform=wayland \
  --composite-to-mailbox --in-process-gpu --enable-low-end-device-mode \
  --enable-logging --v=0 --start-maximized --user-data-dir=data_dir \
  --blink-platform-log-channels=Media \
  https://www.youtube.com/watch?v=-TqVFa2eL4o
```

CPU load is estimated by CPU idle numbers shown by 'top' running on serial console.
