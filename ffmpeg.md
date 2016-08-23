# Create video file (mp4,avi,mkv) from static image and audio file
``
ffmpeg -loop 1 -r 1 -i image.png -i audio.mp3 -c:v libx264 -c:a aac -strict experimental -shortest -pix_fmt yuv420p out.mp4
``
