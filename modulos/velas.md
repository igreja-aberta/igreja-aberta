# Módulo: Vela virtual de 7 dias (Fase 1)

## Objetivo
Permitir que qualquer pessoa acenda uma vela virtual a um santo ou devoção, sem cadastro e sem anúncio.

## Funções
- Fluxo: escolher o estilo da vela, escolher o santo ou devoção, escrever uma intenção (opcional), acender.
- **Vida de 7 dias** (configurável): a cera diminui visualmente e a chama se apaga no fim, com mensagem serena.
- Várias velas ao mesmo tempo (limite configurável) e página "Minhas velas".
- **Sem dados no servidor:** o estado fica no navegador (`localStorage`, esquema versionado). Se o armazenamento estiver bloqueado, funciona em memória e avisa.
- **Link de recuperação** com o estado no fragmento da URL (nunca enviado ao servidor) para abrir a vela em outro aparelho.
- **Lembrete `.ics`** do fim da vela.
- Lista de santos e devoções **cadastrada pela paróquia**, com pacote padrão de devoções comuns no Brasil (só nome e ilustração original).
- Chama animada em SVG/CSS, som ambiente opcional desligado por padrão, chama estática com movimento reduzido.
- Opcional (desligado por padrão): link de WhatsApp para enviar um pedido de oração à paróquia.

## Regras
- A intenção escrita **nunca sai do aparelho** e o aviso é claro na tela.
- Sem rastreamento, sem cookies, sem contagem global na versão inicial. O mural coletivo é ideia futura, exige servidor e proteção contra abuso.

## Permissões
Público. Administração dos santos: `velas.editar`.

## Pronto quando
Acender, recarregar, esperar o tempo passar (teste com relógio simulado) e ver a cera diminuir e a chama apagar, tudo sem requisição externa.
