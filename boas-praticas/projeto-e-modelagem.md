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

# Projeto e Modelagem

O processo de projeto e modelagem é fundamental para criar uma arquitetura de microsserviços bem-sucedida. Este tópico abrange as práticas essenciais que orientam a estrutura e o comportamento dos microsserviços dentro do ecossistema mais amplo.

***

## Design de Domínio Específico

O Design de Domínio Específico, ou Domain-Driven Design (DDD), é uma abordagem de desenvolvimento de software que foca na complexidade dos problemas de negócios e cria uma linguagem comum entre desenvolvedores e stakeholders. A ideia é modelar cada microsserviço em torno de um domínio de negócio claramente definido.

#### Exemplo Prático:

Suponha que estamos desenvolvendo um aplicativo para uma rede de cinemas. Podemos modelar microsserviços específicos para:

* **Programação de Filmes**: Gerencia informações sobre filmes e horários de exibição.
* **Vendas de Bilhetes**: Trata das transações de compra e reserva de assentos.
* **Gestão de Clientes**: Mantém registros de clientes e suas interações com o cinema.

Cada um desses microsserviços opera de forma independente, com seu próprio banco de dados e lógica de negócios, focando exclusivamente em seu domínio.

***

## Decomposição de Dados

A decomposição de dados é uma prática que envolve separar os bancos de dados por microsserviço, de forma que cada um gerencie seus próprios dados. Isso evita dependências e acoplamentos entre serviços, promovendo a autonomia e a facilidade de manutenção.

#### Exemplo Prático:

Continuando o exemplo da rede de cinemas:

* O **microsserviço de Programação de Filmes** poderia usar um banco de dados NoSQL para armazenar dados semi-estruturados sobre filmes e horários, dada a flexibilidade necessária para mudanças frequentes na programação.
* O **microsserviço de Vendas de Bilhetes** poderia utilizar um sistema de banco de dados relacional, como PostgreSQL, para gerenciar transações financeiras e reservas de assentos, onde a integridade dos dados é crítica.

***

### Referências

* MICROSOFT. **Best Practice - An Introduction To Domain-Driven Design**. Disponível em: [https://learn.microsoft.com/en-us/dotnet/architecture/microservices/microservice-ddd-cqrs-patterns/](https://learn.microsoft.com/en-us/dotnet/architecture/microservices/microservice-ddd-cqrs-patterns/). Acesso em: 16 maio 2024.
* MOMENTS LOG. **The Role of Domain-Driven Design in Software Architecture**. Disponível em: https://www.momentslog.com/architecture/domain-driven-design-role-in-software-architecture. Acesso em: 16 maio 2024.
* INFOQ. **Domain Driven Design and Development In Practice**. Disponível em: https://www.infoq.com/articles/domain-driven-design-in-practice/. Acesso em: 16 maio 2024.
*   **Microservices.io**

    RICHARDSON, Chris. **Pattern: Database per service**. Disponível em: [https://microservices.io/patterns/data/database-per-service.html](https://microservices.io/patterns/data/database-per-service.html). Acesso em: 16 maio 2024.
* **Microsoft Learn**\
  MICROSOFT. **Data considerations for microservices - Azure Architecture Center**. Disponível em: [https://learn.microsoft.com/en-us/azure/architecture/microservices/data-considerations](https://learn.microsoft.com/en-us/azure/architecture/microservices/data-considerations). Acesso em: 16 maio 2024.
