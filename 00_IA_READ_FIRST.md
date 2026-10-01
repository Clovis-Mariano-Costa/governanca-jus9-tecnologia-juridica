# IA READ FIRST — GOVERNANCA JUS 9

SCHEMA = JUS9_REPO_ENTRY_V1
STATE = DRAFT_BRANCH
PRIMARY_READER = IA
CLASSIFICATION = PUBLICO_SANITIZADO
RULES = IA_FIRST + LINK_FIRST + EVIDENCE_FIRST + FAIL_CLOSED

## PURPOSE
Repositorio de governanca geral/transversal e historica da Jus 9.
Nao presumir que todo arquivo aqui esta vigente.

## START
1. Leia README.md.
2. Distinga VIGENTE | PROPOSTA | HISTORICO | SUPERADO | RASCUNHO.
3. Consulte o Vademecum/catalogo antes de afirmar vigencia.
4. Consulte o mapa de comunicacao para Codex/Legislador/Mestre.
5. Preserve genealogia e autoridade.

COMMUNICATION_MAP = https://docs.google.com/document/d/1xaQXGbZ0LdHaipUhLewWtPmoajEeUKS9s1RChjMjWWU/edit
GITHUB_INVENTORY = https://docs.google.com/document/d/1MfktKZtfL9imoyZ9DWDmBe3-z2jE_2HkRcTXydPSrPI/edit

## CORE
DOCUMENT_EXISTS != VIGENT
MERGE != PROMULGATION
PR_DRAFT != APPROVAL
LOWER_TOKEN_COST != AUTHORITY
NORM_CONFLICT -> LEGISLADOR
IMPLEMENTATION -> CODEX
CROSS_ROLE_PRIORITY -> MESTRE

## SECURITY
PUBLIC_REPO_SECRET = PROIBIDO
COFRE/SECRET/SIGILOSO name = classification signal, not protection.
Secret material -> route to Security/Access workflow; do not copy into this repository.

## NEXT
Reconciliar Elefante Colorido, Mao na Massa, IACOM, C0/C1/C2 e ProtocolRegistry sem criar canones concorrentes.
