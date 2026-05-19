# Regra - Pacote Lembrando Backend Jus 9

Data: 2026-05-19

Esta regra torna obrigatorio manter, em todos os repertorios da Jus 9 Tecnologia Juridica, um arquivo de continuidade chamado `LEMBRANDO_BACKEND_PROXIMOS_PASSOS.md`.

## Objetivo

Tudo o que nao puder ser feito imediatamente com seguranca deve ficar registrado como proximo passo de Backend, sem virar simulacao enganosa no frontend e sem expor dados reais.

## Quando usar

- Integracao com Google Agenda, WhatsApp, e-mail transacional, pagamentos ou APIs externas.
- Login real, perfis, permissoes, auditoria e area secreta.
- Dados reais de cliente, processo, documento, investimento ou equipe.
- Criptografia, cofre juridico, assinatura, tokens, secrets ou webhooks.
- Servidor local, deploy, Cloudflare Workers, banco de dados ou migracoes.

## Procedimento obrigatorio

1. Ler `LEMBRANDO_BACKEND_PROXIMOS_PASSOS.md` no repertorio afetado.
2. Classificar o dado e o risco antes de implementar.
3. Se ainda for MVP, manter dados ficticios e avisos de demonstracao.
4. Se exigir backend real, encaminhar para os repertorios de backend, auth, banco, cofre, logs e infra.
5. Atualizar governanca/documentacao quando a regra geral mudar.
6. Testar links, rotas, responsividade e ausencia de referencias antigas antes do commit.

## Repertorios de referencia

- `backend-api-jus9-tecnologia-juridica`
- `auth-identidade-acesso-jus9-tecnologia-juridica`
- `db-modelos-migracoes-jus9-tecnologia-juridica`
- `cofre-documentos-seguros-jus9-tecnologia-juridica`
- `logs-auditoria-jus9-tecnologia-juridica`
- `infra-cloudflare-jus9-tecnologia-juridica`
- `workers-pages-functions-jus9-tecnologia-juridica`

© Jus 9 Tecnologia Juridica - software livre, autoria preservada.