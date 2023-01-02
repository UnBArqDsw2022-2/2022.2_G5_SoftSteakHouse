# GoF(s)

## Introdução

Padrões de projeto são princípios e soluções usados durante a criação de um software, codificados em um formato estruturado, descrevendo o problema e a respectiva solução adotada. Com isso, os padrões GoF (Gang of Four) buscam uma solução consolidada para um problema recorrente no desenvolvimento e manutenção de software orientado a objetos.

A referência mais relevante para é a 'Design Patterns: Elements of Reusable Object-Oriented Software', Erich Gamma, Richard Helm, Ralph Johnson e John Vlissides, de 1995. Eles descrevem seus padrões de projeto em diversos elementos:

- **Nome e classificação do padrão:** O nome deve passar a essência do padrão sucintamente.
- **Intenção:** Pequena explicação que responde às perguntas: o que o padrão faz? Qual sua intenção? Qual problema de design específico resolve?
- **Também conhecido como:** Outros nomes para o padrão, caso exista.
- **Motivação:** Um cenário que ilustra o problema e como as classes e objetos estruturados no padrão resolvem o problema.
- **Aplicabilidade:** Quais são as situações que os padrões podem ser aplicados?
- **Estrutura:** Representação gráfica das classes no padrão.
- **Participantes:** Classes e objetos que participam do padrão e suas responsabilidades.
- **Colaborações:** Como os participantes colaboram com suas responsabilidades.
- **Consequências:** Como o padrão suporta seus objetivos? Quais trade-offs e resultados do uso do padrão?
- **Implementação:** Quais dicas ou técnicas devem ser conhecidas quando implementando o padrão? Existem problemas ligados à linguagem?
- **Exemplo de Código:** Fragmentos de código que ilustram como se implementam o padrão.
- **Usos conhecidos:** Exemplos do padrão em sistemas reais.
- **Padrões relacionados:** Quais padrões são relacionados com o descrito?

Os padrões de projeto GoFs podem ser divididos em três tipos: **Criacionais**, **Estruturais** e **Comportamentais**.

## GoFs Criacionais

Em um projeto orientado a objetos, a criação de objetos tem dois problemas principais que se destacam:

- Definir qual classe concreta deve ser utilizada para criar o objeto;
- Definir como os objetos devem ser criados e como eles se relacionam com outros objetos do sistema.

Conforme o princípio do encapsulamento, essa complexidade deve ser, preferencialmente, isolada. Assim, pode-se citar alguns padrões de projeto GoFs Criacionais e seus objetivos para resolver esses problemas (os usados no projeto são melhor explorados em seus artefatos únicos):

- **Factory Method**: permitir delegar a instanciação às subclasses.
- **Abstract Factory**: permitir a criação de famílias de objetos relacionados ou dependentes por meio de uma única interface e sem que a classe concreta seja especificada.
- **Builder**: permitir a construção de objetos complexos passo a passo.
- **Prototype**: permitir a cópia de objetos existentes sem deixar o código dependente de suas classes.
- **Singleton**: permitir a garantia que uma classe tenha apenas uma instância, enquanto provê um ponto de acesso global para essa instância.

## GoFs Estruturais

A partir de interações, os objetos podem gerar fortes dependências entre si, aumentando a complexidade de eventuais alterações no funcionamento do sistema (e, consequentemente, o custo também aumenta).

Com isso, os padrões de projeto estruturais buscam diminuir o acoplamento entre os objetos de um sistema baseado em OO, trabalhando, principalmente, no nível de classes. Assim, pode-se citar alguns padrões de projeto GoFs Estruturais e seus objetivos para resolver esses problemas (os usados no projeto são melhor explorados em seus artefatos únicos):

- **Adapter**: permitir que um objeto seja substituído por outro que, apesar de realizar a mesma tarefa, possui uma interface diferente.
- **Bridge**: permitir a divisão de uma classe grande ou um conjunto de classes ligadas em duas hierarquias separadas que podem ser desenvolvidas independentemente umas das outras.
- **Composite**: agrupar objetos que fazem parte de uma relação parte-todo para tratá-los sem distinção.
- **Decorator**: permitir a adição de novos comportamentos a objetos colocando eles em um wrapper de objetos que contém os comportamentos.
- **Facade**: fornecer uma interface simplificada para uma biblioteca ou framework.
- **Proxy**: permitir o fornecimento de um substituto para outro objeto (controle do acesso ao objeto original).

## GoFs Comportamentais

Os padrões comportamentais são voltados para alterações no nível de comportamento dos objetos, auxiliando, por exemplo, usar vários algoritmos diferentes, cada um apropriado para um determinado contexto.

Nesse caso, permitem usar mecanismos/recursos para facilitar tanto a incorporação de novos algoritmos para novos contextos quanto a seleção de qual algoritmo usar dado um contexto. Assim, pode-se citar alguns padrões de projeto GoFs Comportamentais e seus objetivos para resolver esses problemas (os usados no projeto são melhor explorados em seus artefatos únicos): 

- **Command**: permitir a parametrização de métodos com diferentes pedidos, uma vez que transforma pedidos em objetos independente. 
- **Strategy**: permitir de forma simples a variação dos algoritmos utilizados na resolução de um determinado problema.
- **Template Method**: Definir a ordem na qual determinados passos devem ser realizados na resolução de um problema e permitir que esses passos possam ser realizados de formas diferentes conforme a situação.
- **Chain of Responsibility**: permitir passar pedidos por uma corrente de handlers (processa ou passa para o próximo handler).
- **Iterator**: permitir percorrer elementos de uma coleção sem expor as representações estruturais dele.
- **Mediator**: permitir a redução das dependências caóticas entre objetos (restringe comunicações diretas entre objetos e os força a colaborar apenas através do mediador).
- **Observer**: permitir a definição de um mecanismo de assinatura para notificar múltiplos objetos sobre eventos que aconteçam sobre um objeto observado.
- **State**: permitir que um objeto altere seu comportamento quando seu estado interno muda.
- **Visitor**: permitir a separação de algoritmos dos objetos que eles operam.

## Histórico de Versões

|    Data    | Versão |            Descrição           |       Autor     |    Revisor    |
|  --------  |  ----  |            ----------          | --------------- |    -------    |
| 01/01/2023 |  1.0.0 |  Criação do artefato de GoFs | [Victor Leão](https://github.com/victorleaoo) | [Caio César](https://github.com/oCaioOliveira) |

## Referências
SERRANO, Milene. GoFs, 2022. Material apresentado na Disciplina de Arquitetura e Desenho de Software do curso de engenharia de software da UnB, FGA. Acesso em: 01 jan. 2023.

Erich Gamma, Richard Helm, Ralph Johnson, John Vlissides. Design Patterns: Elements of Reusable Object-Oriented Software. Addison-Wesley, 1995.

REFACTORING GURU. Padrões de projeto criacionais. Disponível em: https://refactoring.guru/pt-br/design-patterns/creational-patterns. Acesso em: 01 jan. 2023.

REFACTORING GURU. Padrões de projeto estruturais. Disponível em: https://refactoring.guru/pt-br/design-patterns/structural-patterns. Acesso em: 01 jan. 2023.

REFACTORING GURU. Padrões de projeto comportamentais. Disponível em: https://refactoring.guru/pt-br/design-patterns/behavioral-patterns. Acesso em: 01 jan. 2023.
