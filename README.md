# Lab Kubernetes: Frontend

## Resumo

Landing page de currículo estática, empacotada em uma imagem Docker com Nginx não-root e executada no Kubernetes local do Docker Desktop.

## O que foi implementado

- Landing page responsiva em HTML, CSS e JavaScript.
- Imagem `lab-frontend:local`, baseada em `nginx-unprivileged`.
- Deployment Kubernetes com três réplicas, verificações HTTP, limites de recursos e execução sem root.
- Service do tipo `LoadBalancer` na porta `8080`.

## Pré-requisitos

- Docker Desktop em execução, com Kubernetes habilitado.
- Docker CLI e `kubectl` instalados.
- Contexto Kubernetes do Docker Desktop selecionado.

## Estrutura

- `frontend/`: página estática e Dockerfile.
- `k8s/deployment.yaml`: Deployment da aplicação.
- `k8s/service.yaml`: Service para acesso local.

