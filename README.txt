PAINEL BM • GBR / 3P (V5 • LOGIN BRANCO PRO)

✅ Melhorias:
- Login com fundo branco (visual mais profissional)
- Alternância Visualização/Admin por abas
- Indicador de acesso (Acesso: Visualização/Admin)
- Correção da classe .hidden (Admin e Ações somem corretamente no modo Visualização)
- Login obrigatório ao iniciar (não dá para fechar sem autenticar)

1) Trocar senhas:
   Abra o arquivo index.html e procure por:
     ADMIN_PASSWORD: "ADMIN_123"
     VIEWER_PASSWORD: "VIEW_123"
   Troque para as suas.

2) Rodar localmente (recomendado):
   - VS Code -> extensão Live Server -> abrir index.html com Live Server
   OU
   - Terminal na pasta:
     npx serve .

3) Publicar na Vercel:
   - Suba a pasta no GitHub e importe na Vercel
   OU
   - Vercel CLI:
     vercel
     vercel --prod

Webhooks:
- GET:   https://webhook.sistemavieira.com.br/webhook/get-bms
- SAVE:  https://webhook.sistemavieira.com.br/webhook/save-bms
- ALTER: https://webhook.sistemavieira.com.br/webhook/alter-bms
- DELETE:https://webhook.sistemavieira.com.br/webhook/delete-bms

Obs:
- Se o browser bloquear DELETE, o painel tenta fallback POST automaticamente.
