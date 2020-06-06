# youtube-shell-transcriber
Util for uploading voice clips to YouTube via the command line.

### Conversion
`ffmpeg` command required for m4a to mp3  conversion is:
```shell script
ffmpeg -i foo.m4a -acodec libmp3lame -aq 2 foo.mp3
```
Converting AIFF to an MP$:
```shell script
ffmpeg -loop 1 -i video_bg.jpg -i foo.aiff -c:v libx264 -tune stillimage -c:a aac -b:a 192k -pix_fmt yuv420p -shortest foo.mp4
```