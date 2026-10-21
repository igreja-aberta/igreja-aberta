# Módulo: Calendário litúrgico (Fase 1)

## Objetivo
Mostrar o calendário litúrgico correto e oferecê-lo por API, sem distribuir textos protegidos.

## Funções
- **Cálculo por regra:** data da Páscoa, tempos litúrgicos (Advento, Natal, Tempo Comum, Quaresma, Tríduo Pascal, Tempo Pascal), **cor litúrgica**, ciclo dominical (A, B, C) e ano par ou ímpar.
- **Solenidades, festas e memórias** do calendário geral e as **próprias do Brasil**, com fonte registrada (ver [fontes](../08-fontes-e-cuidados.md)).
- **Celebrações locais:** padroeiro, dedicação da igreja e festas da comunidade, cadastradas pelo administrador.
- Visões mensal, semanal e do dia, com cor e celebração. Programação semanal para o site e para impressão (horários de missa + celebração + cor).
- **Santo ou memória do dia:** só nome e classificação. Biografia somente com fonte livre.
- **Referências das leituras:** campo opcional, preenchido pela paróquia, com link para fonte licenciada. O sistema não traz os textos.
- **API pública** `GET /api/v1/calendario/{AAAA-MM-DD}` e `GET /api/v1/calendario/{AAAA}`, com cache e limite de requisições.
- Widget incorporável ("hoje na liturgia") para sites de terceiros.

## Regras
- Datas que não puderem ser confirmadas em fonte **não entram** até a confirmação.
- Testes com datas conhecidas (Páscoa de vários anos, Quarta de Cinzas, Pentecostes, Advento, ciclos), com a fonte de cada expectativa.

## Permissões
`liturgia.ver` (público), `liturgia.editar_local` (administrador, secretaria).

## Pronto quando
Calendário correto para um intervalo de anos validado contra fonte oficial e revisado por alguém com conhecimento litúrgico.
