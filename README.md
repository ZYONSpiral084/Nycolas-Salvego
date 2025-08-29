# Integração GitHub → Make → Telegram
**Tarefa de Faculdade — FATEC Ourinhos**

**Descrição rápida**
Integração para enviar notificações de push do GitHub para um bot do Telegram usando Make (Integromat). Baseado no guia fornecido. 

**Arquivos principais**
- `Guia Completo Atualizado com Grupo.pdf` — documentação e passo a passo. 

**Passo a passo resumido**
1. Crie um bot no Telegram com `@BotFather` e guarde o TOKEN.  
2. Obtenha seu Chat ID (ex.: via `@userinfobot`) ou ID do grupo.  
3. No Make, crie um **Custom Webhook** e copie a URL.  
4. Configure Webhook no GitHub (Settings → Webhooks) apontando para a URL do Make (Content type: `application/json`, evento: `push`).  
5. No cenário do Make, adicione o módulo **Telegram Bot → Send a text message**, conecte com o TOKEN e use o Chat ID; monte a mensagem com as variáveis do webhook.  
6. Ative o cenário no Make e teste com um `git push`.

**Teste**
Faça um commit e `git push` — verifique se a notificação chegou no Telegram.

**Créditos**
Material e roteiro base: *Guia Completo Atualizado com Grupo.pdf* (uso acadêmico). 

**Licença**
Uso acadêmico. Cite a fonte ao reutilizar.




