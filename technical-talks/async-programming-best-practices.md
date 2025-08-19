# Programação Assíncrona: Melhores Práticas

## O Problema
Em sistemas que lidam com I/O (requisições de rede, acesso a banco de dados), a abordagem síncrona pode levar a gargalos e baixa performance.

## A Solução: Assincronismo
A programação assíncrona permite que o programa realize outras tarefas enquanto espera por uma operação de I/O.

### Exemplos em GoLang (Goroutines)
Go usa `goroutines` e `channels` para concorrência.
```go
package main

import (
	"fmt"
	"time"
)

func fetchData() {
	time.Sleep(2 * time.Second) // Simula uma requisição lenta
	fmt.Println("Dados foram carregados.")
}

func main() {
	go fetchData() // Inicia a goroutine
	fmt.Println("Continuando o processamento sem esperar...")
	time.Sleep(3 * time.Second)
}

