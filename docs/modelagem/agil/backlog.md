# Product Backlog Priorizado

## Introdução 

De forma simples, o Product Backlog é uma lista extensa de itens que compõem e são desejados no produto a ser desenvolvido. Esse artefato é mutável ao longo do projeto, então, novos itens podem ser adicionados, os itens já presentes podem sofrer alterações e ainda removidos. Por ter essas características, é muito comum encontrar o Product Backlog em projetos que usam metodologias ágeis, o que é o caso desse projeto, que, como explicitado, no artefato de [Escolhas Metodológicas](https://unbarqdsw2022-2.github.io/2022.2_G5_SoftSteakHouse/#/base/proce-metod-aborda/escolhas_metodologicas), segue Scrum.

Com os itens definidos, é importante ordená-los, para que haja conhecimento de quais são mais relevantes (e, portanto, devem receber mais atenção) e quais são poucos essenciais para a entrega e funcionamento do produto. Dessa forma, para realizar essa tarefa, a técnica **MoSCoW** foi a escolhida.

## Metodologia

### Product Backlog

Buscando a criação de Product Backlog com diferentes níveis de granularidade, isto é, a especificidade da descrição, foi seguido um padrão com 4 níveis (começando pelo menor nível e acabando com o maior):

- Épico
- Feature
- História de Usuário
- Critérios de Aceitação

Dessa forma, uma tabela foi criada com a identificação (ID) de cada uma das histórias, o épico e feature que a história pertence, também com seus critérios de aceitação. Além disso, pode-se encontrar a prioridade da história e sua rastreabilidade em artefatos anteriores.

Os integrantes participantes dessa técnica foram:

- [Caio César](https://github.com/oCaioOliveira): responsável pelos épicos 2 e 3. 
- [Victor Leão](https://github.com/victorleaoo): responsável pelos épicos 1 e 4.

### Priorização

Para realizar a priorização do itens (em especial, as histórias de usuário), foi usada a técnica MoSCoW, que trabalha com os seguintes níveis de prioridade:

- Must (Have): requisitos que são indispensáveis para o funcionamento do software.
- Should (Have): requisitos importantes, mas não vitais/críticos.
- Could (Have): requisitos desejáveis, mas que podem ser atendidos quando houver tempo e disposição.
- Would (Have): requisitos menos críticos, com menor retorno final.

## Product Backlog

| ID   | Épico | Feature | História de usuário | Priorização | Rastreabilidade | Critérios de Aceitação |
| ---- | ----- | ------- | --------------      | ----------- | ----            | ---------------        |
| US01 | E01 - Cadastro e Autenticação | FE01 - Recuperar a senha | Eu, como usuário do produto, quero poder recuperar minha senha para que sempre possa acessar as funcionalidades. | Could | [Prototipação](https://unbarqdsw2022-2.github.io/2022.2_G5_SoftSteakHouse/#/base/abordagem-geral/prototipo-alta-fidelidade) | O usuário deve inserir seu e-mail cadastrado para poder receber a recuperação de senha.<br>O usuário deve receber um e-mail com o processo de nova senha. |
| US02 | E01 - Cadastro e Autenticação | FE01 - Recuperar a senha | Eu, como administrador do sistema, quero poder recuperar minha senha para que sempre possa acessar as funcionalidades. | Should | [Prototipação](https://unbarqdsw2022-2.github.io/2022.2_G5_SoftSteakHouse/#/base/abordagem-geral/prototipo-alta-fidelidade) | O administrador deve inserir seu e-mail cadastrado para poder receber sua nova senha.<br>O administrador deve receber uma nova senha em seu e-mail. |
| US03 | E01 - Cadastro e Autenticação | FE02 - Login | Eu, como usuário do produto, quero poder realizar login para acessar funcionalidades restritas para usuários cadastrados. | Could | [Prototipação](https://unbarqdsw2022-2.github.io/2022.2_G5_SoftSteakHouse/#/base/abordagem-geral/prototipo-alta-fidelidade) | O usuário deve inserir seu e-mail e senha para realizar login.<br>O usuário deve ser notificado caso o login não seja efetuado por algum problema de autenticação. |
| US04 | E01 - Cadastro e Autenticação | FE02 - Login | Eu, como administrador do sistema, quero poder realizar login para acessar funcionalidades restritas para administradores. | Must | [Prototipação](https://unbarqdsw2022-2.github.io/2022.2_G5_SoftSteakHouse/#/base/abordagem-geral/prototipo-alta-fidelidade) | O administrador deve inserir seu e-mail cadastrador e senha pré-definida para realizar login.<br>O administrador deve ser notificado caso o login não seja efetuado por algum problema de autenticação. |
| US05 | E01 - Cadastro e Autenticação | FE03 - Logout | Eu, como usuário do sistema, quero poder realizar logout para não estar mais autenticado. | Could | [Prototipação](https://unbarqdsw2022-2.github.io/2022.2_G5_SoftSteakHouse/#/base/abordagem-geral/prototipo-alta-fidelidade) | O usuário deve ter um botão de 'Sair' disponível para realizar logout.<br>O usuário deve ser redirecionado para a tela inicial após sair. |
| US06 | E01 - Cadastro e Autenticação | FE03 - Logout | Eu, como administrador, quero poder realizar logout para não estar mais autenticado e não acessar mais funcionalidades e telas restritas. | Must | [Prototipação](https://unbarqdsw2022-2.github.io/2022.2_G5_SoftSteakHouse/#/base/abordagem-geral/prototipo-alta-fidelidade) | O administrador deve ter um botão de 'Sair' disponível para realizar logout.<br>O administrador deve ser redirecionado para a tela inicial após sair. |
| US07 | E01 - Cadastro e Autenticação | FE04 - Cadastro  | Eu, como usuário do produto, quero poder realizar cadastro para poder acessar funcionalidades acessíveis apenas para usuários autenticados. | Could | [Observação](https://unbarqdsw2022-2.github.io/2022.2_G5_SoftSteakHouse/#/base/abordagem-geral/requisitos) | O usuário deve poder acessar a tela específica para cadastro.<br>O usuário deve informar seus dados necessários para cadastro.<br>O usuário deve ser redirecionado para a tela de login após o cadastro. |
| US08 | E01 - Cadastro e Autenticação | FE04 - Cadastro | Eu, como administrador do sistema, quero poder solicitar cadastro para os desenvolvedores por meio do suporte disponível no site para poder acessar minhas funcionalidades específicas. | Must | [Introspecção](https://unbarqdsw2022-2.github.io/2022.2_G5_SoftSteakHouse/#/base/abordagem-geral/requisitos) | O administrador do sistema terá seus dados cadastrais fornecidos pelos desenvolvedores. |
| US09 | E02 - Cardápio | FE05 - Visualização do cardápio | Eu, como usuário do produto, quero visualizar o cardápio com todos os itens disponíveis do restaurante. | Must | [Introspecção](https://unbarqdsw2022-2.github.io/2022.2_G5_SoftSteakHouse/#/base/abordagem-geral/requisitos)<br>[Observação](https://unbarqdsw2022-2.github.io/2022.2_G5_SoftSteakHouse/#/base/abordagem-geral/requisitos)<br>[Rich Picture](https://unbarqdsw2022-2.github.io/2022.2_G5_SoftSteakHouse/#/base/abordagem-geral/rich_picture)<br>[Mapa Mental](https://unbarqdsw2022-2.github.io/2022.2_G5_SoftSteakHouse/#/base/abordagem-geral/mapa_mental) | O usuário deve visualizar o cardápio com os itens que o restaurante prepara.<br>Todos os itens do cardápio devem estar disponíveis na página inicial do cardápio com seu nome, preço e descrição. |
| US10 | E02 - Cardápio | FE05 - Visualização do cardápio | Eu, como usuário do produto, quero visualizar o cardápio separado por categorias, com objetivo de ter uma visão melhor sobre os itens e suas características. | Must | [Introspecção](https://unbarqdsw2022-2.github.io/2022.2_G5_SoftSteakHouse/#/base/abordagem-geral/requisitos) | O usuário deve visualizar o cardápio separando os itens por categorias.<br>Cada categoria deve ter seus itens dispostos abaixo de si. |
| US11 | E02 - Cardápio | FE06 - CRUD no cardápio | Eu, como administrador do sistema, quero cadastrar novos itens ao cardápio. | Must | [Introspecção](https://unbarqdsw2022-2.github.io/2022.2_G5_SoftSteakHouse/#/base/abordagem-geral/requisitos)<br>[Mapa Mental](https://unbarqdsw2022-2.github.io/2022.2_G5_SoftSteakHouse/#/base/abordagem-geral/mapa_mental) | O administrador deve cadastrar novos itens ao cardápio.<br>O administrador deve ser capaz de adicionar nome, preço, descrição, ingredientes e categoria do item. |
| US12 | E02 - Cardápio | FE06 - CRUD no cardápio | Eu, como administrador do sistema, quero editar itens disponíveis no cardápio. | Must | [Introspecção](https://unbarqdsw2022-2.github.io/2022.2_G5_SoftSteakHouse/#/base/abordagem-geral/requisitos) | O administrador deve editar itens no cardápio.<br>Cada item e seus respectivos atributos deve poder ser editáveis em uma tela única para cada um deles. |
| US13 | E02 - Cardápio | FE06 - CRUD no cardápio | Eu, como administrador do sistema, quero deletar itens disponíveis no cardápio. | Must | [Introspecção](https://unbarqdsw2022-2.github.io/2022.2_G5_SoftSteakHouse/#/base/abordagem-geral/requisitos) | O administrador deve deletar itens no cardápio.<br>O administrador deve ser perguntado se tem certeza que quer deletar o item. |
| US14 | E02 - Cardápio | FE07 - Visualização de itens do cardápio | Eu, como usuário do produto, quero visualizar um item individualmente ao selecioná-lo. | Should | [Introspecção](https://unbarqdsw2022-2.github.io/2022.2_G5_SoftSteakHouse/#/base/abordagem-geral/requisitos)<br>[Observação](https://unbarqdsw2022-2.github.io/2022.2_G5_SoftSteakHouse/#/base/abordagem-geral/requisitos) | O usuário deve visualizar um item individualmente ao selecioná-lo.<br>Cada item deve ter uma tela única para sua exposição. |
| US15 | E02 - Cardápio | FE07 - Visualização de itens do cardápio | Eu, como usuário do produto, quero visualizar adicionais a um item ao selecioná-lo. | Should | [Observação](https://unbarqdsw2022-2.github.io/2022.2_G5_SoftSteakHouse/#/base/abordagem-geral/requisitos) | O usuário deve visualizar adicionais de um item individualmente ao selecioná-lo.<br>Os adicionais devem ter seus preços mostrados. |
| US16 | E03 - Gerenciamento de Mesas | FE08 - Visualização da disponibilidade de mesas | Eu, como administrador do sistema, quero visualizar a disponibilidade de mesas para cada quantidade de pessoas. | Must | [Prototipação](https://unbarqdsw2022-2.github.io/2022.2_G5_SoftSteakHouse/#/base/abordagem-geral/prototipo-alta-fidelidade)<br>[Rich Picture](https://unbarqdsw2022-2.github.io/2022.2_G5_SoftSteakHouse/#/base/abordagem-geral/rich_picture)<br>[Mapa Mental](https://unbarqdsw2022-2.github.io/2022.2_G5_SoftSteakHouse/#/base/abordagem-geral/mapa_mental)<br>[Introspecção](https://unbarqdsw2022-2.github.io/2022.2_G5_SoftSteakHouse/#/base/abordagem-geral/requisitos) | O administrador do sistema deve visualizar a disponiblidade de cada mesa.<br>Devem ser mostradas a quantidade de mesas para cada tipo de mesa<br>Os tipos de mesa devem ser de acordo com a quantidade de pessoas que elas acomodam. |
| US17 | E03 - Gerenciamento de Mesas | FE09 - Alteração a disponibilidade de mesas | Eu, como administrador do sistema, quero editar a disponibilidade de mesas para cada quantidade de pessoas. | Must | [Prototipação](https://unbarqdsw2022-2.github.io/2022.2_G5_SoftSteakHouse/#/base/abordagem-geral/prototipo-alta-fidelidade)<br>[Rich Picture](https://unbarqdsw2022-2.github.io/2022.2_G5_SoftSteakHouse/#/base/abordagem-geral/rich_picture)<br>[Mapa Mental](https://unbarqdsw2022-2.github.io/2022.2_G5_SoftSteakHouse/#/base/abordagem-geral/mapa_mental)<br>[Introspecção](https://unbarqdsw2022-2.github.io/2022.2_G5_SoftSteakHouse/#/base/abordagem-geral/requisitos) | O administrador do sistema deve editar a disponiblidade de cada mesa.<br>A mudança de disponibilidade deve ser feita de acordo com a quantidade de mesas disponíveis e ocupadas |
| US18 | E03 - Gerenciamento de Mesas | FE09 - Reserva de mesas para usuários | Eu, como usuário do produto, quero reservar uma mesa. | Could | [Observação](https://unbarqdsw2022-2.github.io/2022.2_G5_SoftSteakHouse/#/base/abordagem-geral/requisitos)<br>[Rich Picture](https://unbarqdsw2022-2.github.io/2022.2_G5_SoftSteakHouse/#/base/abordagem-geral/rich_picture) | O usuário deve reservar uma mesa de sua vontade.<br>O usuário deve informar para quantas pessoas ele reservará sua mesa. |
| US19 | E04 - Gerenciamento de Pedidos | FE10 - CRUD de pedido | Eu, como funcionário, quero adicionar itens a um novo pedido para que ele possa estar disponível. | Could | [Rich Picture](https://unbarqdsw2022-2.github.io/2022.2_G5_SoftSteakHouse/#/base/abordagem-geral/rich_picture)<br>[Mapa Mental](https://unbarqdsw2022-2.github.io/2022.2_G5_SoftSteakHouse/#/base/abordagem-geral/mapa_mental) | O funcionário deve ser capaz de adicionar os itens e suas quantidades no pedido.<br>O funcionário deve direcionar o pedido à uma mesa.<br>O estado do pedido inicialmente deve ser 'Novo Pedido'. |
| US20 | E04 - Gerenciamento de Pedidos | FE10 - CRUD de pedido | Eu, como funcionário, quero ver todos os pedidos realizados em um dia para que eu possa ter um controle dos pedidos feitos. | Would | [Rich Picture](https://unbarqdsw2022-2.github.io/2022.2_G5_SoftSteakHouse/#/base/abordagem-geral/rich_picture)<br>[Mapa Mental](https://unbarqdsw2022-2.github.io/2022.2_G5_SoftSteakHouse/#/base/abordagem-geral/mapa_mental) | O funcionário deve ser capaz de ver todos os pedidos em uma única página.<br>Cada pedido deve ter uma página única com seus itens e mesa. |
| US21 | E04 - Gerenciamento de Pedidos | FE10 - CRUD de pedido | Eu, como funcionário, quero poder editar um pedido para mudar algo, caso necessário. | Would | [Rich Picture](https://unbarqdsw2022-2.github.io/2022.2_G5_SoftSteakHouse/#/base/abordagem-geral/rich_picture)<br>[Mapa Mental](https://unbarqdsw2022-2.github.io/2022.2_G5_SoftSteakHouse/#/base/abordagem-geral/mapa_mental) | Cada pedido deve ter uma opção de edição em suas telas únicas. |
| US22 | E04 - Gerenciamento de Pedidos | FE10 - CRUD de pedido | Eu, como funcionário, quero poder deletar um pedido. | Could | [Rich Picture](https://unbarqdsw2022-2.github.io/2022.2_G5_SoftSteakHouse/#/base/abordagem-geral/rich_picture)<br>[Mapa Mental](https://unbarqdsw2022-2.github.io/2022.2_G5_SoftSteakHouse/#/base/abordagem-geral/mapa_mental) | Deve haver um botão de apagar pedido na tela de pedidos.<br>O funcionário deve ser pedido para confirmar a deleção do pedido. |
| US23 | E04 - Gerenciamento de Pedidos | FE11 - Mudança de estado de pedido | Eu, como funcionário, quero poder mudar o estado de um pedido, para que ele possa ser acompanhado de forma visível. | Could | [Rich Picture](https://unbarqdsw2022-2.github.io/2022.2_G5_SoftSteakHouse/#/base/abordagem-geral/rich_picture)<br>[Mapa Mental](https://unbarqdsw2022-2.github.io/2022.2_G5_SoftSteakHouse/#/base/abordagem-geral/mapa_mental) | Somente pedidos não fechados podem ser alterados.<br>Os pedidos podem ser 'Novo Pedido', 'Sendo Feito', 'Para Entrega em Mesa', 'Entregue' e 'Fechado'. |

## RoadMap

Esta seção é destinada para apresentar as atividades realizadas pela equipe por sprint.

Sprint 1 | Sprint 2 | Sprint 3 | Sprint 4 | Sprint 5 |
-------- | -------- | -------  | -------- | -------- |
5W2H     | 5W2H |          |          |          | 
Plano de riscos | Protótipo de alta fidelidade  |          |          |          | 
Protótipo de média fidelidade | Product backlog |          |          |          | 
Guia de estilo |  BPMN |          |          |          | 
Product backlog | MOSCOW  |          |          |          | 
Rich picture  | Validação do protótipo |          |          |          | 
Mapa mental | Diagrama de Classes |          |          |          | 
Plano de custo | Diagrama de Pacotes |          |          |          | 
Plano de tempo  | Diagrama de Componentes |          |          |          | 
Design sprint | Diagrama de Implementação |          |          |          | 
Escolhas metodológicas  |Diagrama de Sequência |          |          |          | 
Personas | Diagrama de Comunicação|          |          |          | 
Léxicos |Diagrama de Estados |          |          |          | 
BPMN  | Diagrama de Atividades|          |          |          | 
Diagrama causa-efeito |       |          |          |          | 

## Histórico de Versões

| Data  | Versão | Descrição | Autor | Revisor |
| --- | --- | --- | --- | --- |
| 03/12/2022 | 0.1 | Criação do documento | [Caio César](https://github.com/oCaioOliveira) | [Victor Leão](https://github.com/victorleaoo) |
| 03/12/2022 | 0.2 | Criação dos épicos e features | [Caio César](https://github.com/oCaioOliveira) | [Victor Leão](https://github.com/victorleaoo) |
| 03/12/2022 | 0.3 | Criação de histórias de usuários nos épicos 2 e 3 | [Caio César](https://github.com/oCaioOliveira) | [Victor Leão](https://github.com/victorleaoo) |
| 03/12/2022 | 0.4 | Criação de histórias de usuários nos épicos 1 e 4 | [Victor Leão](https://github.com/victorleaoo) | [Caio César](https://github.com/oCaioOliveira) |
| 03/12/2022 | 0.5 | Adição do RoadMap | [Caio César](https://github.com/oCaioOliveira) | [Victor Leão](https://github.com/victorleaoo) |

## Referências

**PRODUCT BACKLOG | ELEMENTOS BASE DO FRAMEWORK SCRUM**, 2018. Disponível em: https://www.youtube.com/watch?v=Gh9PEgZIBCo. Acesso em: 03 dez. 2022.
