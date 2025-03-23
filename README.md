# Desafio CI/CD - Fake Shop aula 3

Este repositório contém a implementação de uma pipeline CI/CD utilizando GitHub Actions para automatizar o processo de build e deploy da aplicação Fake Shop.

## Visão Geral

A pipeline realiza as seguintes etapas:
1. **CI (Continuous Integration)**:
   - Faz checkout do código.
   - Faz login no Docker Hub.
   - Constrói a imagem Docker e publica no Docker Hub.

2. **CD (Continuous Deployment)**:
   - Obtém o código.
   - Configura o contexto do Kubernetes.
   - Realiza o deploy da aplicação no Kubernetes aplicando os manifests necessários.

## Requisitos

Antes de executar a pipeline, certifique-se de configurar os seguintes segredos no repositório do GitHub:
- `DOCKERHUB_USERNAME`: Nome de usuário do Docker Hub.
- `DOCKERHUB_TOKEN`: Token de acesso ao Docker Hub.
- `K8S_KUBECONFIG`: Configuração do kubeconfig para acessar o cluster Kubernetes.

## Estrutura do Repositório

```
.
├── .github/workflows/
│   ├── ci-cd.yml  # Pipeline do GitHub Actions
├── src/
│   ├── Dockerfile  # Definição da imagem Docker
├── k8s/
│   ├── deployment.yaml  # Manifesto para o Kubernetes
├── README.md  # Instruções de execução
```

## Como Executar

### 1. Configurar Segredos no GitHub
No repositório forkado, acesse **Settings > Secrets and variables > Actions** e adicione os segredos listados acima.

### 2. Commit na Branch `main`
A pipeline é acionada automaticamente ao realizar um push na branch `main`. Caso queira iniciar manualmente, utilize o `workflow_dispatch` pelo GitHub Actions.

### 3. Monitorar a Execução
Acompanhe o progresso da pipeline acessando a aba **Actions** no GitHub.

## Contato
Caso encontre algum problema ou tenha dúvidas, abra uma issue no repositório.
