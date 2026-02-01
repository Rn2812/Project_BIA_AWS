# Project_BIA_AWS
Este repositório contém o desenvolvimento e a migração da aplicação BIA para a nuvem AWS, realizado durante a Imersão AWS &amp; IA. O projeto demonstra a evolução de uma arquitetura tradicional para uma infraestrutura moderna, containerizada e escalável, utilizando agentes de IA para otimizar o deploy e a gestão.


🛠️ Tecnologias Utilizadas
Cloud: Amazon Web Services (AWS)

Serviços: EC2 (Instâncias para ambiente de dev), ECR (Registro de imagens), ECS (Orquestração de containers), CloudShell.

Containerização: Docker

Infraestrutura como Código & IA: Uso de MCP Server (Model Context Protocol) e agentes de IA para automação de tarefas.

Versionamento & CI/CD: Git e GitHub.

🧠 Aprendizados e Etapas do Desafio
1. Preparação do Ambiente e Docker
Configuração de ambiente de trabalho isolado para evitar conflitos locais.

Criação de Dockerfiles otimizados para a aplicação BIA.

Gestão de imagens no Amazon ECR.

2. Infraestrutura na AWS
Configuração de instâncias EC2 na região us-east-1 (Norte da Virgínia).

Entendimento de redes (VPC) e grupos de segurança para acesso à aplicação via porta 3001.

3. Modernização com ECS e Fargate
Transição da arquitetura de uma única máquina para um modelo de clusters e serviços.

Configuração de Task Definitions (vCPU e Memória) para rodar containers de forma eficiente.

Uso de Application Load Balancers (ALB) para distribuição de tráfego.



Para rodar localmente: docker-compose up --build

Para deploy na AWS: Siga os passos de configuração do ECS detalhados na pasta /infra.
