# NextBlog

基于 [Gmeek](https://github.com/Meekdai/Gmeek) 的博客系统，使用 `GitHub Pages` + `GitHub Issues` + `GitHub Actions` 快速搭建个人博客。

## 快速开始

### 第一步：创建仓库

点击 [**Use this template**](https://github.com/MurthiNext/NextBlog/generate) 按钮，选择 `Create a new repository`，填写仓库名称后创建。

> 仓库名称建议使用 `<username>.github.io` 格式，这样博客地址就是 `https://<username>.github.io`。如果用其他名称，博客地址为 `https://<username>.github.io/<repo-name>`。

### 第二步：配置博客

1. 进入新仓库，找到 `config.json` 文件
2. 编辑内容，填入你自己的信息：

```json
{
    "title": "你的博客名称",
    "subTitle": "博客副标题/简介",
    "avatarUrl": "你的头像图片链接",
    "email": "your-email@example.com",
    "startSite": "01/01/2025",
    "i18n": "CN",
    "UTC": 8,
    "urlMode": "issue",
    "GMEEK_BRANCH": "beta-dev"
}
```

3. 提交更改。

### 第三步：设置 GitHub Pages

进入仓库 `Settings` → `Pages`：
- `Source` 选择 `GitHub Actions`

### 第四步：写文章

进入仓库 `Issues` 页面，点击 `New issue`：
- 标题就是文章标题
- 正文使用 Markdown 格式
- 右侧 `Labels` 可以给文章打标签分类

提交 Issue 后，GitHub Action 会自动生成博客页面，稍等片刻即可访问。

> 修改 Issue 内容也会自动触发博客更新。

## 配置说明

| 配置项 | 说明 | 默认值 |
|--------|------|--------|
| `title` | 博客标题 | 必填 |
| `subTitle` | 副标题/简介 | 必填 |
| `avatarUrl` | 头像 URL | 必填 |
| `email` | 用于 Git 提交记录 | 必填 |
| `startSite` | 建站日期 (mm/dd/yyyy) | 空 |
| `i18n` | 语言：`CN`/`EN`/`RU` | `CN` |
| `UTC` | 时区偏移 | `+8` |
| `urlMode` | URL 模式：`issue`/`pinyin`/`ru_translit` | `pinyin` |
| `GMEEK_BRANCH` | NextBlog 模板分支 | `beta-dev` |
| `onePageListNum` | 每页文章数 | `15` |
| `needComment` | 是否启用评论 | `1` |

更多配置项请参考 [Gmeek 文档](https://github.com/Meekdai/Gmeek)。

## License

此项目基于 [Gmeek](https://github.com/Meekdai/Gmeek)，使用 [MIT License](LICENSE)。请保留页面底部和 console 界面的版权信息。
