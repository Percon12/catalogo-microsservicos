---
layout:
  title:
    visible: true
  description:
    visible: false
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# Comunicação e Integração

Este tópico aborda como os microsserviços interagem entre si e com outros sistemas, garantindo que a comunicação seja eficaz, segura e escalável. A comunicação e integração eficientes são vitais para o sucesso de uma arquitetura baseada em microsserviços.

***

## Comunicação Baseada em API

APIs são a espinha dorsal da comunicação em uma arquitetura de microsserviços. Elas permitem que serviços distintos interajam de maneira desacoplada e flexível, usando padrões de comunicação como REST, GraphQL ou gRPC.

#### Exemplo Prático:

Imagine um aplicativo de entrega de alimentos onde diferentes microsserviços precisam interagir:

* **Microsserviço de Pedidos**: Recebe pedidos dos clientes e envia solicitações ao microsserviço de Cozinha.
* **Microsserviço de Cozinha**: Gerencia a preparação dos alimentos e notifica o microsserviço de Entrega quando o pedido está pronto.

A comunicação entre esses serviços é feita por meio de APIs RESTful, onde cada serviço expõe endpoints específicos para receber requisições ou enviar respostas. Para facilitar e gerenciar essa comunicação, um API Gateway é frequentemente utilizado. O API Gateway atua como um ponto de entrada centralizado para todas as requisições, roteando-as para os microsserviços apropriados, aplicando políticas de segurança, realizando a agregação de dados e oferecendo outras funcionalidades essenciais para uma comunicação eficiente e segura.

#### POC:

Para demonstrar na prática essa boa prática, desenvolvemos uma Prova de Conceito (PoC) na qual implementamos um microsserviço específico onde as comunicações e chamadas de API são feitas por meio de um Gateway.

Para acessar os detalhes, clique no link: [https://tcc-organization.gitbook.io/trabalho-de-conclusao-de-curso/pocs/poc-2](https://tcc-organization.gitbook.io/trabalho-de-conclusao-de-curso/pocs/poc-2)

***

## Automação de Deploy (CI/CD)

A automação de deploy, incluindo Integração Contínua (CI) e Entrega Contínua (CD), é crucial para manter a agilidade e a qualidade em ambientes de microsserviços. Essas práticas permitem a implementação rápida e segura de novas funcionalidades e correções.

#### Exemplo Prático:

Utilizando ferramentas como Jenkins, GitLab CI ou GitHub Actions, o processo pode ser configurado para:

* **Build automático**: Cada push no repositório gera uma nova build, executando testes automatizados.
* **Deploy automatizado**: Se a build for bem-sucedida, o deploy é feito automaticamente em ambientes de teste ou produção, dependendo da branch e das políticas de deploy.

***

## Configuração Externa

Gerenciar as configurações externamente permite que os microsserviços sejam executados em diferentes ambientes sem necessidade de alteração no código. Isso facilita operações como testes, deploys e escalabilidade.

#### Exemplo Prático:

Utilizando o Spring Cloud Config, um serviço de configuração centralizada, é possível:

* Armazenar configurações em um repositório central (como um repositório Git).
* Permitir que os microsserviços busquem sua configuração específica do ambiente em que estão sendo executados (desenvolvimento, teste, produção).

***

### Referências

1. NGINX. **Building Microservices: Inter-Process Communication**. Disponível em: [https://www.nginx.com/blog/building-microservices-inter-process-communication/](https://www.nginx.com/blog/building-microservices-inter-process-communication/). Acesso em: 16 maio 2024.
2. MICROSOFT. **Communication in a microservice architecture**. Disponível em: [https://learn.microsoft.com/en-us/dotnet/architecture/microservices/communication-in-microservice-architecture](https://learn.microsoft.com/en-us/dotnet/architecture/microservices/communication-in-microservice-architecture). Acesso em: 16 maio 2024.
3. AMAZON WEB SERVICES. **Continuous Integration and Continuous Delivery (CI/CD)**. Disponível em: [https://aws.amazon.com/devops/continuous-integration/](https://aws.amazon.com/devops/continuous-integration/). Acesso em: 16 maio 2024.
4. GOOGLE CLOUD. **Continuous Integration**. Disponível em: [https://cloud.google.com/solutions/continuous-integration?hl=pt-br](https://cloud.google.com/solutions/continuous-integration?hl=pt-br). Acesso em: 16 maio 2024.
5. **GOOGLE CLOUD. Continuous Delivery Solutions.** Disponível em: [https://cloud.google.com/solutions/continuous-delivery?hl=pt-br](https://cloud.google.com/solutions/continuous-delivery?hl=pt-br). Acesso em: 21 mai. 2024.
6. RED HAT. **CI/CD for Microservices**. Disponível em: [https://www.redhat.com/en/technologies/cloud-computing/openshift/ci-cd](https://www.redhat.com/en/technologies/cloud-computing/openshift/ci-cd). Acesso em: 16 maio 2024.
7. SPRING. **Externalized Configuration**. Disponível em: [https://docs.spring.io/spring-boot/docs/current/reference/html/spring-boot-features.html#boot-features-external-config](https://docs.spring.io/spring-boot/docs/current/reference/html/spring-boot-features.html#boot-features-external-config). Acesso em: 16 maio 2024.

