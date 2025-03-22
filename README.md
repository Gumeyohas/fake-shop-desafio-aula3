# Fake Shop - Desafio Aula 2
Este repositório contém a solução do desafio da **Aula 2**, que envolve a arquitetura do kubernetes (deployment, replicaset, pods, services), orquestração de contêineres e etc...

## 🚀 Tecnologias Utilizadas

- **Kubernetes**: Para criação e execução de contêineres.
- **Docker**: Para criação e envio das imagens de contêiner.
- **DigitalOcean Kubernetes (DOKS)**: Cluster Kubernetes na DigitalOcean.

## 📌 Desafios Concluídos

- ✅ Provisionamento de um cluster Kubernetes Digital Ocean
- ✅ Cluster acessível via LoadBalancer.
- ✅ Construção de um **Manifesto Kubernetes** 
- ✅ Criação dos services para expor a aplicação: ClusterIP e LoadBalancer 
- ✅ Criação dos Deployments para gerenciarem os pods da aplicação
- ✅ Troca de versões da aplicação sem downtime (é possível ver as versões no docker hub)
- ✅ Deploy da aplicação no cluster Kubernetes.

### Para mais detalhes sobre a publicação no Docker Hub, consulte o arquivo dockerhub.md.

## Variável de Ambiente
DB_HOST	=> Host do banco de dados PostgreSQL.

DB_USER => Nome do usuário do banco de dados PostgreSQL.

DB_PASSWORD	=> Senha do usuário do banco de dados PostgreSQL.

DB_NAME	=>	Nome do banco de dados PostgreSQL.

DB_PORT	=>	Porta de conexão com o banco de dados PostgreSQL.
