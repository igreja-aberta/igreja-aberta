# Módulo: Secretaria (Fase 2)

## Objetivo
Automatizar o balcão da secretaria paroquial.

## Funções
- **Intenções de missa:** cadastro por missa (data, horário, intenção, solicitante, oferta opcional), controle de limite por missa, relatório e lista para o celebrante. **Publicação do nome é opcional e só com autorização.**
- **Certidões e declarações auxiliares:** geração de modelos em PDF a partir dos registros, com numeração e controle de quem emitiu. **Documento de apoio, sem validade canônica própria** (a validar com a cúria).
- **Protocolo e atendimento:** registro de pedidos (batismo, casamento, declaração) com status e prazo.
- **Documentos e arquivo digital:** anexos organizados por pessoa ou assunto, com controle de acesso e prazo de retenção.
- **Livro de avisos e correspondência** (registro simples).
- **Modelos de documentos** editáveis pela paróquia (cartas, convites, declarações).
- **Mural interno** de recados para a equipe.
- **Contatos úteis** (fornecedores, outras paróquias, diocese).

## Regras
- Intenções de missa citam pessoas, inclusive falecidas: limitar a visibilidade pública e permitir ocultar.
- Todo documento emitido gera trilha de auditoria.

## Permissões
`secretaria.intencoes`, `secretaria.documentos`, `secretaria.certidoes`.

## Pronto quando
A secretaria atende pedido de intenção e declaração sem papel, com lista do dia para o padre.
