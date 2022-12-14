# Léxicos

## 1. Introdução

Léxicos são utilizados para descrever os símbolos de uma linguagem através de suas **noções** e **impactos**, isto é, respectivamente, suas definições/conceitos/denotações e suas implicações/resultados. No contexto de software, geralmente toma-se a aplicação que está sendo desenvolvida como referencial para a medição do impacto e elicitação das denotações.

Além das noções e impactos, léxicos também possuem um, e somente um, tipo associado. Os três que serão utilizadaos podem ser visualizados na tabela 1 abaixo.

| Tipo   |  Noção                                                             |  Impacto                                                                                | Sinônimos            |
|--------|--------------------------------------------------------------------|-----------------------------------------------------------------------------------------|----------------------|
| Verbo  | Quem realiza, quando acontece e quais procedimentos são envolvidos | Quais os reflexos da ação                                                               | Sinônimos do símbolo |
| Objeto | Definir o objeto e outros objetos com os quais se relaciona        | Ações que podem ser aplicadas ao objeto                                                 | Sinônimos do símbolo |
| Estado | O que significa e quais ações levaram a esse estado                | Identificar outros estados e ações que podem ocorrer a partir do estado que se descreve | Sinônimos do símbolo |

_Tabela 1: Modelo para os léxicos (SERRANO, Requisitos - Aula 10)_

Não obstante, também possuem um sinônimo - um objeto equivalente que está associado a mesma noção.

Essas quatro características são agregadas nos léxicos agrupados por tipo das tabelas abaixo.

## 2. Léxicos

### 2.1 Verbos

#### LV01 - Ver cardápio

| Noção                                                                                            | Impacto                                                                                                 | Sinônimos                            |
|--------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------|--------------------------------------|
| Ação realizada pelo cliente a fim de visualizar os produtos e pratos disponíveis no restaurante. | O cliente pode ver quais são os produtos oferecidos pelo restaurante, seus preços e realizar um pedido. | Olhar os pratos, acessar o cardápio. |

#### LV02 - Realizar pedido

| Noção                                                                                                                              | Impacto                                                                                                                                         | Sinônimos                  |
|------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------|
| Ação realizada pelo cliente na qual ele seleciona um item do cardápio e solicita a um funcionário que ele seja trazido a sua mesa. | - O valor da soma dos itens selecionados é adiciona à conta do cliente; <br> - Depois de prontos, os pedidos são levados até a mesa do cliente. | Fazer pedido, pedir prato. |

#### LV03 - Cancelar pedido

| Noção                                                                                                               | Impacto                                                                                                                        | Sinônimos                        |
|---------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------|----------------------------------|
| Ação realizada pelo cliente na qual ele consulta alguns dos pedidos ainda não enviados para a cozinha e os cancela. | - O valor da soma dos itens cancelados é subtraída da conta do cliente; <br> - Os pedidos não serão levados à mesa do cliente. | Retirar pedido, cancelar pedido. |

#### LV04 - Finalizar a conta

| Noção                                                                             | Impacto                                                                                                                     | Sinônimos                      |
|-----------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------|--------------------------------|
| Ação realizada pelo cliente na qual ele consulta a lista de pedidos e a finaliza. | - Um valor final, gerado a partir da soma dos pedidos entregues, será gerado; <br> - A conta aberta pelo cliente é fechada. | Pedir a conta, fechar a conta. |


### 2.2 Objetos

#### LO01 - Cliente

| Noção                                                                                                       | Impacto                                                                                                                                                                                        | Sinônimos |
|-------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------|
| Indivíduo que se utiliza do sistema a fim de fazer e cancelar pedidos, entrar na fila, consultar preços etc | - O cliente pode logar no sistema; <br> - O cliente pode ver o cardápio dos restaurantes cadastrados; <br> - O cliente pode fazer e cancelar um pedido; <br> O cliente pode contatar o suporte; | Usuário.  |

#### LO02 - Funcionário

| Noção                                                            | Impacto                                                                                                                                                     | Sinônimos                    |
|------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------|
| Usuário que recepciona e/ou responde às solicitações do cliente. | - Um funcionário pode ver a situação dos pedidos (pendente, cancelado ou entregue) e avaliar as requisições dos clientes e mesas (esgotado, disponível, demora...); | Garçom, balconista, gerente. |

### 2.3 Estados

#### LE01 - Status Pedido

| Noção                                             | Impacto                                                                                                                                                     | Sinônimos                    |
|---------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------|
| Métrica que avalia a atual situação de um pedido. | - Um funcionário pode ver a situação dos pedidos (pendente, cancelado ou entregue) e avaliar as requisições dos clientes (esgotado, disponível, demora...); | Garçom, balconista, gerente. |

## Histórico de Versões

| Versão | Data       | Descrição            | Autor                    | Revisor |
| ------ |------------|----------------------|--------------------------|---------|
| 1.0    | 15/11/2022 | Criação do documento | [Nícolas Georgeos Mantzos](https://github.com/ngm1450) | [Victor Leão](https://github.com/victorleaoo) |

## Referências Bibliográficas

SERRANO, Maurício; SERRANO, Milene. Requisitos - Aula 10. 1º/2019. 35 slides. Material apresentado para a disciplina de Requisitos de Software no curso de Engenharia de Software da UnB, FGA.
