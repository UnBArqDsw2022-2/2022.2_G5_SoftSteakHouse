# Padrões de Projeto GRASP(s)

## Introdução

Os padrões de projeto GRASP são guiados pelo Projeto Guiado por Responsabilidades (PGR).

Um Projeto Guiado por Responsabilidades (PGR) é uma forma de criar desenhos de software com base em responsabilidades, papéis e colaborações. No caso de um software, os objetos desempenham papéis, responsabilidades são as obrigações do objeto no papel dele, sendo 'fazer' (realizar algo, iniciar uma ação em outros objetos e controlar atividades em outros objetos) e 'conhecer' (conhecer sobre dados privados encapsulados, objetos relacionados e coisas que ele pode derivar ou calcular) duas responsabilidades de um objeto.

Padrões de projeto são princípios e soluções usados durante a criação de um software, codificados em um formato estruturado, descrevendo o problema e a respectiva solução adotada. Com isso, GRASP (General Responsability Assignment Software Patterns), ou Padrões de Software para Atribuição de Responsabilidade Geral em português, é um tipo de padrões de projeto que pode ser aplicado para o desenvolvimento de um projeto. Em outras palavras, os padrões GRASP são princípios descritos de modo metódico, explicável e repetível para atribuir as responsabilidades (fazer e conhecer) dos papéis (objetos).

A primeira literatura que os cita é o 'Utilizando UML e Padrões', Craig Larman, primeiramente publicado em 1997. O livro é renomado, sendo recomendado até por Martin Fowler, grande nome na área de arquitetura de software, especialmente na orientação de objetos e UML (abordados durante o projeto).

Existem 9 princípios, os problemas que eles resolvem estão representados abaixo, mas aqueles que foram usados no projeto estão melhor explicados em seus artefatos específicos:

- **Criador:** Quem deve ser responsável pela criação de uma nova instância de uma classe?
- **Especialista:** Qual é um princípio geral de atribuição de responsabilidade a objetos?
- **Alta Coesão:** Como manter os objetos bem focados, com propósitos claros, gerenciáveis e com acoplamento baixo?
- **Baixo Acoplamento:** Como apoiar a baixa dependência, o baixo impacto de modificações e o aumento de reutilização?
- **Controladora:** Qual é o primeiro objeto além da camada de IU que recebe e coordena uma operação do sistema?
- **Polimorfismo:** Como tratar alternativas com base no tipo do objeto?
- **Invenção Pura ou Fabricação Própria:** Uma responsabilidade deve ser alocada a um objeto (geralmente sugerida pelo padrão Especialista), mas irá atrapalhar a Coesão e/ou o Acoplamento daquele objeto.
- **Indireção:** Como distribuir responsabilidades entre objetos de modo a evitar acoplamento direto entre dois (ou mais) objetos?
- **Variações Protegidas:** Como projetar objetos, subsistemas e sistemas de modo que as variações ou instabilidades nesses elementos não tenham impacto indesejável sobre outros elementos?

## Histórico de Versões

|    Data    | Versão |            Descrição           |       Autor     |    Revisor    |
|  --------  |  ----  |            ----------          | --------------- |    -------    |
| 01/01/2023 |  1.0.0 |  Criação do artefato de GRASP | [Victor Leão](https://github.com/victorleaoo) | - |

## Referências
SERRANO, Milene. GRASP, 2022. Material apresentado na Disciplina de Arquitetura e Desenho de Software do curso de engenharia de software da UnB, FGA. Acesso em: 01 jan. 2023.

PINTO, Rodrigo V. Padrões Esquecidos - GRASP. LinkedIn, 2022. Disponível em: https://www.linkedin.com/pulse/padr%C3%B5es-esquecidos-grasp-rodrigo-vieira-pinto-msc/. Acesso em: 01. jan. 2023.