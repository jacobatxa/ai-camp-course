# assets/cats/ — Day 1 猫挑战离线视频

## 当前状态

`kids.html` 的 Day 1 第 4 页使用本目录 3 个本地 MP4，点击卡片即可播放：

- `cat_daily.mp4`
- `cat_office.mp4`
- `cat_school.mp4`

播放器策略为「仅本地离线播放」，不依赖外网。

## 推荐素材规格

- 编码：H.264（`libx264`）+ `yuv420p`
- 分辨率：1280x720（或 720p 等效）
- 时长：8–20 秒
- 音频：可无音轨（课堂演示不受环境噪音影响）
- 内容：建议保留 AI 痕迹，便于课堂讨论

## 快速替换命令

```bash
# 进入仓库根目录执行
ffmpeg -y -i "你的源视频.mp4" \
  -vf "scale=1280:720:force_original_aspect_ratio=cover,crop=1280:720,format=yuv420p" \
  -r 30 -c:v libx264 -profile:v high -level 4.0 -movflags +faststart -an \
  "ai-day-camp/assets/cats/cat_daily.mp4"
```

按同样方式替换 `cat_office.mp4`、`cat_school.mp4` 即可。

## 文件说明

| 文件 | 说明 |
|------|------|
| `cat_daily.jpg` | 日常猫封面图 |
| `cat_daily.mp4` | 日常猫离线视频 |
| `cat_office.jpg` | 上班猫封面图 |
| `cat_office.mp4` | 上班猫离线视频 |
| `cat_school.jpg` | 上学猫封面图 |
| `cat_school.mp4` | 上学猫离线视频 |
