# NextBlog

基于 [Gmeek](https://github.com/Meekdai/Gmeek) 的博客系统 — `GitHub Issues` 写作 + `GitHub Actions` 构建 + `GitHub Pages` 部署。
此项目由 [MurthiNext](https://github.com/MurthiNext) 维护，某种意义上可视作Gmeek的主题版本。

## 相对于 Gmeek 的改变

**前端重构**
- CSS 变量驱动的卡片式设计，暖灰色背景 + 白色卡片悬浮窗。
- 列表区移除外层方框，整体变为圆角卡片容器。
- 标签改为全圆角药片样式，悬停微动效。
- 深色/浅色主题完整适配。
- 页脚版权信息始终固定在页面底部，内容区自动撑满剩余空间。
- 内置使用 [vercount](https://github.com/EvanNotFound/vercount) 模块。

**更好的移动端适配**
- 文章标题与标签分为两行显示，标题不再被截断遮挡。
- 顶部头像与博客名紧凑排列为一行。

## 快速开始

### 1. 创建仓库

点击 [**Use this template**](https://github.com/MurthiNext/NextBlog/generate) → `Create a new repository`。

> 仓库名用 `<username>.github.io` 则博客地址为 `https://<username>.github.io`，否则为 `https://<username>.github.io/<repo-name>`。

### 2. 配置博客

编辑仓库根目录的 `config.json`：

```json
{
    "title": "你的博客名",
    "subTitle": "副标题",
    "avatarUrl": "头像链接",
    "email": "your-email@example.com",
    "startSite": "01/01/2025",
    "i18n": "CN",
    "UTC": 8,
    "GMEEK_BRANCH": "main"
}
```

### 3. 启用 Pages

仓库 `Settings` → `Pages` → Source 选 `GitHub Actions`。

### 4. 写文章

`Issues` → `New issue`，标题即文章标题，正文用 Markdown，右侧 Labels 打标签。提交后 Action 自动构建发布。

## License

基于 [Gmeek](https://github.com/Meekdai/Gmeek)，[MIT License](LICENSE)。请保留页面底部和 console 的版权信息。
