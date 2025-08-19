# Estratégia de Versionamento de API

## Contexto
Nossas APIs estão em constante evolução, e a falta de uma estratégia de versionamento clara causa problemas de compatibilidade com clientes antigos. Precisamos de uma abordagem que seja fácil de manter e que garanta a estabilidade.

## Decisão
Adotar o **versionamento de URI** (`/api/v1/resource`). Esta abordagem é simples, transparente para o cliente e permite que diferentes versões da API coexistam sem conflitos de headers ou media types.

## Consequências
-   **Positivas**:
    -   Fácil de entender e implementar.
    -   Compatibilidade com todos os clientes HTTP.
-   **Negativas**:
    -   Pode tornar as URIs mais longas.
    -   Exige que o cliente altere a URI ao migrar de versão.