# AI 文档知识库设置文档

**日期**: 2026-02-01
**主题**: 系统设置

## 概述

本文档记录了 AI 文档知识库的自动设置过程。

## 系统架构

- **SSH 认证**: 使用 SSH key 与 GitHub 仓库通信
- **自动化脚本**: `/root/.openclaw/workspace/scripts/save-doc.sh`
- **存储结构**: 按日期和主题分类归档

## 目录结构

```
summaries/
├── YYYY/
│   ├── YYYY-MM/
│   │   ├── YYYY-MM-DD-topic-name.md
```

## 工作流程

1. 用户请求总结或保存文档
2. 系统自动提取/总结内容
3. 生成 Markdown 文件
4. 按日期和主题命名
5. 自动提交到 GitHub

## 测试

这是第一个自动保存的文档，用于验证系统是否正常工作。

---

**来源**: https://github.com/nikogu123/ai-docs
