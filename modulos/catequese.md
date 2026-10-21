# Módulo: Catequese (Fase 1)

## Objetivo
Organizar turmas, catequizandos, encontros e frequência com o mínimo de dados e o máximo de praticidade para a catequista.

## Funções
- **Turmas:** nome, etapa ou ano, dia e horário, local, catequistas responsáveis.
- **Catequizandos:** nome, data de nascimento, turma, responsáveis (nome e telefone), observações curtas. **Consentimento do responsável** registrado (data, versão do termo, quem registrou).
- **Encontros:** data, tema e observações. **Presença** por encontro (presente, ausente, justificado), marcada pelo celular em lista com toque grande.
- **Frequência:** relatório por turma e por catequizando, limite de faltas configurável com alerta, exportação em CSV e impressão em PDF.
- **Transferência de turma** e histórico da trajetória na catequese (etapas cursadas).
- **Contato com responsáveis** pelo módulo de comunicação, com modelos de mensagem ("falta no encontro", "aviso de evento") e consentimento respeitado.
- **Lista de espera e inscrições** online simples (fase 2, formulário público com consentimento).
- **Materiais:** campo de links para materiais da paróquia (não distribui conteúdo protegido).
- **Fim de ano:** fechar turma, registrar conclusão da etapa e gerar a lista para sacramentos (liga com [sacramentos](sacramentos.md)).

## Regras de privacidade
- Sem foto, documento ou endereço completo na versão inicial. Exportar e apagar dados a pedido da família. Retenção configurável e anonimização depois do prazo (ver [04](../04-privacidade-lgpd.md)).
- Catequista só enxerga as próprias turmas.

## Permissões
`catequese.ver`, `catequese.presenca`, `catequese.editar`, `catequese.relatorios`, `catequese.exportar`.

## Pronto quando
Uma catequista consegue registrar a presença de uma turma de 25 crianças em menos de 2 minutos no celular e o coordenador tira o relatório do ano.
