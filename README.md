# CI/CD para Aplicação Web

## Objetivo

O objetivo deste projeto é criar uma solução completa de entrega contínua (CI/CD) para uma página web simples. 
Este repositório contém a configuração necessária para Dockerização, integração contínua e entrega contínua da aplicação.

## Estrutura Proposta

### Dockerização da Aplicação

- **Dockerfile**: Cria um ambiente isolado e replicável para a aplicação, incluindo todas as dependências.
- **Multi-stage builds**: Otimiza a imagem final, separando as etapas de construção e execução.
- **Best practices**: Seguir as melhores práticas do Docker para criar imagens seguras e eficientes.

### Fluxo de Trabalho CI/CD no GitHub Actions

1. **Trigger**: Acionamento automático a cada push na branch principal.
2. **Build**: Construção da imagem Docker utilizando o Dockerfile.
3. **Push**: Publicação da imagem no Docker Hub.
4. **Deploy**: Implantação da imagem no Google Kubernetes Engine (GKE), utilizando um manifesto Kubernetes.

## Tecnologias Utilizadas

- Docker
- GitHub Actions
- Kubernetes
- Nginx (para servir a aplicação web)
