# 5. Modo demonstração

Objetivo: a demo pública em servidor gratuito dá a **sensação de usar o sistema** sem salvar nada e sem risco de abuso.

## Comportamento
- `DEMO_MODE=true` ativa o modo. Dados **fictícios e sempre iguais**, gerados por `php artisan demo:preparar`. O banco é recriado a cada inicialização do servidor.
- **Nada é salvo:** toda requisição que altera dados roda dentro de uma transação **sempre desfeita**. O formulário valida normalmente e o sistema mostra a mensagem em destaque: "Modo demonstração: nada foi salvo. Instale na sua paróquia para usar de verdade."
- Efeitos colaterais desligados: sem e-mail, sem mensagens, sem upload, sem Pix real (cobranças de exemplo), sem filas.
- Botões "Entrar como administrador / secretaria / tesouraria / catequista" sem senha.
- **Faixa fixa "DEMONSTRAÇÃO"** em todas as páginas, `noindex`, limite de requisições, limite de tamanho de campos e escape de HTML.
- Sessão e cache fora do banco.

## Hospedagem
Contêiner pequeno em plano gratuito (por exemplo, Render). O serviço pode "dormir" sem acessos e levar cerca de um minuto para acordar; a demo mostra uma página de carregamento amigável. Limites dos planos gratuitos mudam: conferir no dia da publicação.

## Testes obrigatórios
- Em cada módulo, criar, editar e apagar no modo demo e provar que o banco continua idêntico.
- O modo demo não pode ser ligado por engano em produção (aviso na inicialização e variável explícita).
