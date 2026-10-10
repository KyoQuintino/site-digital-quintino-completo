# Publicação no Netlify — DigitalQuintino

## Configuração
- Comando de build: `npm run build:netlify` (compila a aplicação React/Vite sem tentar iniciar o servidor Express).
- Pasta publicada: `dist/public`.
- `netlify.toml` inclui fallback para as rotas da aplicação, como `/admin`.
- As imagens do catálogo ficam em `client/public/assets` e são copiadas para a pasta publicada durante o build.
- O projeto usa pnpm (`pnpm-lock.yaml`). Se o Netlify solicitar configurações manualmente, mantenha o gerenciador de pacotes detectado pelo lockfile.

## Publicar a partir do GitHub
1. Extraia o ZIP e envie o conteúdo da pasta `DigitalQuintino-vendas-editado` para um repositório GitHub sob seu controle.
2. Abra o painel do Netlify e escolha **Add new project → Import an existing project**.
3. Conecte o GitHub e selecione o repositório.
4. Confirme o comando `npm run build:netlify` e a pasta `dist/public`. O `netlify.toml` já define esses valores.
5. Inicie o deploy e confira o log de compilação.
6. Depois da publicação, teste em celular e computador: imagens, busca, filtros, visualização rápida, links Hotmart, WhatsApp e atualização de rotas internas.

## Atenção antes de vender
- Confirme todos os links de checkout, preços, descrições, direitos de uso das capas e dados de contato. Não validei compras reais nem transações.
- O formulário de novidades abre uma conversa no WhatsApp; não armazena nem envia e-mail para uma lista.
- O painel `/admin` salva capas apenas no `localStorage` do navegador atual. Ele não tem autenticação nem sincronização de servidor e **não é um painel privado seguro**. Não coloque informações confidenciais nele.
- Acessibilidade recebeu ajustes de teclado, foco e movimento reduzido, mas ainda precisa de testes manuais com leitor de tela e auditoria automatizada; não é uma certificação WCAG.
- Não consegui executar uma compilação nesta sessão porque o gerenciador de pacotes não pôde ser baixado da rede. Faça o primeiro deploy e confira o log do build.
