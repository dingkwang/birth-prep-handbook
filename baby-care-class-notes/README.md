# 婴儿护理课讲义 · Free Baby Care Class

基于 **The Baby Academy** Free Baby Care Class（讲师 Cris）中文字幕整理的**结构化中文讲义**。

静态站点：`index.html` + `images/`（必须同目录保留，否则配图失效）。

## 本地预览

```bash
cd baby-care-class-notes
open index.html
# 或（checklist 的 localStorage 在部分浏览器 file:// 下更稳）
python3 -m http.server 8080 --directory .
# 浏览器打开 http://localhost:8080
```

## 目录结构

```
baby-care-class-notes/
  index.html          # 讲义正文（单页）
  images/             # 课中截帧与裁切（约 30+ JPG）
  README.md
```

**发布时务必包含 `images/`**，不要只提交 `index.html`。

## 功能

| 项目 | 说明 |
|------|------|
| 语言 | 简体中文要点讲义 |
| 配图 | 课中画面截帧（学习笔记用） |
| 交互 | 第 14 章可勾选清单（localStorage）· 回顶 · 阅读进度条 · 章间导航 |
| 版式 | ABC 磁贴 · 应当/不建议对照 · TOG 摄氏对照表 · 每章「带走」 |
| 温度 | 正文摄氏度；个别课件图可能仍含华氏，caption 会注明 |
| 不含 | 完整字幕正文、视频文件（体积过大） |
| 免责 | **非医疗建议**，请遵循儿科医生医嘱 |

可选：将 `婴儿护理课_完整版_中文字幕.mp4` 放在上级 `out/` 目录复习用，**不要**塞进 GitHub Pages（约 300MB+）。

## 发布到 GitHub Pages（自行操作）

请在你**自己的**公开账号创建仓库后再推送；本目录默认不关联远程。

```bash
cd baby-care-class-notes
git init
git add index.html README.md images/
git commit -m "Add baby care class lecture notes for GitHub Pages"
git branch -M main
git remote add origin git@github.com:<YOUR_USER>/<YOUR_REPO>.git
git push -u origin main
```

然后在 GitHub：**Settings → Pages → Deploy from a branch → main / root**。

## 许可与署名

讲义为学习整理笔记。课程版权归 The Baby Academy / 原讲师所有；请勿将本页宣称为官方教材。
截帧仅供个人学习对照，勿作商业传播。
