# DAS - Documento de Arquitetura de Software

## 1. Introdução

O Documento de Arquitetura de Software (DAS) é um artefato que apresenta a arquitetura de um projeto de software desenvolvido em diferentes visões. Para o software Soft SteakHouse, o DAS apresentará as visões arquiteturais de Casos de Uso, Lógica, Implantação, Implementação e Dados (camada de persistência). Além disso, Tamanho e Desempenho também serão tópicos analisados no artefato.

### 1.1 Propósito

Como explicitado acima, o propósito desse documento é apresentar uma visão geral arquitetural do sistema a partir de diferentes visões arquiteturais, detalhando, assim, diferentes aspectos do sistema. Busca-se capturar e mostrar as decisões arquiteturais significantes que foram feitas ao longo do desenvolvimento do software Soft SteakHouse.

### 1.2 Escopo

O Documento de Arquitetura de Software se aplica ao projeto Soft SteakHouse desenvolvido no segundo semestre de 2022 (2.2022) da Universidade de Brasília para a disciplina Arquitetura e Desenho de Software. Com esse artefato, a arquitetura do projeto é explicada e destrinchada, afetando e influenciando quem buscar por tais informações (desde a equipe de desenvolvimento até interessados pela arquitetura utilizada).

De forma geral, o projeto possui o foco em resolver problemas para restaurantes que desejam passar por um processo de digitalização de alguns de seus serviços. Como pode ser melhor observado no [Product Backlog](https://unbarqdsw2022-2.github.io/2022.2_G5_SoftSteakHouse/#/modelagem/agil/backlog) da aplicação, as funcionalidades que receberam maior enfoque e, portanto, são essenciais para o produto, foram a de apresentação de cardápio digital e gerenciamento de mesas, além do acesso pelo administrador do restaurante.

O escopo imaginado da aplicação, com uma visão mais geral conceitual da mesma, pode ser vista de forma mais completa em alguns artefatos:

- [Mapa Mental](https://unbarqdsw2022-2.github.io/2022.2_G5_SoftSteakHouse/#/base/abordagem-geral/mapa_mental)

![Mapa Mental Exemplo Escopo](../../base/abordagem-geral/assets/MapaMental-Caio.jpeg)

<center>
<figcaption>Imagem: Exemplo Mapa Mental do Projeto</figcaption>
<figcaption>Autor: Caio (Integrante do Grupo)</figcaption>
</center>

- [Rich Picture](https://unbarqdsw2022-2.github.io/2022.2_G5_SoftSteakHouse/#/base/abordagem-geral/rich_picture)

![Rich Picture Exemplo Escopo](../../base/abordagem-geral/assets/RichPicture1.jpg)

<center>
<figcaption>Imagem: Exemplo Rich Picture do Projeto</figcaption>
<figcaption>Autor: Hian (Integrante do Grupo)</figcaption>
</center>

### 1.3 Definições, acrônimos e abreviações

A tabela abaixo possui algumas definições, acrônimos e abreviações importantes que deve-se conhecer para interpretar o DAS. 

| Abreviação | Acrônimo | Definição |
| :--------: | :------: | :-------- |
| DAS | Documento de Arquitetura de Software | Artefato desenvolvido nessa página, que apresenta a arquitetura do projeto Soft SteakHouse com diversas visões |
| MTV | Model Template View | Modelo arquitetural dividido em 3 camadas usado pelo framework Django em Python |
| SGBD | Sistema Gerenciador de Banco de Dados | Software usado para gerenciar e manipular a base de dados (armazenamento persistente) do projeto |
| AWS | Amazon Web Services | Serviços de nuvens da empresa Amazon |

O artefato de [léxicos](https://unbarqdsw2022-2.github.io/2022.2_G5_SoftSteakHouse/#/base/abordagem-geral/lexicos) também ajuda a entender alguns outros termos relacionados ao projeto.

### 1.4 Visão Geral

A partir da introdução, pode-se entender um pouco o quê é o DAS e seu propósito, então, abaixo, o documento se expande, apresentando a arquitetura do projeto, desde uma forma geral, até cada uma das visões (lógica, implementação, implantação e dados).

## 2. Representação Arquitetural

Antes de explicar a arquitetura do sistema em diferentes visões, é importante entender a divisão inicial de frameworks no back-end (onde a lógica de negócio é desenvolvida) e front-end (apresentação para o usuário). É interessante mencionar que no projeto existem [templates de implementação](https://unbarqdsw2022-2.github.io/2022.2_G5_SoftSteakHouse/#/templates-implementacao/templates) para as duas frentes, auxiliando tanto os desenvolvedores na aplicação, quanto para quem deseja entender como o sistema está sendo desenvolvido.

### 2.1 Back-End

Primeiramente, para o back-end, foi escolhida a linguagem Python para o desenvolvimento. O motivo de tal seleção foi, principalmente, pela familiaridade por maior parte dos integrantes do grupo, além da concordância geral que o desenvolvimento de uma aplicação web poderia ser beneficiado por certos frameworks disponíveis para a linguagem.

Assim, o framework Django foi selecionado, também por causa do conhecimento e experiência prévia de membros da equipe e, portanto, o risco para o desenvolvimento seria menor e menos tempo seria gasto no aprendizado da ferramenta. Como modelo arquitetural, então, foi adotado, "automaticamente" o [MTV (Model Template View)](https://unbarqdsw2022-2.github.io/2022.2_G5_SoftSteakHouse/#/padroes-projeto/padrao-extra/django), uma vez que é o padrão implementado pelo framework.

### 2.2 Banco de Dados

O SGBD usado no projeto foi o PostgreSQL, uma vez que é o sistema gerenciador padrão implementado pelo Django e os dados armazenados pelo projeto são relacionais.

A ferramenta AWS é encontrada, também, no projeto para o armazenamento das imagens dos itens, similar a um repositório. A tecnologia trabalha em forma de nuvem.

### 2.3 Front-End

Por outro lado, para o front-end, o desenvolvimento foi realizado com a linguagem JavaScript, a partir da biblioteca React. Essa ferramenta foi selecionada pelo mesmo motivo das escolhas de back-end, sendo então, a familiaridade e entendimento já existente por alguns membros do grupo, o principal deles. Além disso, é uma biblioteca com grande utilização pelo mercado, o que facilita o trabalho de buscas e pesquisas para o desenvolvimento.

A ferramenta Docker também foi implementada para a integração em ambiente isolados, para que todos os membros pudessem executar a aplicação de forma semelhante independente de sua configuração pessoal.

## 3. Metas e Restrições Arquiteturais

### 3.1 Metas

Abaixo estão listados alguns requisitos e objetivos do software, com impacto significativo na arquitetura.

| Categoria | Metas |
| :-------: | :---- |
| Segurança e confiabilidade | A aplicação deve garantir proteção aos dados sensíveis dos usuários.</br>Falhas ou erros devem ser reportados ao usuário.</br>O sistema deve fornecer a capacidade de autenticação com credenciais únicas (cada usuário é identificado unicamente por um e-mail e senha). |
| Portabilidade e suportabilidade | O usuário deve conseguir acessar a aplicação web em navegadores tanto de desktop, quanto mobile. |
| Responsividade | As páginas desenvolvidas devem ser responsivas ao tamanho de tela do usuário. |
| Escalabilidade | O software deve ser desenvolvido para suportar novas evoluções (escalar), tanto de funcionalidades, quanto de dados. |

### 3.2 Restrições

Algumas restrições especiais também são aplicadas à arquitetura, abaixo elas estão listadas.

| Categoria | Restrições |
| :-------: | :--------- |
| Conectividade | O usuário deve estar conectado à internet para utilizar o sistema.</br>O usuário deve ter acesso a um navegador da web. |
| Idioma | As funcionalidades desenvolvidas devem estar em português. |
| Cronograma | O sistema deve estar disponível até, pelo menos, o fim do segundo semestre de 2.2022 da Universidade de Brasília (18 de fevereiro de 2023). | 
| Estrutura do Time | A equipe segue a estrutura da [metodologia ágil](https://unbarqdsw2022-2.github.io/2022.2_G5_SoftSteakHouse/#/base/proce-metod-aborda/escolhas_metodologicas) Scrum.</br>A equipe é formada de 8 membros. |
| Ferramentas de desenvolvimento | React (front-end), Django (back-end) e PostgreSQL (SGBD) |

### 4 Visões

#### [4.1 Geral](arquitetura-reutilizacao/das/visao_geral.md)

#### [4.2 Casos de Uso](arquitetura-reutilizacao/das/visao_casos_uso.md)

#### [4.3 Lógica](arquitetura-reutilizacao/das/visao_logica.md)

#### [4.4 Implementação](arquitetura-reutilizacao/das/visao_implementacao.md)

#### [4.5 Processos](arquitetura-reutilizacao/iniciativas-extras/das_visao_processos.md)

#### [4.6 Implantação](arquitetura-reutilizacao/das/visao_implantacao.md)

#### [4.7 Dados](arquitetura-reutilizacao/das/visao_dados.md)

## 5. Tamanho e Performance

[A description of the major dimensioning characteristics of the software that impact the architecture, as well as the target performance constraints.]

## Histórico de Versões

|    Data    | Versão |            Descrição           |       Autor     |    Revisor    |
|  --------  |  ----  |            ----------          | --------------- |    -------    |
| 23/01/2023 |  1.0.0 |  Criação da estrutura inicial em tópicos e preenchimento da introdução, representação arquitetural, metas e restrições arquiteturais, visão de casos de uso e visão lógica. | [Victor Leão](https://github.com/victorleaoo) | [Caio César](https://github.com/oCaioOliveira) |

## Referências

1. BENHAROSH, Joseph. What is REST API? in plain English. Disponível em: https://phpenthusiast.com/blog/what-is-rest-api. Acesso em: 24 jan. 2023.

2. AMAZON. O que é API RESTful?. Disponível em: https://aws.amazon.com/pt/what-is/restful-api/. Acesso em: 24. jan. 2023.
