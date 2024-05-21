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

# Arquitetura e Design

A estratégia de arquitetura e design influencia diretamente a eficácia e a flexibilidade dos microsserviços, permitindo que eles sejam bem integrados e mantenham a capacidade de evoluir ao longo do tempo.

***

## Utilização de Container

Containers são fundamentais para a arquitetura de microsserviços, proporcionando um ambiente isolado e consistente para cada serviço, o que facilita a portabilidade e a escalabilidade.

#### Exemplos Práticos:

Em um aplicativo de mídia social que inclui serviços para gerenciamento de usuários, postagens e comentários:

* **Docker**: Cada microsserviço é encapsulado em seu próprio container, garantindo que as dependências e o ambiente sejam uniformes em desenvolvimento, teste e produção.
* **Kubernetes**: Gerencia esses containers, automatizando o deployment, a escalabilidade e a gestão operacional.

***

## Padrão de Design de Microsserviços

Adotar padrões de design específicos pode resolver problemas comuns na arquitetura de microsserviços, melhorando a comunicação entre serviços e a gestão de dados.

#### Exemplo Prático:

Suponha um sistema de e-commerce com alta demanda e complexidade:

* **API Gateway**: Funciona como um ponto único de entrada para todas as requisições, roteando-as para os serviços apropriados e agregando as respostas.
* **Pattern BFF (Backend for Frontend)**: Implementado para otimizar a comunicação entre a interface do usuário e os microsserviços, oferecendo endpoints customizados que atendem especificamente às necessidades de diferentes clientes, como desktops e smartphones.
* **SAGA**: Gerencia transações que envolvem múltiplos microsserviços, assegurando a consistência dos dados em operações distribuídas através de eventos sequenciais que podem compensar ações anteriores em caso de falhas.



***

### Referências

**MICROSOFT. Architecting container and microservice-based applications.** Disponível em: [https://learn.microsoft.com/en-us/dotnet/architecture/microservices/architect-microservice-container-applications/](https://learn.microsoft.com/en-us/dotnet/architecture/microservices/architect-microservice-container-applications/). Acesso em: 21 mai. 2024.

**JFROG. The Role of Containers in Your Microservice Architecture.** Disponível em: [https://jfrog.com/devops-tools/article/role-of-containers-in-your-microservice-architecture/#:\~:text=Containers%20are%20a%20lightweight%20alternative,host%20operating%20system%20(OS).](https://jfrog.com/devops-tools/article/role-of-containers-in-your-microservice-architecture/). Acesso em: 21 mai. 2024.

**AWS. Let’s Architect! Architecting microservices with containers.** Disponível em: [https://aws.amazon.com/blogs/architecture/lets-architect-architecting-microservices-with-containers/](https://aws.amazon.com/blogs/architecture/lets-architect-architecting-microservices-with-containers/). Acesso em: 21 mai. 2024.

**IBM. Four Architecture Choices for Application Development in the Digital Age.** Disponível em: [https://www.ibm.com/blog/four-architecture-choices-for-application-development/](https://www.ibm.com/blog/four-architecture-choices-for-application-development/). Acesso em: 21 mai. 2024.

**MICROSOFT. Architecting container and microservice-based applications.** Disponível em: [https://learn.microsoft.com/en-us/dotnet/architecture/microservices/architect-microservice-container-applications/](https://learn.microsoft.com/en-us/dotnet/architecture/microservices/architect-microservice-container-applications/). Acesso em: 21 mai. 2024.

**MICROSOFT. Padrões de design de microsserviços.** Disponível em: [https://learn.microsoft.com/pt-br/azure/architecture/microservices/design/patterns](https://learn.microsoft.com/pt-br/azure/architecture/microservices/design/patterns). Acesso em: 21 mai. 2024.

**CODEFRESH. Top 10 Microservices Design Patterns and How to Choose.** Disponível em: [https://codefresh.io/learn/microservices/top-10-microservices-design-patterns-and-how-to-choose/](https://codefresh.io/learn/microservices/top-10-microservices-design-patterns-and-how-to-choose/). Acesso em: 21 mai. 2024.
