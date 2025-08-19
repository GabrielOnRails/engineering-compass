# Runbook para Serviço de API (ex: User Service)

## 1. Diagnóstico de Problemas
-   **Serviço Inativo**:
    -   Verificar logs no Kibana/Grafana buscando por erros 500 ou timeouts.
    -   Checar o status do serviço no Kubernetes (`kubectl get pods -n <namespace>`).
-   **Latência Alta**:
    -   Monitorar métricas de CPU e memória no Prometheus.
    -   Analisar os `endpoints` mais lentos no tracing (ex: Jaeger).

## 2. Ações de Recuperação
-   **Reiniciar o Serviço**:
    `kubectl rollout restart deployment user-service-deployment`
-   **Reverter a Última Implantação**:
    `kubectl rollout undo deployment user-service-deployment`