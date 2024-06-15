# DesafioControleFluxo

Este projeto Java é um desafio de programação desenvolvido para praticar conceitos de controle de fluxo em Java.

## Descrição do Desafio

O desafio consiste em criar um programa Java que:

1. Recebe dois números inteiros como entrada do usuário via terminal.
2. Conta e imprime os números inteiros em sequência a partir do primeiro número até o segundo número.
3. Lança uma exceção customizada (`ParametrosInvalidosException`) se o primeiro número fornecido for maior que o segundo número.

## Funcionalidades

- **Entrada de Dados:** Os números inteiros são inseridos pelo usuário através do terminal.
- **Saída Esperada:** O programa imprime cada número em sequência no formato "Imprimindo o número X".
- **Exceção Customizada:** Se o primeiro número for maior que o segundo, o programa lança uma exceção com a mensagem "O segundo parâmetro deve ser maior que o primeiro".

## Estrutura do Projeto

O projeto está estruturado da seguinte forma:

- **`Contador.java`**: Contém a lógica principal do programa, incluindo a validação dos parâmetros e a contagem dos números.
- **`ParametrosInvalidosException.java`**: Classe de exceção customizada para lidar com parâmetros inválidos.
- **`README.md`**: Este arquivo, que fornece informações sobre o projeto e sua utilização.