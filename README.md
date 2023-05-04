Ref
- https://medium.com/bootdotdev/create-a-golang-video-streaming-server-using-hls-a-tutorial-f8c7d4545a0f
- https://zenn.dev/tera_ny/articles/42bc5e704fbdb7
- https://itnext.io/how-to-create-an-hls-stream-using-golang-and-ffmpeg-20f30c7c9750

変換コマンド
```
ffmpeg -i video.mp4 -profile:v baseline -level 3.0 -start_number 0 -hls_time 10 -hls_list_size 0 -f hls ./playlist.m3u8
```

```
go run main.go
cd app
yarn dev
```
