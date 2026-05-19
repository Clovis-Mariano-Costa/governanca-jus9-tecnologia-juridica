# Regra - Servidor local no computador pessoal para MVP Jus 9

## Principio

Computador pessoal pode funcionar como servidor em menor escala para desenvolvimento, demonstracao e teste do MVP Jus 9, desde que o uso seja local, controlado e sem dados reais sensiveis.

## Uso permitido

- Rodar APP/PWA em `localhost` para teste no proprio computador.
- Rodar em rede Wi-Fi local para teste visual no celular, quando necessario.
- Demonstrar telas, fluxos, responsividade, navegacao, instalacao PWA e comportamento offline.
- Validar fluxo de WhatsApp somente com arquivos ficticios ou demonstrativos.

## Uso proibido sem camada de producao

- Inserir dados reais de clientes, processos, documentos, WhatsApp ou identificacao pessoal sensivel.
- Expor o computador pessoal diretamente para a internet publica.
- Usar HTTP simples para trafego real fora de teste local.
- Transformar pasta privada, cofre, WhatsApp extraido ou transcricoes em conteudo publico.

## Requisitos antes de uso real

- HTTPS.
- Autenticacao.
- Controle de permissao por perfil.
- Logs de acesso e auditoria.
- Cofre criptografico.
- Politica de backup.
- Consentimento e classificacao de dados.

## Padrao tecnico atual

- Repertorio institucional: `servidor-local-iniciar.ps1` na porta `8099`.
- Repertorio MVP: `servidor-local-iniciar.ps1` na porta `8098`.
- Modo local padrao: `127.0.0.1`.
- Modo rede local: usar `-RedeLocal` apenas em Wi-Fi confiavel.

Esta regra integra o Protocolo Mao na Massa: construir o que for possivel agora, sem fingir que MVP local ja e infraestrutura de producao.
