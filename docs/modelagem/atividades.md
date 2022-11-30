# Diagrama de Atividades

## Introdução
O Diagrama de Atividades é um diagrama dinâmico que mostra o fluxo entre os objetos, ou seja, a parte comportamental, representando-a como um fluxo de ações. O foco se encontra nos procedimentos, processos de negócio e fluxo de trabalho.

## Metodologia

O Diagrama de Atividades tem 5 elementos principais na sua composição:
1. Atividades
>Na UML, as atividades são elementos de contêiner que descrevem o nível mais alto do comportamento em um diagrama de atividades. As atividades contêm diversos nós de atividade e linhas de atividade que representam a seqüência de tarefas em um fluxo de trabalho que resulta em um comportamento.
2. Ações
>Na UML, uma ação representa uma unidade discreta de funcionalidade em uma atividade.
3. Nós de Controle
>Nos diagramas de atividade, um nó de controle é um nó de atividade abstrata que coordena o fluxo de controle em uma atividade.
4. Nós do Objeto
>Nos diagramas de atividades, um nó de objeto é um nó de atividade abstrato que ajuda a definir o fluxo de objetos em uma atividade. Um nó de objeto indica que uma instância de um classificador pode estar disponível em um ponto específico na atividade.
5. Linhas de Atividade
>Nos diagramas de atividades, uma extremidade de atividade é uma conexão direcionada entre dois nós de atividade. Quando uma ação específica em uma atividade é concluída, a linha de atividade continua o fluxo para a próxima ação na seqüência.

A partir do entendimento da diagramação e de seus elementos, foram desenvolvidos diagramas para 3 tipos de casos de usos diferentes encontrados no projeto:
* Reserva de mesa
* Geral, que é composto por acessar o cardápio online, gerenciar o pedido e gerenciar mesa

## Diagramas

### Reserva de mesa

![Diagrama de atividades Reserva de mesa](./assets/reserva_de_mesa.png)

### Geral
![Diagrama de atividades Geral](./assets/geral.png)

## Histório de versão

Data | Versão |Descrição |Autor | Revisor
-----|--------|----------|------|--------
30/11/2022| 1.0.0| Elaboração do artefato de Diagrama de Atividades | Carla | --

## Referências
SERRANO, Milene. Diagrama de Colaboração, 2022. Material apresentado na Disciplina de Arquitetura e Desenho de Software do curso de engenharia de software da UnB, FGA. Acesso em: 30 nov. 2022.

UML DIAGRAMS. UML Communication Diagrams Overview. Disponível em: https://www.uml-diagrams.org/communication-diagrams.html. Acesso em: 30 nov. 2022.

Diagramas de Atividades. Disponível em: https://www.ibm.com/docs/pt-br/rational-soft-arch/9.7.0?topic=diagrams-activity. Acesso em: 30 nov. 2022.

