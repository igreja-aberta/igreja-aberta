# Integração: API pública

## Objetivo
Permitir que sites, aplicativos e outras paróquias usem os dados abertos do sistema.

## Versão pública (sem autenticação, com cache e limite de requisições)
- `GET /api/v1/calendario/{AAAA-MM-DD}`: celebração, tempo litúrgico, cor e ciclo do dia.
- `GET /api/v1/calendario/{AAAA}`: o ano inteiro.
- `GET /api/v1/horarios`: horários de missa e confissão da paróquia.
- `GET /api/v1/avisos`: avisos publicados.
- `GET /api/v1/eventos`: eventos públicos.

## Versão autenticada (fase 2 em diante)
- Token por usuário ou aplicação, com escopos por módulo e papéis iguais aos do painel.
- Recursos: paroquianos, turmas, presenças, escalas, contribuições (conforme a permissão).
- Webhooks de saída opcionais (novo evento, pagamento confirmado).

## Regras
- Versionamento em `/api/v1`; mudanças que quebram viram `/api/v2`.
- Respostas em JSON, erros padronizados, documentação em OpenAPI.
- **Dados pessoais nunca na API pública.**
- Limite de requisições por IP e por token.

## Documentação
OpenAPI em `docs/openapi.json` e exemplos de `curl` por endpoint.
