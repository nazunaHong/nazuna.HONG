# 个人主页 · GitHub Pages

静态站点，直接由 GitHub Pages 托管。

## 本地预览

```bash
python3 -m http.server 8080
# 打开 http://localhost:8080
```

## 发布到 GitHub Pages

### 方式一：GitHub Actions（推荐，自动部署）

仓库已包含 `.github/workflows/deploy.yml`，推送到 `main` 分支即自动发布到
`https://<你的用户名>.github.io/<仓库名>/`。

需要的仓库权限：`Settings → Pages → Build and deployment → Source` 选 `GitHub Actions`。

### 方式二：分支发布

把根目录内容推到 `gh-pages` 分支，然后仓库设置里 Source 选 `gh-pages` 分支、`/ (root)`。

## 修改内容

所有内容都在 `index.html` 里：
- **个人信息** — 顶部导航、Hero、`#about`、`#contact` 各段文字
- **作品集** — `#work` 区块的 `<article>` 卡片
- **技术栈百分比** — `#stack` 里 `data-w="95"` 这类属性
- **经历时间线** — `#path` 区块的 `.step` 结构
