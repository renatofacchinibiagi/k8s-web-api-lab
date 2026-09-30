
## Relato do projeto

🚀 Laboratório Kubernetes Local | Docker Desktop + kind

Nos últimos dias, venho buscando desenvolver, fortalecer e aprofundar mais minhas habilidades em Kubernetes, containers e SRE, entendendo os conceitos e como cada componente funciona na prática.

Para isso, criei um laboratório utilizando o Kubernetes integrado ao Docker Desktop, executado com kind (Kubernetes IN Docker).

Para o workload, desenvolvi um frontend em HTML, CSS e JavaScript, containerizado com Nginx.

Durante o laboratório, pratiquei:

🐳 Criação de imagem Docker com Nginx;

☸️ Deployment com 3 réplicas;

🔄 Deployment, ReplicaSet e Pods;

🌐 Service LoadBalancer;

🏷️ Labels e Selectors;

❤️ Readiness e Liveness Probes;

⚙️ Requests e Limits de CPU e memória;

🔍 Troubleshooting com kubectl get, describe, logs, events e exec;

📈 Scaling e self-healing;

🌐 Acesso à aplicação por outros dispositivos da rede local.

O objetivo foi fortalecer minhas habilidades em Kubernetes na prática, acompanhando o comportamento dos Pods, exposição da aplicação, disponibilidade e recuperação.

🔎 Como evolução, pretendo adicionar uma API para gerar requisições e diferentes comportamentos, permitindo praticar observabilidade, acompanhando latência, erros, tempo de resposta, health checks, logs e métricas em cenários controlados.

☁️ Apesar de já ter realizado outros labs com Azure Kubernetes Service (AKS), também pretendo evoluir este projeto para um cenário de modernização para Cloud, levando o workload local para o AKS na Microsoft Azure e aplicando os conceitos de Kubernetes, observabilidade e SRE em ambiente Cloud.

Em breve compartilho essa evolução por aqui! 🚀

GitHub: github.com/renatofacchinibiagi/k8s-web-api-lab

#Kubernetes #Docker #Azure #AKS #SRE #DevOps #Observability #Containers #Modernization



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


## Registros do laboratório

![Modernização do laboratório](Moderniza%C3%A7%C3%A3o.png)
![Visão do laboratório](Lab%20explicado.png)
![Comandos de observabilidade](Comandos%20Observabilidade.png)
