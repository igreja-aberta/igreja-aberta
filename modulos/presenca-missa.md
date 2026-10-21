# Módulo: Presença em missa (Fase 1)

## Objetivo
Registrar a presença de catequizandos nas missas, com regra de presença mínima definida pela paróquia.

## Funções
- **Cadastro das missas** (data, horário, local) a partir dos horários da paróquia, geradas automaticamente por período.
- **Registro por turma** em lista no celular, **ou por leitura de QR** de uma **carteirinha imprimível**. O QR contém só um identificador aleatório (nunca nome ou dado pessoal) e a leitura roda no navegador pela câmera.
- **Regra de presença mínima** por período (por exemplo, X missas por mês), configurável por etapa.
- **Relatórios** por catequizando e por turma, alerta de baixa presença e exportação em CSV.
- Presença de **outros grupos** (coroinhas, jovens) por reaproveitamento do mesmo mecanismo (fase 2).
- Carteirinha em PDF com layout configurável (nome da paróquia, logotipo e identificador).

## Regras
- Sem biometria e sem foto. Se a carteirinha for perdida, o identificador é regerado e o antigo invalidado.
- A leitura do QR funciona offline e sincroniza depois.

## Permissões
`missa.presenca` (catequista, coordenador), `missa.relatorios`.

## Pronto quando
Na saída da missa, a catequista lê as carteirinhas de uma turma em poucos minutos e o relatório mensal fica correto.
