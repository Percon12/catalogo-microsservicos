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

# Monitoramento e Segurança

Este tópico aborda práticas essenciais para garantir que os microsserviços não só operem de maneira confiável e eficiente, mas também mantenham a segurança dos dados e das operações em todas as interações e transmissões.

***

## Monitoramento e Logging

Monitorar e registrar as atividades dos microsserviços é crucial para entender o comportamento do sistema, identificar problemas rapidamente e tomar decisões baseadas em dados concretos.

**Exemplo Prático:**

Em um sistema de gestão de saúde onde a confiabilidade é crítica:

* **Microsserviço de Agendamentos**: Registra cada solicitação de agendamento de consultas.
* **Microsserviço de Prontuários**: Monitora o acesso e as alterações nos registros dos pacientes.

Utilizando ferramentas como Prometheus para monitoramento em tempo real e ELK Stack (Elasticsearch, Logstash, Kibana) para agregação e visualização de logs, os administradores podem obter insights sobre o desempenho e qualquer comportamento anômalo nos serviços.

***

## Segurança

Implementar medidas robustas de segurança é fundamental para proteger as APIs e as comunicações entre os microsserviços contra acessos não autorizados e ataques cibernéticos.

#### Exemplo Prático:

Numa aplicação bancária onde a segurança é uma prioridade máxima:

* **Microsserviço de Transações**: Utiliza TLS para criptografar a comunicação de dados sensíveis.
* **Microsserviço de Autenticação**: Implementa OAuth para gerenciar autorizações e utiliza JWT (JSON Web Tokens) para assegurar as sessões de usuários.

Essas práticas são projetadas para garantir que as informações sejam transmitidas de forma segura e que o acesso aos microsserviços seja controlado e monitorado.

***

### Referências

1. SNIEDERM, R. **10 Rules to Microservice Logging**. Medium, 2023. Disponível em: [https://medium.com/@sniederm/10-rules-to-microservice-logging-4d24f6dd7abb](https://medium.com/@sniederm/10-rules-to-microservice-logging-4d24f6dd7abb). Acesso em: 16 maio 2024.
2. STACKIFY. **Monitoring Microservices: A 5-Step Guide**. Disponível em: [https://stackify.com/monitoring-microservices-a-5-step-guide/](https://stackify.com/monitoring-microservices-a-5-step-guide/). Acesso em: 16 maio 2024.
3. ATLASSIAN. **Microservices Security**. Disponível em: [https://www.atlassian.com/microservices/cloud-computing/microservices-security](https://www.atlassian.com/microservices/cloud-computing/microservices-security). Acesso em: 16 maio 2024.
4. SQUADCAST. **Microservices Security Tutorial and Best Practices**. LinkedIn, 2023. Disponível em: [https://www.linkedin.com/pulse/microservices-security-tutorial-best-practices-squadcast](https://www.linkedin.com/pulse/microservices-security-tutorial-best-practices-squadcast). Acesso em: 16 maio 2024.
5. WIZ. **Microservices Security Best Practices**. Disponível em: [https://www.wiz.io/academy/microservices-security-best-practices](https://www.wiz.io/academy/microservices-security-best-practices). Acesso em: 16 maio 2024.
