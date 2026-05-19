# Regra - Renome de rotas publicas e verificacao de links

## Principio

Quando o Fundador pedir para renomear uma URL publica, a IA deve tratar como pacote de rota, nao apenas como troca de nome de arquivo.

## Checklist obrigatorio

- Renomear ou criar o arquivo/rota nova.
- Atualizar todos os links internos nos repertorios aplicaveis.
- Atualizar `manifest.webmanifest`, `sw.js`, `robots.txt`, `sitemap.xml` e documentos de versionamento quando existirem referencias.
- Criar redirecionamento do caminho antigo para o novo quando o site usar Cloudflare Pages, Workers ou outro roteador.
- Testar localmente a rota nova com HTTP 200.
- Verificar que a rota antiga nao permanece em links internos, salvo em regras de redirecionamento ou historico explicitamente intencional.
- Se a alteracao envolver menu da home, verificar visualmente a ordem pedida pelo Fundador.

## Regra especifica atual

`https://www.jus9tecnologia.com.br/app-demo` foi renomeado para `https://www.jus9tecnologia.com.br/app-demo-advogar`.

Quando houver `Mais Direito` no menu principal da home, o link `Equipe` deve aparecer imediatamente a esquerda dele.
