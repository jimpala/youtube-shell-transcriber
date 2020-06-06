# youtube-shell-transcriber
Util for uploading voice clips to YouTube via the command line.

### Conversion
`ffmpeg` command required for m4a to mp3  conversion is:
```shell script
ffmpeg -i foo.m4a -acodec libmp3lame -aq 2 foo.mp3
```