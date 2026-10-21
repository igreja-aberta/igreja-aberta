# Integração: Mensageria (WhatsApp e e-mail)

## Princípios
- **Interface própria** (`MensagemProvider`) com adaptadores trocáveis, como no Pix. A paróquia escolhe e configura o canal.
- **Só envia a quem consentiu**; todo envio permite descadastro.
- Tarefas na fila com retentativa e limite de envios.

## Canais
- **E-mail** (SMTP configurável): sempre disponível.
- **WhatsApp:** pelo provedor que a paróquia escolher (por exemplo, a API oficial da Meta ou um provedor homologado). Regras, custos e aprovação de modelos variam e mudam (a verificar). A abertura por link `wa.me` (sem API) é a alternativa gratuita para contato individual.

## Funções
- Envio de texto e de modelos aprovados.
- Estado de entrega e histórico.
- Recebimento de respostas (fase futura) para atendimento simples.
- Variáveis em modelos (nome, data, local).

## Segurança
Credenciais criptografadas por paróquia, webhooks validados, nenhum conteúdo sensível em log.
