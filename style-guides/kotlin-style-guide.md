# Style-guide Kotlin


# Guia de Estilo Kotlin

# 1. Nomenclatura
- **Variáveis**: Use camelCase para variáveis e funções.
- **Classes e Objetos**: Use PascalCase.
- **Constantes**: Use SCREAMING_SNAKE_CASE.

## 2. Null Safety
- Prefira usar o operador de chamada segura (`?.`) e o operador elvis (`?:`).
- Evite o operador de asserção não-nula (`!!`) sempre que possível.

### 3. Imutabilidade
- Prefira usar `val` em vez de `var` para promover imutabilidade.

# Exemplo:
```kotlin
data class User(val id: Int, val name: String)

fun findUser(id: Int?): User? {
    return null // Retorna null se não encontrar o usuário
}

val user = findUser(123)
println(user?.name ?: "Usuário não encontrado")