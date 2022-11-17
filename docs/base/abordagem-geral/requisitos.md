# Elicitação de Requisitos

## Histórico de versões

|    Data    | Versão |      Descrição       |                   Autor(a)                    |                   Revisor(a)                    |
| ---------- | ------ | -------------------- | --------------------------------------------- | ----------------------------------------------- |
| 13/11/2022 |  0.1   | Criação do documento | [Caio César](https://github.com/oCaioOliveira)| [Victor Leão](https://github.com/victorleaoo)   |
| 13/11/2022 |  0.2   | Adição dos requisitos funcionais e regras de negócio por introspecção | [Caio César](https://github.com/oCaioOliveira)| [Victor Leão](https://github.com/victorleaoo)   |
| 14/11/2022 |  0.3   | Adição de uma breve introdução acerca da introspecção,<br/> adição de um 'I' na frente de cada um dos requisitos elicitados por introspecção,<br/> Adição da técnica de observação | [Victor Leão](https://github.com/victorleaoo) | [Caio César](https://github.com/oCaioOliveira) |
| 14/11/2022 |  0.4   | Adição de novos requisitos por meio da técnica de introspecção, além da revisão dos requisitos adicionados anteriormente. | [Caio César](https://github.com/oCaioOliveira)| [Victor Leão](https://github.com/victorleaoo)   |

## Introdução & Objetivo

A primeira, e talvez uma das mais importantes, parte no desenvolvimento de um software é a elicitação e priorização dos requisitos. Esse artefato, então, tem como objetivo usar certas técnicas de elicitação para levantar requisitos importantes do projeto a ser construído pela equipe.

Como as metodologias escolhidas pela equipe são baseadas em abordagens ágeis, é importante mencionar que os requisitos não são imutáveis e estão sujeitos a alterações, tanto como adição e remoção, ao longo do desenvolvimento do software.

## Metodologia

Foram, a princípio, utilizadas duas técnicas de elicitação (introspecção e observação) para levantar os requisitos funcionais e não-funcionais do projeto.

## Introspecção

É uma técnica em que o desenvolvedor se posiciona no papel do cliente/usuário do projeto e elicita os requisitos pensando nos seus desejos e fluxos de usos.

Participante da técnica:
- [Caio César](https://github.com/oCaioOliveira)

### Requisitos Funcionais

|Numeração |                                          Descrição                                      |
| -------- |  ------------------------------------------------------------------------------------   |
| RFI01    |                          Cadastrar conta de administrador.                              |
| RFI02    |                 Recuperar a senha de administrador pelo e-mail cadastrado.              |
| RFI03    |                         Cadastrar dados do administrador.                               |
| RFI04    |                         Visualizar o cardápio digital.                                  |
| RFI05    |                 Visualizar a descrição de um item no cardápio digital.                  |
| RFI06    |                Cadastrar níveis diferentes para os administradores do sistema.          |
| RFI07    |                       Buscar no cardápio digital itens por nome.                        |
| RFI08    |                  Filtrar itens por preço ou ordem alfabética.                           |
| RFI09    |         Visualizar o título, descrição, preço e imagem de cada item no cardápio digital.|
| RFI10    |         O cardápio deve ser dividido por áreas com itens de mesma categoria.            |
| RFI11    |Encontrar a localização, contato para suporte e horário de funcionamento como atalhos dentro do sistema.|
| RFI12    |                  Gerenciar o controle de mesas no estabelecimento como administrador.   |
  

### Requisitos Não Funcionais

|Numeração  |                                          Descrição                                       |
| --------  |  ------------------------------------------------------------------------------------    |
| RFNI01    | O Back-end do sistema deve ser desenvolvido em Python, utilizando o framework Django.    |
| RFNI02    |O Front-end do sistema deve ser desenvolvido em JavaScript, utilizando a biblioteca React.|
| RFNI03    |   O sistema deve ser responsivo para funcionar bem tanto em ambiente WEB quanto MOBILE.  |


## Observação

A técnica de observação consiste em, como o próprio nome já diz, observar um usuário em seu fluxo de uso e obter os requisitos a partir dessa prática. Essa técnica é muito útil para conseguir conhecimentos tácitos, isto é, aqueles que são "óbvios" para o usuário, mas que não foram explicitados.

Para o projeto, a observação foi feita em cima da utilização do software [Life Box](https://www.vucafood.com.br/lifeboxburger/aguas-claras/cardapio-digital), inspiração para o projeto do grupo, por parte de um terceiro participante não pertecente ao grupo.

Participante da técnica:
- [Victor Leão](https://github.com/victorleaoo)

### Requisitos Funcionais

|Numeração |Descrição|
| -------- |---------|
| RFOB01   | O cliente deve ser capaz de visualizar o cardápio digital. |
| RFOB02   | O cliente deve ser capaz de abrir a página específica de cada elemento do cardápio. |
| RFOB03   | O cliente deve ser capaz de visualizar as opções extras de ingredientes e seu valor para cada elemento do cardápio. |
| RFOB04   | O cliente deve ser capaz de realizar cadastro. |
| RFOB05   | O cliente deve ser capaz de realizar login. |
| RFOB06   | O cliente deve ser capaz de sair da sua conta. |
| RFOB07   | O cliente deve ser capaz de informar quantas pessoas estão esperando por uma vaga no restaurante. |
| RFOB08   | O cliente deve ser capaz de entrar na fila de espera do restaurante. |
| RFOB09   | O cliente deve ser capaz de ver a página 'sobre' do restaurante, com informações como telefone, endereço, gerente, entre outras, expostas. |
| RFOB10   | O cliente deve ser capaz de ver seus pedidos já realizados. |
| RFOB11   | O cliente deve ser capaz de adicionar métodos de pagamentos (cartões de crédito). |
| RFOB12   | O cliente deve ser capaz de alterar suas informações cadastradas (nome e e-mail). |

### Requisitos Não Funcionais

| Numeração | Descrição |
| --------  | --------- |
| RFNOB01   | O sistema deve ser responsivo para dispositivos móveis e desktop. |

## Referências

SERRANO, Milene. **Requisitos - Técnicas Elicitação**, 2022. Material apresentado na Disciplina de Arquitetura e Desenho de Software do curso de engenharia de software da UnB, FGA.