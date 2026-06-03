# AWS CLI Lab

## Objetivo
Configurar acesso programático seguro à AWS via CLI, aplicando princípio de least privilege
com usuário IAM dedicado — evitando o uso das credenciais root.

## Contexto de Segurança
O acesso programático mal configurado é uma das principais causas de comprometimento
de contas AWS. Este lab estabelece a base segura para automações futuras com Boto3.

## Etapas Realizadas

1. Instalação da AWS CLI v2 no Windows.
2. Criação de usuário IAM dedicado (sem console access, apenas programático).
3. Geração de Access Key com escopo limitado de permissões.
4. Configuração do perfil local com `aws configure`.
5. Validação das credenciais com `aws configure list`.
6. Confirmação da identidade via `aws sts get-caller-identity`.

## Comandos Utilizados

```bash
aws --version
aws configure
aws configure list
aws sts get-caller-identity
```

## Decisões de Segurança

- **Usuário IAM separado** — credenciais root nunca utilizadas para acesso programático.
- **Permissões mínimas** — usuário criado com apenas as permissões necessárias para o lab.
- **Screenshots sanitizadas** — Account ID, ARN e UserId ocultados nas evidências.
- **Sem hardcode de credenciais** — nenhuma chave exposta em código ou arquivos do repositório.

## Aprendizados

- Configuração segura de credenciais na AWS CLI.
- Diferença entre acesso via console e acesso programático no IAM.
- Validação de identidade AWS via STS (`get-caller-identity`).
- Boas práticas de OPSEC em ambientes de estudo.

## Próximos Passos

- Automatizar auditoria de usuários IAM sem MFA com Python/Boto3.
- Configurar múltiplos profiles na CLI para diferentes contas/ambientes.

## Referências

- [AWS CLI Installation](https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html)
- [IAM Best Practices](https://docs.aws.amazon.com/IAM/latest/UserGuide/best-practices.html)
