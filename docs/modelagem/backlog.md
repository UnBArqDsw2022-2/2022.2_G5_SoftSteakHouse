# Product Backlog Priorizado

## Introdução 

De forma simples, o Product Backlog é uma lista extensa de itens que compõem e são desejados no produto a ser desenvolvido. Esse artefato é mutável ao longo do projeto, então, novos itens podem ser adicionados, os itens já presentes podem sofrer alterações e ainda removidos. Por ter essas características, é muito comum encontrar o Product Backlog em projetos que usam metodologias ágeis, o que é o caso desse projeto, que, como explicitado, no artefato de [Escolhas Metodológicas](https://unbarqdsw2022-2.github.io/2022.2_G5_SoftSteakHouse/#/base/proce-metod-aborda/escolhas_metodologicas), segue Scrum.

Com os itens definidos, é importante ordená-los, para que haja conhecimento de quais são mais relevantes (e, portanto, devem receber mais atenção) e quais são poucos essenciais para a entrega e funcionamento do produto. Dessa forma, para realizar essa tarefa, a técnica **MoSCoW** foi a escolhida.

## Metodologia

### Product Backlog

Buscando a criação de Product Backlog com diferentes níveis de granularidade, isto é, a especificidade da descrição, foi seguido um padrão com 5 níveis (começando pelo menor nível e acabando com o maior):

- Épico
- Feature
- História de Usuário
- Critérios de Aceitação
- Tarefas

Dessa forma, uma tabela foi criada com a identificação (ID) de cada uma das histórias, o épico e feature que a história pertence, também com seus critérios de aceitação. Além disso, pode-se encontrar a prioridade da história e sua rastreabilidade em artefatos anteriores.

### Priorização

Para realizar a priorização do itens (em especial, as histórias de usuário), foi usada a técnica MoSCoW, que trabalha com os seguintes níveis de prioridade:

- Must (Have): requisitos que são indispensáveis para o funcionamento do software.
- Should (Have): requisitos importantes, mas não vitais/críticos.
- Could (Have): requisitos desejáveis, mas que podem ser atendidos quando houver tempo e disposição.
- Would (Have): requisitos menos críticos, com menor retorno final.

## Product Backlog

| ID   | Épico | Feature | História de usuário | Priorização | Rastreabilidade | Critérios de Aceitação |
| ---- | ----- | ------- | --------------      | ----------- | ----            | ---------------        |
| US01 | E01 - Cadastro e Autenticação | FE01 - Recuperar a senha | Eu, como usuário do produto, quero poder recuperar minha senha para que sempre possa acessar as funcionalidades. | Must | Rastreabilidade | Critérios de Aceitação |
| US02 | E01 - Cadastro e Autenticação | FE01 - Recuperar a senha | Eu, como administrador do sistema, quero poder recuperar minha senha para que sempre possa acessar as funcionalidades. | Must | Rastreabilidade | Critérios de Aceitação |
| US0 | E01 - Cadastro e Autenticação | FE02 - Login | História de usuário | Must | Rastreabilidade | Critérios de Aceitação |
| US0 | E01 - Cadastro e Autenticação | FE03 - Logout | História de usuário | Must | Rastreabilidade | Critérios de Aceitação |
| US0 | E01 - Cadastro e Autenticação | FE04 - Cadastro de usuário | História de usuário | Must | Rastreabilidade | Critérios de Aceitação |
| US0 | E02 - Cardápio | FE05 - Visualização do cardápio | Eu, como usuário do produto, quero visualizar o cardápio com todos os itens disponíveis do restaurante. | Must | [Requisitos](../base/abordagem-geral/product_backlog.md) | O usuário deve visualizar o cardápio com os itens que o restaurante prepara. |
| US0 | E02 - Cardápio | FE05 - Visualização do cardápio | Eu, como usuário do produto, quero visualizar o cardápio separado por categorias, com objetivo de ter uma visão melhor sobre os itens e suas características. | Must | [Requisitos](../base/abordagem-geral/product_backlog.md) | O usuário deve visualizar o cardápio separando os itens por categorias. |
| US0 | E02 - Cardápio | FE06 - CRUD no cardápio | Eu, como administrador do sistema, quero cadastrar novos itens ao cardápio. | Must | [Requisitos](../base/abordagem-geral/product_backlog.md) | O administrador deve cadastrar novos itens ao cardápio. |
| US0 | E02 - Cardápio | FE06 - CRUD no cardápio | Eu, como administrador do sistema, quero editar itens disponíveis no cardápio. | Must | [Requisitos](../base/abordagem-geral/product_backlog.md) | O administrador deve editar itens no cardápio. |
| US0 | E02 - Cardápio | FE06 - CRUD no cardápio | Eu, como administrador do sistema, quero deletar itens disponíveis no cardápio. | Must | [Requisitos](../base/abordagem-geral/product_backlog.md) | O administrador deve deletar itens no cardápio. |
| US0 | E02 - Cardápio | FE07 - Visualização de itens do cardápio | Eu, como usuário do produto, quero visualizar um item individualmente ao selecioná-lo. | Should | [Requisitos](../base/abordagem-geral/product_backlog.md) | O usuário deve visualizar um item individualmente ao selecioná-lo. |
| US0 | E02 - Cardápio | FE07 - Visualização de itens do cardápio | Eu, como usuário do produto, quero visualizar adicionais a um item ao selecioná-lo. | Should | [Requisitos](../base/abordagem-geral/product_backlog.md) | O usuário deve visualizar adicionais de um item individualmente ao selecioná-lo. |
| US0 | E03 - Gerenciamento de Mesas | FE08 - Visualização da disponibilidade de mesas | Eu, como administrador do sistema, quero visualizar a disponibilidade de mesas para cada quantidade de pessoas. | Must | [Requisitos](../base/abordagem-geral/product_backlog.md) | O administrador do sistema deve visualizar a disponiblidade de cada mesa. |
| US0 | E03 - Gerenciamento de Mesas | FE09 - Alteração a disponibilidade de mesas | Eu, como administrador do sistema, quero editar a disponibilidade de mesas para cada quantidade de pessoas. | Must | [Requisitos](../base/abordagem-geral/product_backlog.md) | O administrador do sistema deve editar a disponiblidade de cada mesa. |
| US0 | E03 - Gerenciamento de Mesas | FE09 - Reserva de mesas para usuários | Eu, como usuário do produto, quero reservar uma mesa. | Could | Rastreabilidade | O usuário deve reservar uma mesa de sua vontade. |
| US0 | E04 - Gerenciamento de Pedidos | FE10 - CRUD de pedido | História de usuário | Must | Rastreabilidade | Critérios de Aceitação |
| US0 | E04 - Gerenciamento de Pedidos | FE11 - Mudança de estado de pedido | História de usuário | Must | Rastreabilidade | Critérios de Aceitação |

## Histórico de Versões

| Data  | Versão | Descrição | Autor | Revisor |
| --- | --- | --- | --- | --- |
| 03/12/2022 | 0.1 | Criação do documento | [Caio César](https://github.com/oCaioOliveira) | [Victor Leão](https://github.com/victorleaoo) |
| 03/12/2022 | 0.2 | Criação dos épicos e features | [Caio César](https://github.com/oCaioOliveira) | [Victor Leão](https://github.com/victorleaoo) |
| 03/12/2022 | 0.3 | Criação de histórias de usuários nos épicos 2 e 3 | [Caio César](https://github.com/oCaioOliveira) | [Victor Leão](https://github.com/victorleaoo) |

## Referências

**PRODUCT BACKLOG | ELEMENTOS BASE DO FRAMEWORK SCRUM**, 2018. Disponível em: https://www.youtube.com/watch?v=Gh9PEgZIBCo. Acesso em: 03 dez. 2022.