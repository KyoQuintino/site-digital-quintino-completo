# Publicar Digital Quintino na Vercel

## Configuração preparada
- Framework: Vite
- Comando de instalação: `npm install --no-audit --no-fund`
- Build: `npm run build`
- Diretório publicado: `dist/public`
- Rewrite SPA para suportar rotas do frontend.

## Passos
1. Extraia este ZIP e envie a pasta do projeto para um repositório GitHub seu (não publique chaves ou arquivos `.env`).
2. Entre em https://vercel.com/new e importe o repositório.
3. Confirme as configurações de build em `vercel.json` e clique em Deploy.
4. Ao concluir, a Vercel mostrará o subdomínio gratuito `*.vercel.app`.
5. Teste a página inicial, rotas internas, imagens e todos os links de checkout Hotmart.

## Atenção
Este projeto tem uma interface `/admin` que, segundo o README original, guarda alterações apenas no navegador e não tem autenticação nem banco de dados. Não use esse painel para dados privados nem o considere um painel administrativo seguro.

O build não foi validado neste ambiente: a instalação de dependências via npm excedeu o limite de tempo disponível. A Vercel tentará instalar e compilar durante o deploy; confira os logs caso falhe. Este ZIP não foi enviado para sua conta Vercel nem publicado automaticamente.
