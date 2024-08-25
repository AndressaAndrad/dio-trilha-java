# Java List Interface

## Introdução

A **interface List** em Java faz parte da hierarquia de coleções do Java Collection Framework. Ela representa uma coleção ordenada que permite a inclusão de elementos duplicados, sendo uma das coleções mais utilizadas no desenvolvimento de software em Java.

### Características Principais:
- **Ordenação**: Os elementos em uma `List` mantêm uma ordem específica (ordem de inserção).
- **Elementos Duplicados**: Permite a inclusão de elementos duplicados.
- **Acesso por Índice**: Permite acessar, adicionar, remover e modificar elementos com base em seu índice.

## Hierarquia da Interface List

A `List` herda da interface `Collection`, que por sua vez herda da interface `Iterable`. Abaixo está uma hierarquia simplificada das coleções:


## Implementações Comuns

### 1. ArrayList
- **Descrição**: Implementa a interface `List` utilizando um array redimensionável.
- **Vantagem**: Acesso rápido aos elementos via índice.
- **Desvantagem**: Inserções e remoções no meio da lista são mais lentas, pois requerem a realocação dos elementos.

### 2. LinkedList
- **Descrição**: Implementa a interface `List` utilizando uma lista duplamente encadeada.
- **Vantagem**: Inserção e remoção eficientes no início e no final da lista.
- **Desvantagem**: Acesso aos elementos por índice é mais lento em comparação com o `ArrayList`.

### 3. Vector
- **Descrição**: Implementa a interface `List` de forma semelhante ao `ArrayList`, mas é sincronizado (thread-safe).
- **Vantagem**: Manipulação segura em ambientes com múltiplas threads.
- **Desvantagem**: Desempenho inferior ao `ArrayList` devido à sincronização.

## Manipulação de Listas

A classe `Collections` oferece diversos algoritmos úteis para manipulação de listas, como:
- **Ordenação (`sort`)**
- **Embaralhamento (`shuffle`)**
- **Reversão (`reverse`)**
- **Busca binária (`binarySearch`)**

## Exercícios Práticos

### 1. Operações Básicas com List
#### a) Lista de Tarefas
Crie uma classe chamada `ListaTarefas` que possui uma lista de tarefas. Cada tarefa é representada por uma classe `Tarefa` com um atributo `descrição`. Implemente os seguintes métodos:
- `adicionarTarefa(String descricao)`: Adiciona uma nova tarefa à lista.
- `removerTarefa(String descricao)`: Remove uma tarefa da lista com base em sua descrição.
- `obterNumeroTotalTarefas()`: Retorna o número total de tarefas.
- `obterDescricoesTarefas()`: Retorna uma lista com as descrições das tarefas.

#### b) Carrinho de Compras
Crie uma classe `CarrinhoDeCompras` que representa um carrinho de compras online, implementado como uma lista de itens. Cada item é representado por uma classe `Item` com atributos `nome`, `preço` e `quantidade`. Implemente os seguintes métodos:
- `adicionarItem(String nome, double preco, int quantidade)`: Adiciona um item ao carrinho.
- `removerItem(String nome)`: Remove um item do carrinho com base no nome.
- `calcularValorTotal()`: Calcula e retorna o valor total do carrinho.
- `exibirItens()`: Exibe os itens presentes no carrinho.

### 2. Pesquisa em List
#### a) Catálogo de Livros
Crie uma classe `CatalogoLivros` com uma lista de livros (`Livro`), onde cada livro tem atributos como `título`, `autor` e `ano de publicação`. Implemente os seguintes métodos:
- `adicionarLivro(String titulo, String autor, int anoPublicacao)`: Adiciona um livro ao catálogo.
- `pesquisarPorAutor(String autor)`: Pesquisa livros por autor.
- `pesquisarPorIntervaloAnos(int anoInicial, int anoFinal)`: Pesquisa livros publicados em um intervalo de anos.
- `pesquisarPorTitulo(String titulo)`: Pesquisa livros por título.

#### b) Soma de Números
Crie uma classe `SomaNumeros` que contém uma lista de números inteiros. Implemente os seguintes métodos:
- `adicionarNumero(int numero)`: Adiciona um número à lista.
- `calcularSoma()`: Calcula a soma de todos os números na lista.
- `encontrarMaiorNumero()`: Encontra e retorna o maior número.
- `encontrarMenorNumero()`: Encontra e retorna o menor número.
- `exibirNumeros()`: Retorna uma lista contendo todos os números.

### 3. Ordenação em List
#### a) Ordenação de Pessoas
Crie uma classe `OrdenacaoPessoas` que possui uma lista de objetos `Pessoa` com atributos `nome`, `idade` e `altura`. Implemente os seguintes métodos:
- `adicionarPessoa(String nome, int idade, double altura)`: Adiciona uma pessoa à lista.
- `ordenarPorIdade()`: Ordena as pessoas por idade.
- `ordenarPorAltura()`: Ordena as pessoas por altura usando um `Comparator`.

#### b) Ordenação de Números
Crie uma classe `OrdenacaoNumeros` que possui uma lista de números inteiros. Implemente os seguintes métodos:
- `adicionarNumero(int numero)`: Adiciona um número à lista.
- `ordenarAscendente()`: Ordena os números em ordem ascendente.
- `ordenarDescendente()`: Ordena os números em ordem descendente.

## Referências
[1] "Collections in Java Tutorial." DigitalOcean Community. Disponível em: https://www.digitalocean.com/community/tutorials/collections-in-java-tutorial.

[2] "Java™ Platform, Standard Edition 17 API Specification - Class List." Oracle. Disponível em: https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html.
