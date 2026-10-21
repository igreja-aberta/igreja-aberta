# 7. Licença e modelo de negócio

## Licença: MIT
O código é licenciado sob **MIT** (arquivo `LICENSE`). Ela é simples e favorece a adoção, mas tem uma consequência importante: **qualquer pessoa ou empresa pode usar, modificar, hospedar e vender o software, inclusive comercialmente, sem pagar nada e sem avisar**. A única exigência é manter o aviso de copyright e a licença no código. **Não é possível, com MIT, proibir o uso comercial nem exigir pagamento.**

## Saber quem usa: o que fazer e o que não fazer
**Não haverá telemetria oculta nem "ligar para casa" obrigatório.** Um sistema que guarda dados religiosos e de crianças e que envia informação sobre quem o instala, sem o consentimento claro, quebra a confiança das paróquias, tende a ser removido pela comunidade e pode ferir a LGPD. O projeto não fará isso.

O que é legítimo:
1. **Registro voluntário ("Registre sua paróquia"):** opt-in, com o que é enviado mostrado antes (nome da paróquia, cidade, versão, contato, e nada de dado de fiéis). Benefícios reais: aviso de falhas de segurança e atualizações, selo no site, presença no diretório público e prioridade nas dúvidas.
2. **Verificação de atualização opt-in:** consulta anônima da versão mais recente, desligada por padrão, documentada.
3. **Sinais públicos:** estrelas, forks e dependentes no GitHub, menções e buscas. Não identificam sozinhos quem usa comercialmente.
4. **Rodapé "Feito com Igreja Aberta":** ligado por padrão, com link para o projeto. Com MIT, não dá para obrigar a mantê-lo, mas a maioria mantém.
5. **Marca:** o nome e o logotipo "Igreja Aberta" **não** são licenciados pelo MIT. Uma política de uso da marca (e, se fizer sentido, registro no INPI) permite exigir que versões comerciais de terceiros não se apresentem como o projeto oficial.

## Como o Zenoi ganha dinheiro com MIT
O lucro vem do que o código aberto não entrega sozinho:
- **Serviços:** instalação, personalização, migração de dados, treinamento e suporte, com pacote e preço fechados.
- **Hospedagem gerenciada:** instalação mantida, atualizada e com backup pelo Zenoi, em mensalidade.
- **Módulos pagos (núcleo aberto + extensões):** por exemplo, integrações com provedores específicos de Pix, relatórios avançados, módulo diocesano. As extensões podem ter licença comercial própria porque são projetos separados do núcleo.
- **Doações e patrocínio** como complemento (GitHub Sponsors, Pix), com transparência dos custos.
- **Funil de consultoria:** quem chega pelo projeto e não consegue instalar ou personalizar chama o Zenoi.

## Alternativas de licença (decisão do mantenedor)
| Opção | O que permite | Prós | Contras |
|---|---|---|---|
| **MIT** (escolhida) | Tudo, inclusive uso comercial fechado | Máxima adoção e contribuição | Não dá para cobrar de quem usa comercialmente nem impedir versão fechada |
| AGPL-3.0 | Uso livre, mas quem oferece como serviço precisa abrir as modificações | Protege contra versão fechada hospedada | Alguns evitam; uso comercial continua permitido |
| Núcleo MIT + extensões comerciais (open core) | Núcleo livre e extensões pagas | Receita previsível sobre o que é diferencial | Exige separar bem o que é núcleo e extensão |
| Licença "source-available" (por exemplo, não comercial) | Código visível, uso comercial só com licença | Permite cobrar quem usa comercialmente | **Deixa de ser open source** no sentido da OSI, afasta contribuição e pode afastar paróquias |

Conferir a escolha final e o texto da política de marca com um advogado.
