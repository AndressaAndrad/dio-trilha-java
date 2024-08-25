# Java Collection Framework

## Introdução

O **Java Collection Framework** é um conjunto de interfaces e classes que fornecem uma arquitetura padrão para armazenar e manipular grupos de dados como objetos. Ele facilita o desenvolvimento de programas, permitindo que você trabalhe com coleções de forma eficiente e eficaz.

## O que é uma Coleção?

Uma **coleção** é uma estrutura de dados que agrupa muitos elementos em uma única unidade. Estes elementos precisam ser objetos, e as coleções podem ser homogêneas (todos os elementos do mesmo tipo) ou heterogêneas (elementos de tipos diferentes), embora normalmente se utilizem coleções homogêneas.

## Principais Interfaces

O núcleo principal do framework de coleções é composto por diversas interfaces, que permitem manipular coleções independentemente dos detalhes de implementação. As principais interfaces são:

- **Collection**: A interface raiz de todas as coleções.
- **List**: Representa uma coleção ordenada, que pode conter elementos duplicados.
- **Set**: Representa uma coleção que não permite elementos duplicados.
- **Queue**: Representa uma coleção destinada ao processamento de elementos em uma ordem específica (geralmente FIFO - First In, First Out).
- **Map**: Representa uma coleção que mapeia chaves para valores, sem chaves duplicadas.

## Principais Implementações

Existem várias implementações das interfaces acima, cada uma com características específicas que as tornam mais adequadas para diferentes situações. Algumas das implementações mais comuns incluem:

- **ArrayList** (implementa `List`): Armazena os elementos em um array dinâmico.
- **LinkedList** (implementa `List` e `Queue`): Armazena os elementos em uma lista duplamente encadeada.
- **HashSet** (implementa `Set`): Armazena os elementos em uma tabela de hash, sem garantir a ordem.
- **TreeSet** (implementa `Set`): Armazena os elementos em uma árvore binária ordenada.
- **PriorityQueue** (implementa `Queue`): Armazena os elementos de acordo com a sua prioridade.
- **HashMap** (implementa `Map`): Armazena os pares chave-valor em uma tabela de hash.
- **TreeMap** (implementa `Map`): Armazena os pares chave-valor em uma árvore binária ordenada.

## Como Usar

Para utilizar o Java Collection Framework, você deve importar os pacotes `java.util.*`. Por exemplo:

```java
import java.util.ArrayList;
import java.util.HashMap;
import java.util.Set;
import java.util.Map;
