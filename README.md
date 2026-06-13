# 超级 AI 营 · 课程仓库

9–11 岁 AI 素养夏令营课件与教师教案。推荐 **三日营**（每天 90–120 分钟），课件用 URL 参数按天放映。

## 在线访问（GitHub Pages）

| 页面 | 链接 |
|------|------|
| 课程入口 | https://jacobatxa.github.io/ai-camp-course/ |
| 三日营主页 | https://jacobatxa.github.io/ai-camp-course/ai-day-camp/ |
| **孩子课件 Day 1** | https://jacobatxa.github.io/ai-camp-course/ai-day-camp/kids.html?day=1 |
| **孩子课件 Day 2** | https://jacobatxa.github.io/ai-camp-course/ai-day-camp/kids.html?day=2 |
| **孩子课件 Day 3** | https://jacobatxa.github.io/ai-camp-course/ai-day-camp/kids.html?day=3 |
| **教师教案** | https://jacobatxa.github.io/ai-camp-course/ai-day-camp/design.html |

## 课件快捷操作

- **G** — 打开目录（按 Day 1 / 2 / 3 分组），跳转幻灯片  
- **E** — 编辑模式：页内改字，自动保存到本机浏览器（可导出/导入 JSON）  
- **空格 / ← →** — 翻页  
- **?day=1|2|3** — 切换封面角标、学习目标与路线文案，并跳到该天首页

## 目录结构

```
ai-day-camp/
  kids.html      # 孩子版幻灯（25 页，三日营）
  design.html    # 三日营教师教案
  parent.html    # 家长版
  assets/bg/     # 本地背景图
  assets/cats/   # 猫挑战 MP4 + 封面（离线可播）
  assets/day1/   # Day1 户外示意
  assets/day2/   # Day2 工坊示意
```

## 本地预览

```bash
open "ai-day-camp/kids.html?day=1"
# 或
python3 -m http.server 8080
# 浏览器打开 http://localhost:8080/ai-day-camp/kids.html?day=1
```
