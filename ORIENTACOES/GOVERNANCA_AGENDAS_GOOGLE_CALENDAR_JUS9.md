# Governanca de Agendas e Google Calendar - Jus 9

Data: 2026-05-26
Classificacao: INTERNO / GOVERNANCA / AGENDA

## 1. Regra central

Agenda e dado sensivel por padrao.

Agenda pode revelar tempo, deslocamento, contatos, prioridades, reunioes, oportunidades, estrategia e riscos. Por isso, a agenda real do Google Agenda nao deve ser publicada integralmente.

## 2. Camadas de agenda

### Agenda publica

Conteudo sanitizado, informativo e aprovado para paginas publicas.

Pode conter:

- eventos publicos;
- datas sujeitas a confirmacao;
- preparacao publica;
- links oficiais;
- avisos de cautela.

Nao pode conter:

- link privado de calendario;
- link privado de Google Meet;
- telefone, e-mail pessoal ou contato sensivel;
- descricao operacional interna;
- dados reais de cliente, processo, documento, WhatsApp ou cofre.

### Agenda MVP / demonstrativa

Funciona com dados ficticios, localStorage, ICS e rascunho manual para Google Agenda.

Deve mostrar o botao Google Agenda visivel, com aviso:

> Google Agenda em modo contrato. Ainda nao conectado por OAuth.

### Agenda interna

Agenda operacional da Jus 9, Charlie Echo, Charlie Fox, equipe, investidores e Web Summit.

Nao publicar sem revisao humana.

### Agenda integrada futura

Somente pode existir com:

- backend seguro;
- OAuth;
- tokens fora do frontend;
- permissoes minimas;
- logs;
- tratamento de erro;
- revogacao;
- separacao por usuario/perfil;
- revisao humana.

## 3. Padrao visual para agendas MVP

Toda agenda MVP deve ter:

- seletor de MVP ou area;
- botao `Abrir Google Agenda (modo contrato)`;
- botao `Baixar ICS`;
- fallback offline;
- aviso de que nao ha conexao OAuth real;
- aviso de nao usar dados reais;
- classificacao `INTERNO / DEMO` para eventos demonstrativos.

## 4. Separacao por MVP

Cada evento demonstrativo deve identificar sua origem, por exemplo:

- `demo-01-advogado-defensor`;
- `demo-02-professor`;
- `demo-03-estudante`;
- `demo-04-cidadao`;
- `demo-05-empresa`;
- `demo-06-investidor`;
- `demo-07-delegado`;
- `demo-08-juiz`;
- `demo-09-estagiario`;
- `demo-10-cartorio`;
- `demo-11-administrador`;
- `demo-12-promotor`;
- `demo-13-orgao-publico`.

## 5. Proibicoes

Nao publicar:

- calendario privado;
- iframe de Google Calendar privado;
- token;
- secret;
- `.env`;
- refresh token;
- link privado de Meet;
- agenda com dados reais em MVP estatico;
- evento real de cliente, processo, atendimento, WhatsApp, cofre ou documento pessoal.

## 6. Criterio de pronto

A agenda esta adequada quando:

- funciona offline;
- permite baixar ICS;
- mostra botao Google Agenda visivel;
- deixa claro que o Google Agenda ainda nao esta conectado;
- separa o evento por MVP;
- nao promete OAuth real;
- nao envia dados reais;
- preserva revisao humana.

