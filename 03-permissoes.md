# 3. Papéis e permissões

Permissões no formato `modulo.acao`. A paróquia pode criar papéis próprios a partir dos modelos abaixo (a partir da fase 2).

| Papel | Quem | Acesso resumido |
|---|---|---|
| administrador | Padre e secretaria | Tudo, exceto o que for restrito por política |
| secretaria | Secretaria paroquial | Paroquianos, sacramentos, secretaria, agenda, comunicação |
| tesouraria | Tesoureiro | Financeiro completo e patrimônio |
| conselho_economico | Conselho econômico | Leitura do financeiro e prestação de contas |
| coordenador_catequese | Coordenação | Catequese inteira |
| catequista | Catequista | Só as próprias turmas: presença e observações |
| coordenador_pastoral | Coordenador | Sua pastoral: pessoas, escalas, eventos |
| voluntario | Voluntário | Ver a própria escala e confirmar presença |
| leitura | Consulta | Apenas leitura de módulos liberados |

## Regras
- **Mínimo necessário:** cada papel vê só o que precisa. Dados de menores e financeiros têm acesso mais restrito.
- Catequista nunca vê turma de outro catequista; coordenador de pastoral nunca vê o financeiro.
- Alterações de papel, exportações e exclusões geram registro de auditoria.
- Testes automatizados cobrem a matriz inteira (papel × permissão × resultado esperado).
- 2FA recomendado para administrador e tesouraria.
