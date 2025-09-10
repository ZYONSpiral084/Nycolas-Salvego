# 🔗 Integração GitHub → Make → Telegram
**2025-09-09**

**Idiomas:** [English](README.md) • [Português (pt-BR)](README.pt-BR.md) • [中文（简体）](README.zh-CN.md)

---

## 📌 Descrição rápida

Integração para enviar notificações de push do GitHub para um bot do Telegram usando Make (Integromat). Baseado no guia fornecido.

---

## 📂 Arquivos principais

- `Guia Completo Atualizado com Grupo.pdf` — documentação e passo a passo.

---

## 🛠️ Passo a passo resumido

1. Crie um bot no Telegram com `@BotFather` e guarde o TOKEN.  
2. Obtenha seu Chat ID (ex.: via `@userinfobot`) ou ID do grupo.  
3. No Make, crie um **Custom Webhook** e copie a URL.  
4. Configure o Webhook no GitHub (Settings → Webhooks) apontando para a URL do Make (`application/json`, evento: `push`).  
5. No cenário do Make, adicione **Telegram Bot → Send a text message**, conecte com o TOKEN, defina o Chat ID e monte a mensagem com variáveis do webhook.  
6. Ative o cenário e teste com um `git push`.

---

## ✅ Teste

Faça um commit e `git push` — verifique se a notificação chegou no Telegram.

---

## 🙌 Créditos

Material e roteiro base: `Guia Completo Atualizado com Grupo.pdf` (uso acadêmico).

---

## 📜 Licença

Uso acadêmico. Cite a fonte ao reutilizar.

---

## 🔁 Fluxo recomendado

```bash
git checkout -b integration/make-telegram
# add guide PDF and docs
git add Guia\ Completo\ Atualizado\ com\ Grupo.pdf README*.md
git commit -m "Add Make→Telegram integration guide and multilingual READMEs"
git push origin integration/make-telegram
```

---

## 📝 Observações

Mantenha o TOKEN e Chat ID em segredo. Não comite tokens no repositório; use variáveis de ambiente ou secrets.
