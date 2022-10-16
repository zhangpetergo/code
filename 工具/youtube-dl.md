# youtube-dl

1.下载 youtube-dl工具

官网

https://youtube-dl.org/

github

https://github.com/ytdl-org/youtube-dl/



2.下载fmpeg

官网

https://www.ffmpeg.org/

github

https://github.com/BtbN/FFmpeg-Builds/releases





这两个工具下载下来，配置环境变量。





3.下载一个视频演示

https://www.crowdcast.io/e/cryptocurrency-class-2022/1





打开google，开发者工具，选择网络，设置m3u8，然后重新请求视频，然后选择第一个mp4，找到url，复制



分析清晰度

```
youtube-dl --proxy http://127.0.0.1:10809/ -F https://stream.crowdcast.io/623a1aa039166b009da2def0/vod_master.m3u8
```

选择清晰度，下载

```
youtube-dl --proxy http://127.0.0.1:10809/ -f 2340 -o "加密货币.mp4" https://stream.crowdcast.io/623a1aa039166b009da2def0/vod_master.m3u8
```

