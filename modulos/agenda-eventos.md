# Módulo: Agenda, salas e eventos (Fase 2)

## Objetivo
Uma agenda única da paróquia, sem conflito de salas e com inscrição de eventos.

## Funções
- **Agenda geral:** missas, confissões, reuniões, catequese, celebrações, com recorrência e cores por tipo.
- **Reserva de salas e espaços** com checagem de conflito, pedido de uso por pastorais e aprovação.
- **Eventos e festas** (quermesse, retiros, novenas, festa do padroeiro): descrição, local, data, vagas, preço opcional.
- **Inscrições** públicas com formulário, consentimento e lista de espera; confirmação por mensagem.
- **Pagamento de inscrição por Pix** (ver [pix](../integracoes/pix.md)) com baixa automática quando houver provedor configurado.
- **Voluntários do evento** ligados às escalas.
- **Orçamento do evento** ligado ao financeiro (receitas e despesas por evento).
- **Calendário público** incorporável no site e exportação em `.ics`.
- **Lista de presença** do evento por QR ou lista.

## Regras
- Conflito de sala bloqueia a reserva até haver aprovação de quem administra o espaço.
- Dados de inscritos só para a equipe do evento.

## Permissões
`agenda.ver`, `agenda.editar`, `salas.reservar`, `salas.aprovar`, `eventos.gerir`.

## Pronto quando
Um evento com inscrição paga por Pix é criado, divulgado no site e conciliado sem planilha.
