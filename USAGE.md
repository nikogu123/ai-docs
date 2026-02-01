# OpenClaw 文档系统使用指南

## 快速开始

让 OpenClaw 保存文档的触发方式：

```
"帮我保存为文档：[内容]"
"总结成文档：[主题] - [内容]"
"保存这个链接：[URL] - [描述]"
```

## 示例

```
1. 直接保存内容：
   "帮我保存为文档：关于 AI 的学习笔记"

2. 保存带主题的文档：
   "总结成文档：编程技巧 - 如何使用 Git 高效工作"

3. 保存网页链接：
   "保存这个链接：https://example.com/article - 这是一篇关于机器学习的文章"
```

## 文档结构

文档会自动按日期和主题分类：

```
summaries/
├── 2026/
│   ├── 2026-02/
│   │   ├── 2026-02-01-ai-docs-setup.md
│   │   └── 2026-02-01-中文测试文档.md
```

## 功能特性

- ✅ 自动日期归档
- ✅ 中文支持
- ✅ 主题分类
- ✅ 原文链接保存
- ✅ 自动提交到 GitHub
- ✅ Markdown 格式

## 技术细节

- **SSH 认证**: ~/.ssh/id_ed25519_ai_docs
- **仓库**: git@github.com-ai-docs:nikogu123/ai-docs.git
- **脚本**: /root/.openclaw/workspace/scripts/doc.sh
- **Python 工具**: /root/.openclaw/workspace/scripts/save-doc.py

## 维护

如需修改配置，编辑以下文件：
- Python 脚本: `/root/.openclaw/workspace/scripts/save-doc.py`
- 仓库路径: REPO_DIR
- SSH 配置: ~/.ssh/config

---

*最后更新: 2026-02-01*
