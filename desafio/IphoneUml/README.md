# iPhone Project - POO Desafio

## Descrição do Projeto

Este projeto foi desenvolvido como parte do desafio de POO na DIO, onde foi solicitado a modelagem e implementação das principais funcionalidades do iPhone lançado em 2007. As funcionalidades abordadas são:

- **Reprodutor Musical**: Implementa operações básicas como tocar, pausar e selecionar uma música.
- **Aparelho Telefônico**: Implementa operações como fazer uma ligação, atender e iniciar o correio de voz.
- **Navegador na Internet**: Implementa operações como exibir uma página, adicionar uma nova aba e atualizar a página.

Este projeto foi desenvolvido utilizando Java e os conceitos de Programação Orientada a Objetos (POO). Um diagrama UML foi criado para representar as classes e interfaces do sistema.

## Diagrama UML

O diagrama UML a seguir representa a estrutura das classes e interfaces do projeto:

```mermaid
classDiagram
    class ReprodutorMusical {
        +tocar()
        +pausar()
        +selecionarMusica(String musica)
    }
    class AparelhoTelefonico {
        +ligar(String numero)
        +atender()
        +iniciarCorreioVoz()
    }
    class NavegadorInternet {
        +exibirPagina(String url)
        +adicionarNovaAba()
        +atualizarPagina()
    }
    class iPhone {
    }
    iPhone ..|> ReprodutorMusical
    iPhone ..|> AparelhoTelefonico
    iPhone ..|> NavegadorInternet
