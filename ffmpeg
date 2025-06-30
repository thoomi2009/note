# FFMPEG
## 常用参数解释
```
-i xxx.mp4 指定输入文件的路径（避免中文路径）
-c:v libx264 指定视频编码器为libx264（H.264）
-crf 20 设置CRF（常量速率因子）的值。这是视频质量的控制，范围从0（无损）到51（最糟），通常使用18到28的值。
-c:a aac 指定音频编码器为AAC。
-strict experimental 允许使用实验性的编码器。
-b:a 192k 设置音频比特率为192k。
-codec: copy：复用编解码器，这意味着不重新编码视频和音频。
-start_number 0：每个TS切片的起始编号从0开始。
-hls_time 10：每个TS切片的持续时间为10秒。
-hls_list_size 0：播放列表中的TS切片数量没有限制。
-f hls：输出格式为HLS。
output.m3u8：输出的M3U8播放列表文件名。
-s（设置分辨率）
-b:v（设置视频比特率）
```
## 常用命令
```
将mp4文件转为mp3文件
ffmpeg -i input.mp4 -vn -c:a libmp3lame -q:a 4 output.mp3 -y
将mp4文件转为m3u8文件
ffmpeg -i demo.mp4 -codec: copy -start_number 0 -hls_time 10 -hls_list_size 0 -f hls output.m3u8
```
