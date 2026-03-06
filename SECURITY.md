# Security Policy

## Versões Suportadas

Apenas a versão mais recente do NVN.PLUS recebe atualizações de segurança.

| Versão  | Suportada          |
| ------- | ------------------ |
| 1.1.9   | :white_check_mark: |
| < 1.1.8 | :x:                |

## Reportando uma Vulnerabilidade

Se você descobriu uma vulnerabilidade de segurança no NVN.PLUS, **não abra uma issue pública**. Vulnerabilidades divulgadas publicamente antes de serem corrigidas colocam todos os usuários em risco.

### Como Reportar

1. **E-mail**: Envie um relatório detalhado para **security@nvn.plus** com o assunto `[SECURITY] Descrição breve da vulnerabilidade`
2. **GitHub**: Utilize o recurso de [reporte privado de vulnerabilidades](https://github.com/nvngroup/nvnplus/security/advisories/new) do GitHub

### O que Incluir no Relatório

- Descrição clara da vulnerabilidade
- Passos para reproduzir o problema
- Impacto potencial (ex: acesso não autorizado, vazamento de dados, etc.)
- Versão do NVN.PLUS afetada
- Prova de conceito ou screenshots, se disponível

### O que Esperar

| Etapa                              | Prazo estimado |
| ---------------------------------- | -------------- |
| Confirmação de recebimento         | 48 horas       |
| Avaliação inicial da vulnerabilidade | 5 dias úteis  |
| Correção e publicação de patch     | 30 dias        |

Após a correção ser lançada, a vulnerabilidade será divulgada publicamente com os devidos créditos ao responsável pelo reporte (caso desejado).

### Escopo

São consideradas vulnerabilidades elegíveis:

- Execução remota de código
- Acesso não autorizado a dados de outros tenants
- Vazamento de credenciais ou tokens
- Injeção de SQL, XSS armazenado ou CSRF crítico
- Falhas de autenticação ou autorização

Não são elegíveis:

- Vulnerabilidades em versões não suportadas
- Problemas em dependências de terceiros já conhecidos publicamente
- Ataques que requerem acesso físico ao servidor
