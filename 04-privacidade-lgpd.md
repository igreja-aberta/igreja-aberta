# 4. Privacidade e LGPD

> Documento técnico de orientação, **não é parecer jurídico**. Os modelos precisam de revisão de advogado antes do uso real.

## Quem é quem
- **Paróquia = controladora** dos dados cadastrados (decide para que e como usar).
- **Software = ferramenta.** Quem hospeda o servidor pode ser operador (por exemplo, o Zenoi quando presta hospedagem paga, mediante contrato).
- O projeto **não coleta dados** das paróquias que o instalam.

## Dados sensíveis neste sistema
- **Convicção religiosa** (participação em sacramentos, catequese, pastorais) é dado pessoal sensível.
- **Crianças e adolescentes** (catequese): tratamento no melhor interesse do menor, com consentimento específico de um dos pais ou responsável.
- Dados financeiros de contribuintes (dízimo/ofertas) também pedem cuidado.

## Regras do produto
1. **Coletar o mínimo.** Catequizando: nome, nascimento, turma, responsável e contato. Sem foto, documento ou endereço completo na versão inicial.
2. **Consentimento registrado** (data, versão do termo, quem registrou) para menores e para comunicações.
3. **Papéis e permissões** restritos (ver [03](03-permissoes.md)).
4. **Direitos do titular:** exportar e apagar os dados de uma pessoa a pedido, com fluxo no painel.
5. **Retenção configurável** e anonimização depois do prazo.
6. **Auditoria** de acessos e alterações em dados sensíveis.
7. **Transparência:** aviso de privacidade público do site da paróquia (modelo incluído).
8. **Segurança:** HTTPS, senhas com hash, backups protegidos, atualizações. Nenhum dado pessoal em log.
9. **Publicação:** nomes em intenções de missa, aniversariantes e fotos só com autorização e opção de ocultar.
10. **Incidentes:** modelo de procedimento para vazamento (quem avisar e em quanto tempo), a validar com advogado.

## Modelos a entregar (marcados "revisar com advogado")
Termo de consentimento dos responsáveis, termo para adultos, aviso de privacidade, política de retenção, contrato de hospedagem e operação (para o serviço pago).
