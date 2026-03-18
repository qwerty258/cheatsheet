ffmpeg
======

# combine video and audio without encoding

```sh
ffmpeg -i video.m4v -i audio.m4a -c:v copy -c:a copy output.mp4
```

# probe media

```sh
ffprobe unknown.mkv
```

# play media

```sh
ffplay download.mkv
```
