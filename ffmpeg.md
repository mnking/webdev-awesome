## Create video file (mp4,avi,mkv) from static image and audio file
```sh
ffmpeg -loop 1 -r 1 -i image.png -i audio.mp3 -c:v libx264 -c:a aac -strict experimental -shortest -pix_fmt yuv420p out.mp4
```
## Split Video from start to end time
```sh
ffmpeg -ss 00:00:00 -t 00:35:00 -i target.mp4 -acodec copy -vcodec copy output.mp4
```
