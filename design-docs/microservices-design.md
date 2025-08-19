# Design de Arquitetura: Migrando para Microsserviços

## Contexto
Atualmente, nosso e-commerce opera como um monolito, o que está causando gargalos de escalabilidade durante picos de tráfego, como na Black Friday. O tempo de build e deploy é excessivo, e falhas em uma parte do sistema afetam todo o serviço. Precisamos de uma arquitetura que permita escalar componentes individualmente e facilite a inovação.

## Decisão
Migrar a arquitetura monolítica para um sistema de microsserviços. Os componentes serão decompostos em serviços menores, como `payments-service`, `catalog-service` e `user-service`. A comunicação entre os serviços será via RESTful API e mensageria assíncrona (usando RabbitMQ).

**Diagrama da Nova Arquitetura:**
(Aqui você adicionaria um diagrama de alto nível)

## Consequências
-   **Positivas**:
    -   Maior escalabilidade e resiliência.
    -   Permite times independentes.
    -   Tecnologias podem ser escolhidas por serviço (poliglotismo).
-   **Negativas**:
    -   Maior complexidade de operação e monitoramento.
    -   Aumento da latência em algumas operações.
    -   Exige uma forte cultura de DevOps.