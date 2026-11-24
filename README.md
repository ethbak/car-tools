# car-tools

Pages for testing the car apps in [aaos-browser-test](https://github.com/ethbak/aaos-browser-test) on the head unit, served at https://ethbak.github.io/car-tools/.

- `index.html`: opens the car diagnostics screen in the patched Firefox (`cardiag://report`), plus a link to the video test.
- `video-test.html`: plays H.264 clips at 480p, 720p and 1080p (30 fps) and 1080p (60 fps), measures decoded, dropped and presented frames, and checks the WebGL renderer and Widevine levels. Results go to the public ntfy topic `ethbak-car-video-83b31f50` (playback numbers only), or to the topic in `#t=<topic>` if the link has one.
- `clips/`: the test clips, generated with ffmpeg's `testsrc2`.
