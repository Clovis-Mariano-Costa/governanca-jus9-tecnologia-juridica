# Relatorio MVP - formularios e uso adequado de foto

Data: 2026-05-25

## Objetivo

Registrar a continuidade do pacote MVP da Jus 9 Tecnologia Juridica, com foco em:

- validacao das rotas publicas essenciais do MVP;
- varredura de formularios HTML nos repositorios locais do GitHub;
- classificacao de formularios em que foto/avatar pode ser adequada;
- preservacao da regra de MVP demonstrativo, sem dados reais e sem segredos no frontend.

## Validacao publica do MVP

As seguintes rotas foram verificadas com resposta HTTP 200:

- `https://www.jus9tecnologia.com.br/mvp`
- `https://www.jus9tecnologia.com.br/demo-01-advogado-defensor.html`
- `https://www.jus9tecnologia.com.br/demo-02-professor.html`
- `https://www.jus9tecnologia.com.br/demo-03-estudante.html`
- `https://www.jus9tecnologia.com.br/app-demo-professor.html`
- `https://www.jus9tecnologia.com.br/app-demo-estudante.html`
- `https://www.jus9tecnologia.com.br/app-agenda.html`
- `https://www.jus9tecnologia.com.br/login/`

Evidencia detalhada: `validacao_rotas_mvp_publicas_2026-05-25.csv`.

## Professor e estudante

O MVP Professor e o MVP Estudante devem continuar como prioridade imediata, porque ja possuem:

- pagina publica de entrada;
- login demonstrativo adequado ao MVP;
- aviso de ausencia de Google Cloud ativo;
- aviso de nao uso de dados reais;
- painel proprio de demonstracao.

Pontos confirmados no repositorio principal:

- `demo-02-professor.html` aponta o botao principal para `app-demo-professor.html`;
- `demo-03-estudante.html` aponta o botao principal para `app-demo-estudante.html`;
- `app-demo-professor.html` informa `demo2@jus9tecnologia.com.br` e senha demonstrativa `Jus9MVP#2026`;
- `app-demo-estudante.html` informa `demo3@jus9tecnologia.com.br` e senha demonstrativa `Jus9MVP#2026`;
- nenhum desses paineis deve autenticar usuario real nesta fase.

## Varredura de formularios

Foram encontrados 42 formularios HTML ou paginas com campos de formulario suficientes para revisao.

Resumo por recomendacao:

- `nao`: 27 formularios
- `sim-avatar-demo`: 11 formularios
- `ja-cobre-imagem`: 4 formularios

Evidencia detalhada: `formularios_html_classificados_foto_2026-05-25.csv`.

## Onde foto e adequada

A foto e adequada apenas como avatar demonstrativo, imagem ficticia ou foto institucional de teste, sem documento real e sem dado pessoal sensivel.

Prioridade para evolucao:

- `mvp-jus9-tecnologia-juridica/cadastro.html`
- `mvp-jus9-tecnologia-juridica/cadastro-lider.html`
- `mvp-jus9-tecnologia-juridica/cadastro-usuario.html`
- `mvp-jus9-tecnologia-juridica/perfis/professor.html`
- `mvp-jus9-tecnologia-juridica/perfis/estudante.html`
- `mvp-jus9-tecnologia-juridica/lider-mvp.html`
- `jus9-tecnologia-juridica/lider-mvp.html`
- `charlieecho-jus9-tecnologia-juridica/ia-estudantes.html`

Recomendacao visual:

- usar upload opcional ou selecao de avatar demonstrativo;
- exibir previa local no navegador;
- nao enviar imagem para servidor nesta fase;
- nao gravar foto em backend, Google, Drive ou storage externo no MVP;
- incluir aviso curto: "Use imagem ficticia ou avatar demonstrativo. Nao envie documento, foto de menor ou dado real."

## Onde foto nao deve entrar agora

Nao recomendo adicionar campo especifico de foto nos fluxos abaixo:

- agenda;
- login;
- processos;
- WhatsApp;
- importacao de mensagens;
- rotas OAuth;
- formularios puramente operacionais.

Motivo: a foto aumentaria risco de privacidade e complexidade sem ganho para o MVP.

## Onde imagem ja esta contemplada

Os formularios abaixo ja possuem campo de arquivo que aceita imagem ou anexo equivalente:

- `jus9-tecnologia-juridica/app-atendimento-inicial.html`
- `jus9-tecnologia-juridica/app-retorno.html`

Recomendacao: manter como anexo demonstrativo/evidencia ficticia, sem criar campo separado de foto pessoal.

## Cronograma sugerido

### Pacote 1 - Professor e Estudante

Implementar avatar demonstrativo opcional nos formularios de cadastro/perfil do MVP Professor e Estudante.

Critérios:

- funciona offline;
- imagem fica apenas no navegador/localStorage, se necessario;
- sem upload real;
- sem dado pessoal real;
- aviso de uso ficticio visivel.

### Pacote 2 - Lider e usuario

Adicionar avatar demonstrativo aos cadastros de lider e usuario, mantendo separacao entre perfil visual e identidade real.

Critérios:

- avatar opcional;
- botao para remover imagem;
- fallback por iniciais;
- sem documento pessoal.

### Pacote 3 - Atendimento e retorno

Revisar textos dos anexos de imagem ja existentes para reforcar que sao evidencias ficticias.

Critérios:

- nao criar campo novo;
- manter upload apenas demonstrativo;
- reforcar governanca humana e ausencia de dados reais.

### Pacote 4 - Auditoria publica

Validar no navegador as telas alteradas e registrar no versionamento.

Critérios:

- sem quebra mobile;
- sem segredo no codigo;
- sem dependência de Google Cloud;
- versionamento atualizado.

## Decisao recomendada

O proximo passo pratico deve ser implementar avatar/foto demonstrativa primeiro em Professor e Estudante, pois esses perfis sao prioritarios para o MVP e tem baixo risco quando a imagem fica apenas como recurso visual local.

