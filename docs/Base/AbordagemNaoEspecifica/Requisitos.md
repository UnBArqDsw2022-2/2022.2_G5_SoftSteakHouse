# Requisitos

## Histórico de versões

|    Data    | Versão |      Descrição       |                   Autor(a)                    |                   Revisor(a)                    |
| ---------- | ------ | -------------------- | --------------------------------------------- | ----------------------------------------------- |
| 13/11/2022 |  0.1   | Criação do documento | [Caio César](https://github.com/oCaioOliveira)| [Victor Leão](https://github.com/victorleaoo)   |
| 13/11/2022 |  0.2   | Adição dos requisitos funcionais e regras de negócio por introspecção | [Caio César](https://github.com/oCaioOliveira)| [Victor Leão](https://github.com/victorleaoo)   |
| 14/11/2022 |  0.3   | Adição de uma breve introdução acerca da introspecção,<br/> adição de um 'I' na frente de cada um dos requisitos elicitados por introspecção,<br/> Adição da técnica de observação | [Victor Leão](https://github.com/victorleaoo) | [Caio César](https://github.com/oCaioOliveira) |

## Introspecção

É uma técnica em que o desenvolvedor se posiciona no papel do cliente/usuário do projeto e elicita os requisitos pensando nos seus desejos e fluxos de usos. Como base para essa técnica, foram usados os [Rich Pictures](https://unbarqdsw2022-2.github.io/2022.2_G5_SoftSteakHouse/#/Base/AbordagemNaoEspecifica/RichPicture) feitos.

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
| RFI06    |                 Visualizar a descrição de um item no cardápio digital.                  |
          

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
| RFOB06   | O cliente deve ser capaz de deslogar. |
| RFOB07   | O cliente deve ser capaz de informar quantas pessoas estão esperando por uma vaga no restaurante. |
| RFOB08   | O cliente deve ser capaz de entrar na fila de espera do restaurante. |
| RFOB09   | O cliente deve ser capaz de ver a página 'sobre' do restaurante, com informações como telefone, endereço, gerente, entre outras, expostas. |
| RFOB10   | O cliente deve ser capaz de ver seus pedidos já realizados. |
| RFOB11   | O cliente deve ser capaz de adicionar métodos de pagamentos (cartões de crédito). |
| RFOB12   | O cliente deve ser capaz de alterar suas informações cadastradas (nome e e-mail). |

### Requisitos Não Funcionais

| Numeração | Descrição |
| --------  | --------- |
| RFNOB01   | O cardápio digital deve ser disposto separado por categorias de alimento. |
| RFNOB02   | Cada elemento do cardápio deve conter título, imagem, descrição e valor.  |

  ---------------------------- Apagar Abaixo ----------------------------      
### Regras de Negócio

#### RF01

- **Descrição:** Deve haver níveis diferentes para os administradores do sistema, ou seja, um nível para o gerenciamento de mesas apenas, e um nível superior para todas as 
funcionalidades do sistema e a capacidade de cadastrar novos itens no cardápio digital, editá-los ou apagá-los.
- **Prioridade:** 3

#### RF04

- **Descrição:** Deve ser possível visualizar o título, descrição, preço e imagem de cada item no cardápio digital.
- **Prioridade:** 1
<br>

- **Descrição:** Deve ser possível fazer uma busca no cardápio digital por nome ou filtrar por preço e ordem alfabética.
- **Prioridade:** 2
<br>

- **Descrição:** O cardápio deve ser dividido por áreas com itens de mesma categoria, como uma área para pizzas, fritas, hamburgueres, etc.
- **Prioridade:** 2