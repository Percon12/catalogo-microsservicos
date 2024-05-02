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

# Resiliência e Escalabilidade

Este tópico abrange as práticas que garantem que os sistemas baseados em microsserviços possam lidar com falhas e alterações na carga de trabalho de forma eficaz, mantendo a alta disponibilidade e a performance sob diferentes condições.

***

## Isolamento de Falhas

Isolar falhas em uma arquitetura de microsserviços significa garantir que um problema em um serviço não afete os outros. Implementar padrões como Circuit Breaker e Bulkhead são estratégias eficazes para gerenciar e mitigar falhas.

#### Exemplo Prático:

Suponha um sistema de reserva de passagens aéreas:

* **Microsserviço de Reservas**: Responsável por processar reservas.
* **Microsserviço de Pagamentos**: Lida com transações financeiras.

Se o microsserviço de Pagamentos ficar indisponível, um circuit breaker pode ser ativado para evitar chamadas desnecessárias a esse serviço, utilizando um mecanismo de fallback, como emitir um voucher para pagamento posterior, garantindo que o serviço de Reservas permaneça operacional.

***

## Escalabilidade

A escalabilidade em microsserviços envolve a capacidade de um serviço aumentar ou diminuir seus recursos conforme necessário para lidar com variações na demanda.

#### Exemplo Prático:

Em um aplicativo de comércio eletrônico durante a Black Friday:

* **Microsserviço de Pedidos**: Experimenta um aumento significativo na demanda.
* **Microsserviço de Catálogo de Produtos**: Recebe mais consultas para informações de produtos.

Utilizando uma plataforma como Kubernetes, esses microsserviços podem ser automaticamente escalados horizontalmente, adicionando mais instâncias para lidar com o aumento da carga, garantindo que o sistema continue a responder eficientemente às solicitações dos usuários.
