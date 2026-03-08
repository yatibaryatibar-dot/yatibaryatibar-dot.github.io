# Vincent Blog

基于 Hugo + PaperMod 主题的个人博客。

## 本地预览

```bash
# 安装 Hugo (macOS)
brew install hugo

# 启动本地服务器
hugo server -D
```

访问 http://localhost:1313 预览。

## 写文章

```bash
hugo new content posts/文章标题.md
```

编辑 `content/posts/文章标题.md` 文件，修改 front matter 和内容。

## 部署到 GitHub Pages

1. 在 GitHub 创建新仓库，命名为 `yatibaryatibar-dot.github.io`
2. 推送代码到 main 分支
3. 进入仓库 Settings → Pages → Source 选择 GitHub Actions
4. 自动部署完成，访问 https://yatibaryatibar-dot.github.io

## 目录结构

```
.
├── archetypes/          # 内容模板
├── assets/              # 静态资源
├── content/             # 网站内容
│   ├── posts/           # 文章
│   └── about.md         # 关于页面
├── data/                # 数据文件
├── layouts/             # HTML 模板
├── static/              # 静态文件
├── themes/              # 主题
│   └── PaperMod/        # PaperMod 主题
├── hugo.toml            # 站点配置
└── .github/workflows/   # GitHub Actions 配置
```

## 配置说明

修改 `hugo.toml` 可以调整：
- 网站标题、描述
- 导航菜单
- 主题参数
- 社交链接
