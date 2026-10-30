# 个人作品集

石纤惠的个人作品集 —— 戏剧影视文学硕士，文字与影像创作者。柔和粉色系，以「文字作品」为核心。纯 HTML + CSS + 原生 JS，无构建依赖，可直接部署到 GitHub Pages。

## 本地预览

直接用浏览器打开 `index.html` 即可，或运行一个简单的本地服务器：

```bash
python -m http.server 8000
# 然后访问 http://localhost:8000
```

## 页面结构

- 关于我
- 文字作品（支持分类筛选：剧本 / 评论 / 小说）
- 创作与实践
- 经历
- 联系

## 文字作品 PDF

文字作品对应的 PDF 放在 `works/` 目录：

- `works/baixue-gongzhu.pdf` — 戏剧剧本《白雪公主》
- `works/bufu-zhouzi.pdf` — 影视剧剧本《不负周子》第一幕节选
- `works/edipusi-wang.pdf` — 戏剧评论《俄狄浦斯王》
- `works/meiyou-yiwai.pdf` — 小说《没有意外》

## 如何替换成你自己的内容

1. **基本信息**：打开 `index.html`，替换姓名、联系方式、经历等。
2. **文字作品**：复制 `.write-card`，修改标题、简介，并设置 `data-category`（`剧本`、`评论`、`小说`）以匹配筛选；`href` 指向对应的 PDF。
3. **配色**：在 `css/styles.css` 顶部的 `:root` 变量里调整主题色（当前为柔和粉色系）。

## 部署到 GitHub Pages

1. 在仓库 **Settings → Pages**，Source 选择 `Deploy from a branch`，Branch 选 `main`、文件夹选 `/ (root)`，保存。
2. 稍等片刻即可通过 `https://<用户名>.github.io/<仓库名>/` 访问。