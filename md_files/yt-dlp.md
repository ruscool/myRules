# best video + audio

yt-dlp -f 'bv[height=1080][ext=mp4]+ba[ext=m4a]' --merge-output-format mp4 <https://www.youtube.com/watch?v=1La4QzGeaaQ> -o '%(title)s.mp4'
