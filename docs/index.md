# 欢迎来到 Py3fun 文档站

这是使用 MkDocs + Material 主题构建的静态文档网站。你可以在本地用 Markdown 编写内容并发布到 GitHub Pages。

## 快速开始

- 在 `docs/` 目录中新增或编辑 Markdown 文件，例如 `docs/guide/intro.md`。
- 更新站点导航：在根目录的 `mkdocs.yml` 中的 `nav` 字段添加你的文档。
- 本地预览：

```bash
# 安装依赖（首次）
pip install -r requirements.txt

# 启动本地预览服务器（默认 http://127.0.0.1:8000）
mkdocs serve
```

## 部署到 GitHub Pages

本仓库已配置 GitHub Actions，会在你向 `main` 分支推送时自动构建并部署到 GitHub Pages。

- 如果你是 `py3fun/py3fun.github.io` 仓库，站点地址将是 `https://py3fun.github.io/`。
- 也可以手动部署：

```bash
mkdocs gh-deploy --force
```

## 示例内容

- 勾选清单支持：

- [x] 使用 Markdown 编写
- [x] Material 主题美观易用
- [ ] 更多内容等你添加

祝写作愉快！
