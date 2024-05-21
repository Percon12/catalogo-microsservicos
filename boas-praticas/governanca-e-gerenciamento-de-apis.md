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

# Governança e Gerenciamento de APIs

O gerenciamento eficaz de APIs é crucial para garantir que os microsserviços possam se comunicar de forma segura, confiável e eficiente. Este tópico inclui práticas essenciais para a manutenção da integridade e governança das APIs.

***

## Gerenciamento de Versãoi e API

A gestão de versões é fundamental para garantir que mudanças nas APIs não causem disrupções nos serviços existentes e permitam uma transição suave para os consumidores de API.

#### Exemplo Prático:

Suponhamos que um microsserviço de autenticação introduza novas funcionalidades de segurança que alteram a API:

* **Versão Antiga (v1)**: Continua disponível temporariamente para dar aos consumidores tempo para adaptar-se.
* **Nova Versão (v2)**: Introduzida com novos endpoints ou alterações em endpoints existentes, documentados claramente para facilitar a transição.

***

## Documentação de API

Documentar APIs de forma clara e acessível é vital para facilitar a integração e o uso correto dos microsserviços por desenvolvedores internos e externos.

#### Exemplo Prático:

Para um microsserviço que gerencia informações de produtos em um e-commerce:

* Utiliza-se Swagger ou OpenAPI para criar uma documentação interativa:
  * **Endpoints**: Descrição detalhada de cada endpoint, incluindo métodos HTTP, parâmetros esperados e formatos de resposta.
  * **Exemplos de Código**: Fornecem exemplos práticos de como integrar e consumir a API.

***

### Referências

**POSTMAN. What is API versioning? Benefits, types & best practices.** Disponível em: [https://www.postman.com/api-platform/api-versioning/#:\~:text=API%20versioning%20is%20the%20process,tracking%20changes%20to%20an%20API.](https://www.postman.com/api-platform/api-versioning/). Acesso em: 21 mai. 2024.

**AKANA BY PERFORCE. API Versioning Best Practices | API Versioning Strategy.** Disponível em: [https://www.akana.com/blog/api-versioning](https://www.akana.com/blog/api-versioning). Acesso em: 21 mai. 2024.

**NORDIC APIS. Introduction to API Versioning Best Practices.** Disponível em: [https://nordicapis.com/introduction-to-api-versioning-best-practices/](https://nordicapis.com/introduction-to-api-versioning-best-practices/). Acesso em: 21 mai. 2024.

**LONTI. The importance of API versioning and best practices for microservices.** Disponível em: [https://www.lonti.com/blog/the-importance-of-api-versioning-and-best-practices-for-microservices](https://www.lonti.com/blog/the-importance-of-api-versioning-and-best-practices-for-microservices). Acesso em: 21 mai. 2024.\
\
**POSTMAN. API Documentation: How to Write, Examples & Best Practices.** Disponível em: [https://www.postman.com/api-platform/api-documentation/](https://www.postman.com/api-platform/api-documentation/). Acesso em: 21 mai. 2024.

**POSTMAN. What Is a REST API? Examples, Uses & Challenges.** Disponível em: [https://blog.postman.com/rest-api-examples/](https://blog.postman.com/rest-api-examples/). Acesso em: 21 mai. 2024.

**POSTMAN. API Versioning: How Postman Can Help.** Disponível em: [https://www.postman.com/product/api-versioning/](https://www.postman.com/product/api-versioning/). Acesso em: 21 mai. 2024.
