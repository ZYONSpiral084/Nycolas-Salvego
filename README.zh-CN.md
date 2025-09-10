# 🔗 GitHub → Make → Telegram 集成
**2025-09-09**

**语言：** [English](README.md) • [Português (pt-BR)](README.pt-BR.md) • [中文（简体）](README.zh-CN.md)

---

## 📌 简要说明

使用 Make（Integromat）将 GitHub push 通知发送到 Telegram 机器人。基于所提供的指南。

---

## 📂 主要文件

- `Guia Completo Atualizado com Grupo.pdf` — 文档与分步指南。

---

## 🛠️ 步骤概述

1. 使用 `@BotFather` 在 Telegram 上创建机器人并保存 TOKEN。  
2. 获取 Chat ID（例如通过 `@userinfobot`）或群组 ID。  
3. 在 Make 中创建 **Custom Webhook** 并复制 URL。  
4. 在 GitHub（Settings → Webhooks）中配置 Webhook，指向 Make 的 URL（`application/json`，事件：`push`）。  
5. 在 Make 场景中添加 **Telegram Bot → Send a text message** 模块，连接 TOKEN，设置 Chat ID，并使用 webhook 变量构建消息。  
6. 激活场景并通过 `git push` 测试。

---

## ✅ 测试

提交并执行 `git push` — 检查通知是否到达 Telegram。

---

## 🙌 致谢

材料与基础指南：`Guia Completo Atualizado com Grupo.pdf`（学术用途）。

---

## 📜 许可证

学术用途。重复使用请注明来源。

---

## 🔁 推荐工作流

```bash
git checkout -b integration/make-telegram
# add guide PDF and docs
git add Guia\ Completo\ Atualizado\ com\ Grupo.pdf README*.md
git commit -m "Add Make→Telegram integration guide and multilingual READMEs"
git push origin integration/make-telegram
```

---

## 📝 备注

请保管好 TOKEN 与 Chat ID，不要将 token 提交至源码。请在 Make 等自动化平台中使用环境变量或密钥管理。
