# Style-guide Python

```markdown
# Guia de Estilo Python

# 1. PEP 8
- Siga as diretrizes do **PEP 8**, o guia de estilo oficial do Python.
- Use um linter como `flake8` para garantir a conformidade.

## 2. Nomenclatura
- **Variáveis e Funções**: Use `snake_case`.
- **Classes**: Use `PascalCase`.
- **Constantes**: Use `SCREAMING_SNAKE_CASE`.

### 3. Tipagem
- Use type hints para aumentar a legibilidade e a segurança do código.
- **Exemplo**:
  ```python
  def calculate_tax(amount: float) -> float:
      return amount * 0.15