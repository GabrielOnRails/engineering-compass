# Runbook para Migração de Banco de Dados

# 1. Pré-Requisitos
-   Backups recentes do banco de dados.
-   Confirmação de que o serviço está em modo de manutenção ou inativo.

## 2. Procedimento
1.  **Parar o Serviço**: `kubectl scale deployment <app-deployment> --replicas=0`
2.  **Executar Migração**: `kubectl exec -it <pod-name> -- python manage.py migrate` (ou o comando da sua ferramenta de migração)
3.  **Verificar Logs**: Confirme se a migração foi bem-sucedida.
4.  **Iniciar o Serviço**: `kubectl scale deployment <app-deployment> --replicas=<original-replicas>`

### 3. Rollback
-   Em caso de falha, use o backup para restaurar o banco de dados.