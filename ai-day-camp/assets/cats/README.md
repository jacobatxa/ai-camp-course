# 猫挑战 — 本地 MP4 + 封面

课件**优先播放本地 MP4**（山里可离线），YouTube 作有网时的备用。

| 格子 | 本地视频 | YouTube ID（备用） |
|------|----------|-------------------|
| 01 · 可爱的日常猫 | `cat_daily.mp4` | `g6dhJx_GXaA` |
| 02 · 穿西装上班的猫 | `cat_office.mp4` | `k8DzLwHWIbk` |
| 03 · 背书包上学的猫 | `cat_school.mp4` | `_fbiQUff82w` |

## 封面图

课件使用本目录 JPG：

- `cat_daily.jpg`
- `cat_office.jpg`
- `cat_school.jpg`

## 更新视频

若需替换为真实短视频片段，可用 `yt-dlp` 下载低分辨率 MP4 后覆盖同名文件（建议每段 &lt;5MB）：

```bash
yt-dlp -f "worst[ext=mp4]/worst" -o "cat_daily.%(ext)s" "https://www.youtube.com/watch?v=g6dhJx_GXaA"
```

当前仓库内 MP4 为基于封面图的短循环片段，保证离线可播。
