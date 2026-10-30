# 个人作品集

一个柔和粉色系、以「文字作品」为核心的个人作品集页面，适合戏剧与影视 / 文学 / 传媒方向的学生与研究生使用。纯 HTML + CSS + 原生 JS，无构建依赖，可直接部署到 GitHub Pages。

## 本地预览

直接用浏览器打开 `index.html` 即可，或运行一个简单的本地服务器：

```bash
python -m http.server 8000
# 然后访问 http://localhost:8000
```

## 页面结构

- 关于我
- 文字作品（支持分类筛选：剧本 / 影评·剧评 / 随笔 / 论文）
- 影像与实践
- 经历
- 联系

## 如何替换成你自己的内容

1. **基本信息**：打开 `index.html`，把「林晓」「hello@example.com」「github.com/yourname」「中国 · 北京」等替换成你自己的信息。
2. **文字作品**：在「文字作品」区块复制 `.write-card`，修改标题、简介、年份，并设置 `data-category`（可选值：`剧本`、`评论`、`随笔`、`论文`）以匹配筛选。
3. **影像与实践**：复制 `.project-card`，修改标题、描述，并把 `.cover-a/.cover-b/.cover-c` 换成你自己的截图或配色。
4. **经历**：增删 `.timeline-item`。
5. **配色**：在 `css/styles.css` 顶部的 `:root` 变量里调整主题色（当前为柔和粉色系）。

## 部署到 GitHub Pages

1. 在 GitHub 新建仓库（或把本目录推送到已有仓库）。
2. 仓库 **Settings → Pages**，Source 选择 `main` 分支根目录（或 `/docs`），保存。
3. 稍等片刻即可通过 `https://<用户名>.github.io/<仓库名>/` 访问。