# Módulo: Paroquianos e famílias, o CRM paroquial (Fase 2)

## Objetivo
Cadastro único e respeitoso das pessoas e famílias da comunidade, base para os demais módulos.

## Funções
- **Pessoa:** nome, contato, nascimento (opcional), estado civil (opcional), comunidade ou capela, situação (ativo, mudou, falecido), observações. **Só o necessário**; campos sensíveis são opcionais e restritos.
- **Famílias e vínculos:** responsáveis, filhos, padrinhos. Uma pessoa pode estar em várias famílias.
- **Participação:** pastorais, movimentos, catequese e sacramentos recebidos, ligados aos outros módulos.
- **Busca e filtros** por nome, comunidade, pastoral, faixa etária. Etiquetas livres.
- **Aniversariantes** com opção de publicar apenas para quem autorizou.
- **Visitas e acompanhamento pastoral** (registro simples para ministros e visitadores, com acesso restrito).
- **Importação** de planilha CSV com pré-visualização e relatório de erros, e **exportação**.
- **Duplicados:** detecção e mesclagem assistida.
- **Preferências de contato** (WhatsApp, e-mail, telefone, não contatar) e consentimentos.
- **Cartão do paroquiano** opcional (QR com identificador aleatório).

## Regras
- Dados de religião são **sensíveis**: acesso mínimo, auditoria e exclusão a pedido.
- Nada de dados públicos sem autorização.

## Permissões
`pessoas.ver`, `pessoas.editar`, `pessoas.exportar`, `pessoas.sensivel`.

## Pronto quando
A secretaria importa a planilha existente, encontra uma família em segundos e todos os módulos reaproveitam o mesmo cadastro.
