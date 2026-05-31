# IAM Lab

## Objetivo
Configurar identidades e controle de acesso na AWS seguindo 
o princípio do menor privilégio (Least Privilege).

## Serviços utilizados
- AWS IAM (Identity and Access Management)

## Atividades realizadas
1. Criação de usuário IAM
2. Criação de grupo
3. Associação de usuário ao grupo
4. Anexação de políticas de permissão
5. Validação de acesso

## O que aprendi
- Como funciona o modelo de permissões da AWS (usuários, grupos, políticas)
- Por que nunca usar o usuário root para tarefas do dia a dia
- Como o princípio de menor privilégio reduz a superfície de ataque
- Diferença entre políticas gerenciadas pela AWS e políticas customizadas

## Relevância para segurança
IAM mal configurado é uma das principais causas de 
incidentes em cloud. Controle de acesso granular é 
fundamental para o modelo Zero Trust na AWS.


## Evidências

### Criação de usuário
![Criação de usuário](https://github.com/hugo-rich4rd/aws-security-lab/commit/8c7e8b17fac38c1a9e156d548fd46022220f20d2)

### Criação de grupo
![Criação de grupo](https://github.com/hugo-rich4rd/aws-security-lab/commit/7563c7287a264499738ede3a9d68834d5fee3167)

### Associação ao grupo
![Usuário no grupo](https://github.com/hugo-rich4rd/aws-security-lab/commit/ede1350e615f60dc5a2763e00988ae3542cbce3f)
