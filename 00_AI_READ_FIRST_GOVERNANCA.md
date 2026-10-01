# AI_READ_FIRST — GOVERNANCA JUS 9

SCHEMA = JUS9_GOVERNANCE_ENTRY_V1
STATE = OPERACIONAL_EM_TESTE
PRIMARY_READER = IA
RULES = IA_FIRST + LINK_FIRST + EVIDENCE_FIRST + FAIL_CLOSED

## START

1. Leia este arquivo.
2. Leia o README do repositorio.
3. Identifique o objeto: NORMA | PROTOCOLO | HISTORICO | RASCUNHO | MIGRACAO | TECNICO.
4. Verifique autoridade, estado, versao e fonte antes de agir.
5. Nao trate existencia de arquivo como vigencia.
6. Nao trate rascunho como norma.
7. Nao reescreva genealogia; preserve predecessor/sucessor.
8. Use o mapa profissional para encontrar Legislador, Curador Normativo, Mestre, Codex e Seguranca.

## COMUNICACAO INTER-I.A.

MESSAGE_MINIMUM =
REQUEST_ID
FROM_ROLE
TO_ROLE
STATE
AUTHORITY
CLASSIFICATION
OBJECT
CANONICAL_URI
ACTION
PENDING
NEXT_ACTION

LINK_FIRST = preferir ponteiro canonico + metadados a copia integral.
LINK_SOZINHO = insuficiente.
EVIDENCE_FIRST = planejado != executado != verificado.
FAIL_CLOSED = duvida de autoridade/classificacao bloqueia efeito externo.

## CLASSIFICACAO

PISO_ATUAL = PUBLICO | SIGILOSO | SECRETO
Rotulos historicos adicionais podem existir, mas devem ser mapeados e nao criar protecao ficticia.

PUBLICO = acessivel a todos.
SIGILOSO = grupo de trabalho autorizado.
SECRETO = titular definido + custodia tecnica governada.

FOLDER_NAME_SECRET_OR_COFRE != SECURITY.
CUSTODY != READ_AUTHORIZATION.
PREVIOUS_ACCESS != CURRENT_AUTHORIZATION.

## UNIVERSIDADE DO FUTURO

UDF_GOVERNANCE_CHANGES = DEFERRED_UNTIL_CONSTITUTION_PROMULGATED_OR_CONSTITUENT_PROCESS_READY.
Nao reorganizar a Universidade do Futuro nesta espira antes desse gate.

## SEGURANCA

Nao publicar credencial, token, senha, chave privada, segredo real ou segredo de justica.
Caminho contendo COFRE/SECRET/SECRETO/SIGILOSO -> classificar e validar fronteira real antes de publicar/mover.

## PRINCIPIO PEDAGOGICO

IF_JUS9_LEARNED_X -> ECHO_MUST_HAVE_OPPORTUNITY_TO_LEARN_X.
IF_ECHO_LEARNED_X_WITH_SUFFICIENT_COMPETENCE -> ECHO_MAY_TEACH_X_WITH_SOURCE_LIMITS_AND_CLASSIFICATION.

Enquanto a automacao de aprendizagem nao estiver comprovada:
LEARNING_CONFIRMED = testes tecnicos + validacao humana orientada usando API.

## REVISAO DE LINGUAGEM

IACOM_REVIEW = event-driven + max 60 days.
60_DAYS != FORCED_REWRITE.
Mudanca de norma/padrao nao ocorre automaticamente por benchmark tecnico.
