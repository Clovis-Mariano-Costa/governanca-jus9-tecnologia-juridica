# Relatorio - Validacao pos-limpeza e assets publicos Jus 9 v1.0

Data: 2026-05-25

## Objetivo
Validar o ecossistema apos a consolidacao de duplicados, separar o que ainda precisa existir do que deve virar fonte central, e priorizar governanca, criptografia, assets publicos e linguagem institucional.

## Validacao publica
- Rotas testadas: 13
- Rotas com HTTP 200: 13
- https://www.jus9tecnologia.com.br/ | HTTP 200 | text/html; charset=utf-8 | bytes=26608
- https://www.jus9tecnologia.com.br/mvp | HTTP 200 | text/html | bytes=25779
- https://www.jus9tecnologia.com.br/demo-01-advogado-defensor.html | HTTP 200 | text/html | bytes=5715
- https://www.jus9tecnologia.com.br/demo-02-professor.html | HTTP 200 | text/html | bytes=6445
- https://www.jus9tecnologia.com.br/app-demo-advogar.html | HTTP 200 | text/html | bytes=7759
- https://investimentos.jus9tecnologia.com.br/ | HTTP 200 | text/html; charset=utf-8 | bytes=10021
- https://investimentos.jus9tecnologia.com.br/documentos | HTTP 200 | text/html; charset=utf-8 | bytes=16752
- https://investimentos.jus9tecnologia.com.br/downloads/videos/jus9-tecnologia-juridica-em-40-palavras.mp4 | HTTP 200 | video/mp4 | bytes=1498491
- https://investimentos.jus9tecnologia.com.br/downloads/videos/jus9-tecnologia-juridica-em-40-palavras.pdf?v=20260525-pdf-original | HTTP 200 | application/pdf | bytes=13280
- https://carta.jus9tecnologia.com.br/ | HTTP 200 | text/html; charset=utf-8 | bytes=38629
- https://livros.jus9tecnologia.com.br/ | HTTP 200 | text/html; charset=utf-8 | bytes=6455
- https://quandoodesenhofala.jus9tecnologia.com.br/ | HTTP 200 | text/html; charset=utf-8 | bytes=39142
- https://jus9verde.jus9tecnologia.com.br/ | HTTP 200 | text/html; charset=utf-8 | bytes=5201

## Duplicados remanescentes
- Grupos duplicados remanescentes: 118
- Grupos com arquivo nao essencial fora dos repos primarios: 70
Motivo principal: assets publicos ainda usados por HTML/CSS/JS, arquivos padrao por repositorio, fontes primarias Charlie Echo/aulas/governanca e copias de cofre/sigilo.

## Assets duplicados ainda referenciados
- Assets duplicados mapeados: 189
Repositorios com mais assets duplicados ainda referenciados:
- Aeon-Primevo: 28
- jus9-tecnologia-juridica: 28
- quandoodesenhofala-jus9-tecnologia-juridica: 24
- equipe-jus9-tecnologia-juridica: 20
- carta-jus9-tecnologia-juridica: 15
- livros-jus9-tecnologia-juridica: 11
- aulas-charlie-echo-jus9-tecnologia-juridica: 9
- governanca-jus9-tecnologia-juridica: 9
- charlieecho-jus9-tecnologia-juridica: 9
- mvp-jus9-tecnologia-juridica: 6

## Candidatos de segredo nao .env.example
- Total: 18
- provavel_documentacao: 10
- codigo_sem_valor_impresso: 7
- precisa_revisao_humana: 1
Observacao: nenhum valor secreto foi impresso neste relatorio. A maioria parece referencia a variaveis ou documentacao, mas os arquivos JS/backend devem ser revisados pontualmente antes de producao real.

## Linguagem antiga
- Ocorrencias totais: 183
- media: 104
- alta_governanca: 63
- alta_publico: 16
Padrao recomendado: I.A generativa multimodal jurista com governanca humana.

## Diagnostico
O ecossistema esta operacional apos a limpeza. O risco principal agora nao e duplicidade documental, mas duplicidade de assets publicos e linguagem antiga espalhada. Apagar mais sem centralizar assets pode quebrar paginas. O melhor proximo movimento e criar uma fonte oficial de assets publicos e migrar referencias de forma controlada.

## Proximo pacote recomendado
ASSETS_PUBLICOS_CENTRALIZADOS_JUS9_v1_0
Escopo: escolher fonte publica unica de logos, fotos, favicons, CSS compartilhado e imagens institucionais; atualizar referencias em paginas publicas; validar HTTP 200 dos assets; somente depois remover copias locais restantes.

## Arquivos tecnicos gerados
- validacao_http_rotas_publicas_robusta_2026-05-25.csv
- assets_duplicados_referenciados_2026-05-25.csv
- candidatos_segredo_nao_exemplo_2026-05-25.csv
- linguagem_antiga_priorizada_2026-05-25.csv
