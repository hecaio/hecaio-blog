# hecaio's tech blog

AI/大模型、RAG、NLP、后端开发技术博客。

## 技术栈

- **框架**：Hugo + [PaperMod](https://github.com/adityatelange/hugo-PaperMod) 主题
- **托管**：GitHub Pages
- **部署**：GitHub Actions 自动部署（push 到 main 触发）
- **写作**：本地 Markdown，文件在 `content/posts/`

## 本地预览

```bash
hugo server --buildDrafts --bind 127.0.0.1 --port 1313
# 访问 http://127.0.0.1:1313/hecaio-blog/
```

## 写新文章

```bash
hugo new posts/my-new-post.md
# 编辑 content/posts/my-new-post.md
# frontmatter 需要 title / date / tags / author
```

## 部署

push 到 `main` 分支 → GitHub Actions 自动 build + deploy 到 Pages。

无需手动操作。

## 私有信息保护

公开笔名 `hecaio` = GitHub 账户名 = 博客署名，**对外完全一致**。

`.gitignore` 已排除 `.env`、`*.key`、`*.token`、`*.pem` 等敏感文件。

代码、配置、教程示例**绝不硬编码**任何 API key / secret / 真实邮箱。