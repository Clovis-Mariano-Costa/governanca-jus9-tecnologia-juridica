# Versionamento - Governanca cripto GitHub v1.0

Data: 2026-05-25

## Escopo

- Criada varredura local sobre todos os repositorios Git em `Documents/GitHub`.
- Registrado relatorio humano e JSON tecnico em `RELATORIOS/GOVERNANCA_CRIPTO_GITHUB_2026_05_25/`.
- Classificados duplicados por SHA-256, candidatos de segredo/configuracao sensivel, diretorios gerados, arquivos grandes, `.env`, `.gitignore`, `.gitattributes` e linguagem antiga.

## Decisao de seguranca

- Nenhum valor de token, senha ou segredo foi impresso no relatorio.
- Arquivos institucionais duplicados, documentos grandes e conteudo de cofre nao foram apagados automaticamente.
- Remocao automatica ficou restrita a caches/builds locais claramente regeneraveis.

## Proximos passos

- Revisar duplicados institucionais antes de qualquer remocao rastreada pelo Git.
- Revisar linguagem antiga, em especial usos publicos de `assistiva`.
- Avaliar arquivos grandes de cofre/documentos restritos com decisao expressa do Fundador.
