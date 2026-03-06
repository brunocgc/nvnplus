# nvnplus (brunocgc)

Repositório de captura de issues de clientes finais para o projeto [nvngroup/nvnplus](https://github.com/nvngroup/nvnplus).

## Como funciona

Quando uma issue é aberta (ou alterada) neste repositório, o workflow de CI/CD a transporta automaticamente para [nvngroup/nvnplus](https://github.com/nvngroup/nvnplus).

### Ações suportadas

| Ação neste repositório | Ação em nvngroup/nvnplus |
|------------------------|--------------------------|
| Issue aberta (`opened`) | Nova issue criada |
| Issue editada (`edited`) | Issue correspondente atualizada |
| Issue fechada (`closed`) | Issue correspondente fechada |
| Issue reaberta (`reopened`) | Issue correspondente reaberta |
| Issue deletada (`deleted`) | Issue correspondente fechada com aviso |

## Configuração

Para que o workflow funcione, é necessário configurar um token com permissão de escrita no repositório `nvngroup/nvnplus`:

1. Gere um **Personal Access Token (PAT)** ou **Fine-grained token** com permissão `Issues: Read and Write` no repositório `nvngroup/nvnplus`.
2. No repositório `brunocgc/nvnplus`, acesse **Settings → Secrets and variables → Actions**.
3. Crie um novo secret chamado `MIRROR_PAT` com o valor do token gerado.

> **Nota:** O `GITHUB_TOKEN` padrão do GitHub Actions só tem acesso ao repositório atual. Para transportar issues entre repositórios, é necessário um PAT configurado como secret `MIRROR_PAT` com acesso ao repositório de destino.
