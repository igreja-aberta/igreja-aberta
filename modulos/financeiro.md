# Módulo: Financeiro (Fase 3)

> Regras fiscais, contábeis e de prestação de contas de entidades religiosas **precisam ser validadas com um contador e com a diocese** antes de virarem regra do sistema (a validar). O módulo é de **controle e transparência**, não faz contabilidade oficial.

## Objetivo
Dar à tesouraria e ao conselho econômico controle claro de entradas e saídas, com contribuição por Pix e prestação de contas.

## Funções
- **Contribuições:** dízimo, ofertas, doações para obras, campanhas e festas. Por pessoa (opcional e com autorização) ou anônimas.
- **Pix:** QR e "copia e cola" para contribuição; cobrança dinâmica por provedor com baixa automática (ver [pix](../integracoes/pix.md)).
- **Dízimo recorrente:** lembrete mensal e, quando disponível, cobrança recorrente por Pix (a verificar a situação atual e as regras do provedor).
- **Caixa e contas:** caixa da secretaria, contas bancárias, transferências internas, abertura e fechamento diário.
- **Plano de contas simples** (categorias de receita e despesa) e **centros de custo** (pastorais, festas, obras, comunidades).
- **Contas a pagar e a receber** com vencimento, anexo de comprovante e alerta.
- **Conciliação:** importação de extrato (OFX ou CSV) e casamento com lançamentos e Pix recebidos.
- **Recibos** de contribuição e comprovantes numerados.
- **Prestação de contas:** relatórios mensais e anuais por categoria e centro de custo, versão para o conselho econômico e versão resumida para a comunidade (sem nomes de contribuintes).
- **Orçamento e previsão** por centro de custo.
- **Relatório de dizimistas** com acesso muito restrito.
- **Campanhas** (reforma, construção) com meta e acompanhamento público opcional, sem identificar doadores.
- **Fechamento de período** que trava lançamentos antigos; correção por estorno, nunca por edição.

## Regras de segurança
- Lançamentos **imutáveis**: correção cria um estorno e um novo lançamento. Trilha de auditoria completa.
- Acesso restrito: tesouraria e conselho econômico; coordenador de pastoral nunca vê o financeiro geral.
- 2FA recomendado para tesouraria e administrador.
- **O dinheiro nunca passa pelo projeto nem por conta do Zenoi:** o Pix vai direto para a conta da paróquia no provedor que ela contratar.
- Dados de contribuintes seguem a LGPD (ver [04](../04-privacidade-lgpd.md)).

## Permissões
`financeiro.ver`, `financeiro.lancar`, `financeiro.estornar`, `financeiro.fechar`, `financeiro.relatorios`, `financeiro.contribuintes`.

## Pronto quando
A tesouraria fecha o mês com extrato conciliado, o conselho recebe o relatório e nenhum lançamento pode ser alterado sem rastro.
