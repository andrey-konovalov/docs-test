## chromium4 test

```
$ cdmiservice &
$ /usr/bin/chromium/chrome --no-sandbox --use-gl=egl --ozone-platform=wayland \
    --composite-to-mailbox --in-process-gpu --enable-low-end-device-mode \
    --enable-logging --v=0 --start-maximized --user-data-dir=data_dir \
    --blink-platform-log-channels=Media \
    --register-pepper-plugins="/usr/lib64/chromium/libopencdmadapter.so#ClearKey CDM#ClearKey CDM0.1.0.0#0.1.0.0;application/x-ppapi-open-cdm" \
    http://people.linaro.org/~peter.griffin/chrome/eme_player.html
```

Select "External ClearKey" and hit "Play" button.
The test is passed if the video plays back OK.
