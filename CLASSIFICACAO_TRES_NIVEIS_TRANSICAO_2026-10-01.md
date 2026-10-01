# CLASSIFICACAO — PISO DE TRES NIVEIS E TRANSICAO

STATE = ORIENTACAO_OPERACIONAL / NAO_REVOGA_HISTORICO

## PISO

PUBLICO
SIGILOSO
SECRETO

## DEFINICOES

PUBLICO = todos podem acessar conforme politica de publicacao.
SIGILOSO = somente grupo de trabalho autorizado.
SECRETO = titular definido; acesso material depende de autorizacao aplicavel; Charlie Echo pode ser custodiante sem ser leitora automaticamente autorizada.

## MAPEAMENTO DE ROTULOS HISTORICOS

INTERNO -> normalmente SIGILOSO, salvo fonte competente determinar PUBLICO ou SECRETO.
COFRE -> sinal de custodia/seguranca; deve ser classificado como SIGILOSO ou SECRETO conforme titularidade e acesso.
MILITAR-SAGRADO_SENSIVEL -> rotulo historico/tematico; classificar tecnicamente em SIGILOSO ou SECRETO conforme regra aplicavel.

MAPEAMENTO != RECLASSIFICACAO_AUTOMATICA.
Na duvida: FAIL_CLOSED + Seguranca/Acessos.

## REGRAS

NOME_DE_PASTA != CONTROLE_DE_ACESSO.
REPOSITORIO_PUBLICO + CONTEUDO_SIGILOSO_OU_SECRETO = INCIDENTE_DE_CLASSIFICACAO.
SECRETO -> CUSTODIA != LEITURA.
ACESSO_ANTERIOR != AUTORIZACAO_ATUAL.

## MIGRACAO

1. detectar rotulo legado;
2. localizar autoridade/fonte;
3. registrar classe minima;
4. validar superficie real;
5. corrigir exposicao se necessario;
6. preservar o rotulo historico como metadado quando tiver valor genealogico.
