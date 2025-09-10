# 🔗 GitHub → Make → Telegram Integration / Integração GitHub → Make → Telegram
**2025-09-09**

**Languages:** [English](README.md) • [Português (pt-BR)](README.pt-BR.md) • [中文（简体）](README.zh-CN.md)

---

## 📌 Quick Description / Descrição rápida / 简要说明

| 🇺🇸 English | 🇧🇷 Português | 🇨🇳 中文（简体） |
|---|---|---|
| **Quick Description**: Integration to send GitHub push notifications to a Telegram bot using Make (Integromat). Based on the provided guide. | **Descrição rápida**: Integração para enviar notificações de push do GitHub para um bot do Telegram usando Make (Integromat). Baseado no guia fornecido. | **简要说明**：使用 Make（Integromat）将 GitHub push 通知发送到 Telegram 机器人的集成。基于提供的指南。 |

---

## 📂 Main Files / Arquivos principais / 主要文件

| 🇺🇸 English | 🇧🇷 Português | 🇨🇳 中文（简体） |
|---|---|---|
| - `Guia Completo Atualizado com Grupo.pdf` — documentation and step-by-step guide. | - `Guia Completo Atualizado com Grupo.pdf` — documentação e passo a passo. | - `Guia Completo Atualizado com Grupo.pdf` — 文档与分步指南。 |

---

## 🛠️ Step-by-Step / Passo a passo resumido / 步骤概述

| 🇺🇸 English | 🇧🇷 Português | 🇨🇳 中文（简体） |
|---|---|---|
| 1. Create a bot on Telegram using `@BotFather` and save the TOKEN.<br>2. Get your Chat ID (e.g., via `@userinfobot`) or group ID.<br>3. On Make, create a **Custom Webhook** and copy the URL.<br>4. Configure a Webhook in GitHub (Settings → Webhooks) pointing to the Make URL (`application/json`, event: `push`).<br>5. In the Make scenario, add the **Telegram Bot → Send a text message** module, connect with the TOKEN, set the Chat ID, and build the message using webhook variables.<br>6. Activate the scenario in Make and test with a `git push`. | 1. Crie um bot no Telegram com `@BotFather` e guarde o TOKEN.<br>2. Obtenha seu Chat ID (ex.: via `@userinfobot`) ou ID do grupo.<br>3. No Make, crie um **Custom Webhook** e copie a URL.<br>4. Configure um Webhook no GitHub (Settings → Webhooks) apontando para a URL do Make (`application/json`, evento: `push`).<br>5. No cenário do Make, adicione o módulo **Telegram Bot → Send a text message**, conecte com o TOKEN, defina o Chat ID e monte a mensagem usando variáveis do webhook.<br>6. Ative o cenário no Make e teste com um `git push`. | 1. 使用 `@BotFather` 在 Telegram 上创建机器人并保存 TOKEN。<br>2. 获取 Chat ID（例如通过 `@userinfobot`）或群组 ID。<br>3. 在 Make 中创建 **Custom Webhook** 并复制 URL。<br>4. 在 GitHub（Settings → Webhooks）中配置 Webhook，指向 Make 的 URL（`application/json`，事件：`push`）。<br>5. 在 Make 场景中添加 **Telegram Bot → Send a text message** 模块，连接 TOKEN，设置 Chat ID，并使用 webhook 变量构建消息。<br>6. 激活场景并通过 `git push` 测试。 |

---

## ✅ Test / Teste / 测试

| 🇺🇸 English | 🇧🇷 Português | 🇨🇳 中文（简体） |
|---|---|---|
| Make a commit and run `git push` — check if the notification arrived in Telegram. | Faça um commit e `git push` — verifique se a notificação chegou no Telegram. | 提交并执行 `git push` — 检查通知是否到达 Telegram。 |

---

## 🙌 Credits / Créditos / 致谢

| 🇺🇸 English | 🇧🇷 Português | 🇨🇳 中文（简体） |
|---|---|---|
| Material and base guide: *Guia Completo Atualizado com Grupo.pdf* (academic use). | Material e roteiro base: *Guia Completo Atualizado com Grupo.pdf* (uso acadêmico). | 材料与基础指南：*Guia Completo Atualizado com Grupo.pdf*（学术用途）。 |

---

## 📜 License / Licença / 许可证

| 🇺🇸 English | 🇧🇷 Português | 🇨🇳 中文（简体） |
|---|---|---|
| Academic use. Please cite the source when reusing. | Uso acadêmico. Cite a fonte ao reutilizar. | 学术用途。重复使用请注明来源。 |

---

## 🔁 Recommended workflow / Fluxo recomendado / 推荐工作流

```bash
git checkout -b integration/make-telegram
# add guide PDF and docs
git add Guia\ Completo\ Atualizado\ com\ Grupo.pdf README*.md
git commit -m "Add Make→Telegram integration guide and multilingual READMEs"
git push origin integration/make-telegram
# open PR and request review
```

---

## 📝 Notes / Observações / 备注

| 🇺🇸 English | 🇧🇷 Português | 🇨🇳 中文（简体） |
|---|---|---|
| Keep your TOKEN and Chat ID secret. Do not commit tokens to source control. Use environment variables or secrets in CI/automation platforms like Make. | Mantenha o TOKEN e o Chat ID em segredo. Não comite tokens no controle de versão. Use variáveis de ambiente ou secrets em plataformas de automação como o Make. | 请妥善保管 TOKEN 与 Chat ID，勿将 token 提交至源码。请在 Make 等自动化平台中使用环境变量或密钥管理。 |
