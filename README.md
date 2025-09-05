# 🔗 GitHub → Make → Telegram Integration / Integração GitHub → Make → Telegram  
**🎓 College Assignment — FATEC Ourinhos / Tarefa de Faculdade — FATEC Ourinhos**

---

| 🇺🇸 English | 🇧🇷 Português |
|-------------|--------------|
| **Quick Description**<br>Integration to send GitHub push notifications to a Telegram bot using Make (Integromat). Based on the provided guide. | **Descrição rápida**<br>Integração para enviar notificações de push do GitHub para um bot do Telegram usando Make (Integromat). Baseado no guia fornecido. |

---

## 📂 Main Files / Arquivos principais  

| 🇺🇸 English | 🇧🇷 Português |
|-------------|--------------|
| - `Guia Completo Atualizado com Grupo.pdf` — documentation and step-by-step guide. | - `Guia Completo Atualizado com Grupo.pdf` — documentação e passo a passo. |

---

## 🛠️ Step-by-Step / Passo a passo resumido  

| 🇺🇸 English | 🇧🇷 Português |
|-------------|--------------|
| 1. Create a bot on Telegram using `@BotFather` and save the TOKEN.<br>2. Get your Chat ID (e.g., via `@userinfobot`) or group ID.<br>3. On Make, create a **Custom Webhook** and copy the URL.<br>4. Configure a Webhook in GitHub (Settings → Webhooks) pointing to the Make URL (`application/json`, event: `push`).<br>5. In the Make scenario, add the **Telegram Bot → Send a text message** module, connect with the TOKEN, set the Chat ID, and build the message using webhook variables.<br>6. Activate the scenario in Make and test with a `git push`. | 1. Crie um bot no Telegram com `@BotFather` e guarde o TOKEN.<br>2. Obtenha seu Chat ID (ex.: via `@userinfobot`) ou ID do grupo.<br>3. No Make, crie um **Custom Webhook** e copie a URL.<br>4. Configure Webhook no GitHub (Settings → Webhooks) apontando para a URL do Make (`application/json`, evento: `push`).<br>5. No cenário do Make, adicione o módulo **Telegram Bot → Send a text message**, conecte com o TOKEN e use o Chat ID; monte a mensagem com as variáveis do webhook.<br>6. Ative o cenário no Make e teste com um `git push`. |

---

## ✅ Test / Teste  

| 🇺🇸 English | 🇧🇷 Português |
|-------------|--------------|
| Make a commit and run `git push` — check if the notification arrived in Telegram. | Faça um commit e `git push` — verifique se a notificação chegou no Telegram. |

---

## 🙌 Credits / Créditos  

| 🇺🇸 English | 🇧🇷 Português |
|-------------|--------------|
| Material and base guide: *Guia Completo Atualizado com Grupo.pdf* (academic use). | Material e roteiro base: *Guia Completo Atualizado com Grupo.pdf* (uso acadêmico). |

---

## 📜 License / Licença  

| 🇺🇸 English | 🇧🇷 Português |
|-------------|--------------|
| Academic use. Please cite the source when reusing. | Uso acadêmico. Cite a fonte ao reutilizar. |
