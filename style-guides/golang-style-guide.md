# Style-guide GoLang

## 1. Nomenclatura
- **Variáveis**: Use nomes curtos para variáveis locais (ex: `i` para loop, `c` para contador). Use nomes mais longos e descritivos para variáveis globais e exportadas.
- **Funções e Métodos**: Inicie com letra maiúscula para exportar a função. Use verbos no nome de funções que realizam uma ação (ex: `GetUserData`), e substantivos para aquelas que retornam dados sem efeitos colaterais (ex: `User`).

## 2. Tratamento de Erros
- Retorne erros explicitamente.
- Use o pacote `errors` para criar novos erros e `fmt.Errorf` para adicionar contexto.
- **Exemplo**:
  ```go
  if err != nil {
      return fmt.Errorf("falha ao processar a requisição: %w", err)
  }