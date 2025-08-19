# Design de Plataforma de Streaming de Dados em Tempo Real

## Contexto
Precisamos processar grandes volumes de dados de eventos (ex: cliques de usuários, logs de transações) em tempo real para gerar insights para o time de marketing e de produto.

## Decisão
Construir uma plataforma de streaming de dados utilizando **Apache Kafka** para a ingestão e **Apache Flink** para o processamento. O Kafka servirá como a espinha dorsal para os eventos, enquanto o Flink processará os dados para detecção de anomalias e agregação de métricas em tempo real.

## Consequências
-   **Positivas**:
    -   Insights em tempo real, permitindo ações imediatas.
    -   Arquitetura escalável para lidar com picos de eventos.
-   **Negativas**:
    -   A curva de aprendizado para Kafka e Flink é alta.
    -   Exige uma infraestrutura dedicada e um time de SRE.