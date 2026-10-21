# Integração: Pix

## Princípios
1. **O dinheiro vai direto para a conta da paróquia.** O projeto e o Zenoi não recebem, guardam nem intermediam valores.
2. **Cada paróquia contrata o seu provedor** (banco ou instituição de pagamento) e configura as credenciais no painel, guardadas criptografadas.
3. **Funciona sem provedor**: o nível 1 abaixo não exige integração.
4. Regras e tarifas variam por provedor e mudam: conferir na documentação do provedor escolhido (a verificar).

## Níveis
### Nível 1: Pix estático (sem provedor)
- Gera o **código "copia e cola" e o QR** no padrão do Pix (BR Code) **localmente**, com a chave Pix da paróquia, nome e cidade.
- Valor livre ou fixo. Serve para contribuição e inscrição simples.
- **Sem baixa automática:** o recebimento é conferido na conciliação por extrato (ver [financeiro](../modulos/financeiro.md)).

### Nível 2: Cobrança dinâmica por provedor
- Interface própria `PixProvider` com `criarCobranca`, `consultarCobranca`, `cancelarCobranca`, `devolver` e tratamento de **webhook** de pagamento.
- Cada provedor é um adaptador separado e trocável (um por paróquia).
- **Baixa automática:** ao confirmar o pagamento, o sistema registra a contribuição, emite o recibo e atualiza o evento ou a inscrição.
- **Idempotência** (identificador único por cobrança) e **conferência de valor e identificador** antes de dar baixa.
- **Webhook seguro:** validação conforme o provedor (assinatura, certificado ou lista de IPs), tentativas repetidas tratadas sem duplicar baixa.
- **Conciliação:** casa cobranças, Pix recebidos e extrato; aponta divergências.
- **Ambiente de testes (sandbox)** do provedor usado nos testes automatizados.

### Nível 3: Recorrência (dízimo mensal)
- Primeiro, lembrete mensal com link ou QR. Depois, cobrança recorrente **se o provedor oferecer o recurso de Pix recorrente** e a paróquia optar (a verificar a situação atual, as regras do Banco Central e a disponibilidade no provedor).
- O fiel autoriza e pode cancelar a qualquer momento. Nada de cobrança sem consentimento registrado.

## Dados
`contribuicoes`, `cobrancas_pix` (identificador, valor, status, expiração), `eventos_pix` (webhooks recebidos, imutável), ligação opcional com a pessoa.

## Segurança e privacidade
- Credenciais criptografadas por paróquia, nunca em log. Webhooks com limite de requisições.
- Contribuinte identificado só com autorização; contribuição anônima é aceita.
- Divulgação pública de valores sem nomes.
- Estornos por lançamento novo, nunca por edição.

## Pronto quando
Uma contribuição por Pix gera recibo, aparece no caixa e concilia com o extrato, e uma inscrição paga confirma sozinha.
