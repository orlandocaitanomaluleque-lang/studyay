# StudyAI Full — SaaS Educacional

Inclui:
- Cadastro e login
- JWT + SQLite + bcrypt
- Dashboard
- Assistente IA via backend
- Resumo e quiz com IA
- Histórico básico
- Limite gratuito diário
- Estrutura Premium pronta para integração de pagamentos

## Requisitos
Node.js 18+.

## Instalação
```bash
cd backend
npm install
```

Crie a variável `OPENAI_API_KEY` no ambiente antes de usar a IA.
Opcionalmente defina `JWT_SECRET`.

Linux/macOS:
```bash
export OPENAI_API_KEY="SUA_CHAVE"
export JWT_SECRET="UMA_CHAVE_FORTE"
npm start
```

Windows PowerShell:
```powershell
$env:OPENAI_API_KEY="SUA_CHAVE"
$env:JWT_SECRET="UMA_CHAVE_FORTE"
npm start
```

Abra:
http://localhost:3000

A chave da API fica no servidor e não no frontend. A integração usa a Responses API conforme a documentação oficial da OpenAI. citeturn0search0

Antes de produção: HTTPS, rate limiting, recuperação de palavra-passe, cookies/sessões mais robustos, validação, logs, política de privacidade e um provedor de pagamentos.

## PWA / Android

A versão `StudyAI-PWA` inclui:
- Web App Manifest
- Service Worker
- Ícones 192x192 e 512x512
- Botão de instalação quando o navegador disponibilizar o prompt

Para instalar no Android, o site precisa estar publicado em HTTPS. Em Chrome, o menu pode mostrar “Instalar app” ou “Adicionar à tela inicial”.
