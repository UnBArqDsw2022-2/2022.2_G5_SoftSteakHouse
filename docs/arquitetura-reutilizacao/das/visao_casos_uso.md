## Visão de Casos de Uso

Para guiar melhor ainda o Documento de Arquitetura de Software que está sendo lido, essa seção vai listar algumas das funcionalidades mais significantes da aplicação para trazer uma compreensão mais elaborada do sistema que foi desenvolvido. Além disso, essas funcionalidades podem refletir e explicar, de alguma forma, algumas das escolhas e decisões arquiteturais tomadas. Como não foi feito um artefato de casos de uso para os requisitos do projeto durante a parte de elicitação, abaixo serão especificadas histórias de usuário e, como deve-se indicar as mais importantes, serão destacadas a com priorização 'Must' (a maior na técnica de priorização MoSCoW). Importante mencionar que essas histórias de usuário podem ser encontradas mais detalhadas no [Product Backlog](https://unbarqdsw2022-2.github.io/2022.2_G5_SoftSteakHouse/#/modelagem/agil/backlog).

- **US04:** Eu, como administrador do sistema, quero poder realizar login para acessar funcionalidades restritas para administradores.
- **US06:** Eu, como administrador, quero poder realizar logout para não estar mais autenticado e não acessar mais funcionalidades e telas restritas.
- **US08:** Eu, como administrador do sistema, quero poder solicitar cadastro para os desenvolvedores por meio do suporte disponível no site para poder acessar minhas funcionalidades específicas.
- **US09:** Eu, como usuário do produto, quero visualizar o cardápio com todos os itens disponíveis do restaurante.
- **US10:** Eu, como usuário do produto, quero visualizar o cardápio separado por categorias, com objetivo de ter uma visão melhor sobre os itens e suas características.
- **US11:** Eu, como administrador do sistema, quero cadastrar novos itens ao cardápio.
- **US12:** Eu, como administrador do sistema, quero editar itens disponíveis no cardápio.
- **US13:** Eu, como administrador do sistema, quero deletar itens disponíveis no cardápio.
- **US16:** Eu, como administrador do sistema, quero visualizar a disponibilidade de mesas para cada quantidade de pessoas.
- **US17:** Eu, como administrador do sistema, quero editar a disponibilidade de mesas para cada quantidade de pessoas.

### Realizações de Casos de Usos

Para a aplicação de algumas das funcionalidades citadas acima, foi implementada uma API RESTful com o Django, que conceitualmente pode ser explicada como uma interface que dois sistemas de computador usam para trocar informações de forma segura pela internet, de acordo com a Amazon AWS. Assim, pode-se caracterizar o uso de uma **arquitetura cliente-servidor**, uma vez que um cliente faz requisições/solicitações via protocolo HTTP e, então, ela é processada e respondida por um servidor. A figura abaixo representa bem como funciona uma API RESTful e, de semelhante modo, uma arquitetura cliente-servidor.

![Exemplo RESTful](./apirest.png)

<center>
<figcaption>Imagem: Funcionamento de uma API RESTful/Arquitetura cliente-servidor</figcaption>
<figcaption>Fonte: phpenthusiast[1]</figcaption>
</center>

Dessa forma, as funcionalidades que estão relacionadas a cadastro, edição, deleção e visualização são implementadas por meio dessa arquitetura no sistema.