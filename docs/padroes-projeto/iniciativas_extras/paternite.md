# Paternite

## Introdução

A palavra "Pattern" presente na obra que inaugurou boa parte dos padrões discutidos possui dois sinônimos em inglês, com uma tradução elucidativa para o português - "standard" e "default".
"Standard" é uma padrão oficial, ou uma definição definitiva, enquanto "default" é uma escolha atribuída quando nenhuma é ativamente determinada. "Pattern", por outro lado, é 
simplesmente um comportamento repetitivo observado em contextos similares e que não necessariamente representa o jeito definitivo, ou mesmo o melhor. 

Historicamente, o livro da Gang of Four surgiu paralelamente a liguagem Java, o que inevitavelmente os atrelou bastante, de modo que muitos entendessem que um não funcionasse de modo independente do outro.
Assim, à medida que Java crescia, observou-se em muitos sistemas um uso de exagerado de padrões de projeto, muitas vezes em contextos nos quais
os ganhos de extensibilidade e flexibilidade eram questionáveis. 

Esse sintoma ficou conhecido como **paternite** e mereceu até comentário de John Ousterhout, autor de "A Philosophy of Software Design".

> O maior risco de padrões de projetos é a sua super-aplicação (over-application). Nem todo problema precisa ser resolvido por meio dos padrões de projeto; por isso, não tente forçar um problema a caber em um padrão de projeto quando uma abordagem tradicional funcionar melhor. O uso de padrões de projeto não necessariamente melhora o projeto de um sistema de software; isso só acontece se esse uso for justificado. Assim como ocorre com outros conceitos, a noção de que padrões de projetos são uma boa coisa não significa que quanto mais padrões de projeto usarmos, melhor será nosso sistema.

A confusão nasce da convicção de que o "Pattern" é sinônimo de "Standard", representando portanto o definitivo e, na maioria das vezes, melhor. 

## Exemplificando a crítica

O objetivo fundamental dos padrões é tornar o projeto mais flexível. Por exemplo, Factories facilitam a troca do tipo dos objetos manipulados, 
Decorators permitem personalizar a classe com novas fucnionalidades e Strategies permitem configurar os algoritmos usados por uma classe etc

Entretanto, cada um deles possui seus malefícios. Strategies requerem a criação de uma classe abstrata e mais uma classe para CADA algoritmo, Factory
exigem a implementação de, ao menos, mais uma classe etc. Portanto, cabe uma análise mais crítica ao utilizá-los. 

Via ser realmente necessária a criação de objetos de tipos diferentes no sistema? Esses objetos serão de fato necessários? São perguntas
que devem preceder a criação de uma Fábrica. Os algoritmos utilizados na implementação de uma classe precisarão ser parametrizados? Há, de fato, 
usuários que precisarão de algoritmos alternativos? São questionamentos anteriores ao código de um Strategy, por exemplo.

Levando Ousterhout a aprofundar o comentário, segundo ele Decorators criam complexidade desnecessária para a criação de arquivos em Java; pois é regra
a necessidade de buffers ao abrir qualquer arquivo. Portanto, classes como ```FileInputStream``` e ```BufferedInputStream``` poderiam ser unificadas.






















































