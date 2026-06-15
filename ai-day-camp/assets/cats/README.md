# assets/cats/ — AI猫视频素材

## 当前状态

当前 MP4 为 ffmpeg 从 JPG 图片转换的占位文件（单帧静止，约 30 KB），
播放器检测到 `duration < 1.5s` 时会自动降级：
1. 尝试本地 MP4
2. 若检测为静止帧 → 尝试 YouTube 嵌入（需网络）
3. 若 YouTube 也不可用 → 显示友好提示

## 替换为真实 AI 视频（推荐）

### 方法一：yt-dlp 下载 YouTube

```bash
pip install yt-dlp

# 日常猫（AI生成）
yt-dlp -o "assets/cats/cat_daily.mp4" -f "mp4[height<=720]" "https://www.youtube.com/watch?v=g6dhJx_GXaA"

# 上班猫（AI生成）
yt-dlp -o "assets/cats/cat_office.mp4" -f "mp4[height<=720]" "https://www.youtube.com/watch?v=k8DzLwHWIbk"

# 上学猫（AI生成）
yt-dlp -o "assets/cats/cat_school.mp4" -f "mp4[height<=720]" "https://www.youtube.com/watch?v=_fbiQUff82w"
```

### 方法二：从 B 站下载（内容质量更好）

```bash
pip install yt-dlp

# 替换 BV 号为你找到的AI生成猫视频
yt-dlp -o "assets/cats/cat_daily.mp4" "https://www.bilibili.com/video/BVxxxxxxxx"
```

B 站搜索关键词：`AI生成 猫` / `Sora 猫` / `Kling 猫咪` / `可灵 AI猫`

### 视频规格建议

- 时长：15–45 秒
- 分辨率：720p 以上
- 内容：明显带有 AI 生成痕迹（爪子变形、毛发不自然、背景失真等）
- 主题：三段须明显区分（日常 / 职场 / 校园 场景）

## 文件列表

| 文件 | 说明 |
|------|------|
| `cat_daily.jpg` | 日常猫封面图 |
| `cat_daily.mp4` | 日常猫视频（需替换） |
| `cat_office.jpg` | 上班猫封面图 |
| `cat_office.mp4` | 上班猫视频（需替换） |
| `cat_school.jpg` | 上学猫封面图 |
| `cat_school.mp4` | 上学猫视频（需替换） |
