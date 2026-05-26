# Mapa de Agendas Jus 9 e Charlie Echo

Data: 2026-05-26

## Agendas identificadas

### 1. Agenda real / privada

Fonte: Google Agenda conectado ao Fundador.

Uso: reunioes, tarefas, preparacao, Web Summit, contatos e rotina interna.

Tratamento: nao publicar integralmente.

### 2. Agenda MVP / demonstrativa

Fontes:

- `mvp-jus9-tecnologia-juridica/agenda.html`
- `mvp-jus9-tecnologia-juridica/app-agenda.html`
- `jus9-tecnologia-juridica/app-agenda.html`

Uso: dados ficticios, separacao por MVP, localStorage, ICS e Google Agenda em modo contrato.

### 3. Agenda Web Summit / investidores

Fonte: documentos publicos e materiais de investimentos.

Uso: eventos publicos, preparacao, pitch, QR Codes, follow-up e oportunidades.

Tratamento: pode virar pagina publica sanitizada, sem agenda real privada.

### 4. Agenda Charlie Echo

Fonte: tarefas da Jus 9 que mencionam Charlie Echo, linguagem das IAs, materiais publicos, governanca e revisoes.

Uso: recorte interno ou publico controlado.

### 5. Agenda tecnica / backend

Fonte: `backend-api-jus9-tecnologia-juridica`.

Rotas existentes:

- `GET /api/agenda/status`
- `POST /api/agenda/events`
- `GET /api/integrations/readiness`

Uso: validar contrato local. Ainda nao envia evento real ao Google.

## Decisao atual

Manter Google Agenda como botao visivel em modo contrato, sem prometer conexao real.

Integracao real somente depois de OAuth, backend seguro, logs, permissoes e revisao humana.

