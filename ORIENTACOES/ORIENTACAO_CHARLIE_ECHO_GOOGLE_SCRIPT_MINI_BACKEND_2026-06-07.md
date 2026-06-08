# Orientacao para Charlie Echo - Google Script, mini Backend e Cartorio Digital

Registrado em: 2026-06-07 21:02:00.00000

## Finalidade

Este registro ensina Charlie Echo a reconhecer o trabalho atual sobre o `JUS9_DRIVE_SAVER_MVP`, o mini backend em Google Apps Script usado para salvar documentos no Cartorio Digital com governanca minima.

## Onde esta o projeto

`C:\Users\aeonp\Documents\GitHub\charlieecho-jus9-tecnologia-juridica\INTEGRACOES\JUS9_DRIVE_SAVER_MVP`

Arquivos principais:

- `Code.gs`
- `Enviar-Jus9Documento.ps1`
- `TESTES_MANUAIS.md`
- `GUIA_USO_RAPIDO_DRIVE_SAVER_MVP_2026-06-08.md`

## Regras que Charlie Echo deve respeitar

1. Nao pedir senha Google.
2. Nao salvar token, chave, `.env` ou segredo em repositorio.
3. Nao escrever automaticamente em `04_COFRE_NAO_AUTOMATICO`.
4. Nao editar, excluir ou sobrescrever arquivos existentes.
5. Criar sempre documento novo com cabecalho de classificacao.
6. Enviar `JURIDICO_SIGILOSO` para `00_ENTRADA_PARA_REVISAO_HUMANA`.
7. Enviar classificacao desconhecida para revisao humana.
8. Pausar quando houver risco juridico, humano, familiar, institucional, financeiro, reputacional, de cofre ou de dados reais.

## Rotas do mini backend

- `PUBLICO`: `01_DOCUMENTOS_PUBLICOS_E_EDUCATIVOS`
- `INTERNO`: `02_DOCUMENTOS_INTERNOS_JUS9`
- `JURIDICO_SIGILOSO`: `00_ENTRADA_PARA_REVISAO_HUMANA`
- `COFRE_NAO_AUTOMATICO`: bloqueado

## Como testar sem violar governanca

Usar conteudo ficticio. Usar `-PedirChave` no PowerShell ou variavel de ambiente local. Nao escrever a chave interna, a URL ativa do Web App ou IDs privados em arquivo publico.

## Criterio de autonomia

Charlie Echo so deve ser considerada apta a operar sozinha quando demonstrar que sabe:

- classificar documentos;
- respeitar revisao humana;
- bloquear cofre automatico;
- nao expor segredo;
- criar documento novo;
- registrar resultado;
- pedir ajuda quando faltar contexto.

## Lembrete final

O objetivo do mini backend nao e dar autonomia sem limite. O objetivo e reduzir atrito operacional mantendo Charlie Echo protegida, governada e ensinavel.
