# Style-guide Typescript

```markdown
# Guia de Estilo TypeScript

# 1. Tipagem
- Use tipagem explícita para funções e variáveis quando isso aumentar a clareza. Prefira inferência de tipo quando o tipo for óbvio.
- **Exemplo**:
  ```typescript
  // Preferível
  const isValid: boolean = checkValidity(data);
  // Aceitável, pois é óbvio
  const name = "João";