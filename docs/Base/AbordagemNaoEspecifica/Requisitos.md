# Requisitos

## Histórico de versões

|    Data    | Versão |      Descrição       |                   Autor(a)                    |                   Revisor(a)                    |
| ---------- | ------ | -------------------- | --------------------------------------------- | ----------------------------------------------- |
| 13/11/2022 |  0.1   | Criação do documento | [Caio César](https://github.com/oCaioOliveira)| [Victor Leão](https://github.com/victorleaoo)   |
| 13/11/2022 |  0.2   | Adição dos requisitos funcionais e regras de negócio por introspecção | [Caio César](https://github.com/oCaioOliveira)| [Victor Leão](https://github.com/victorleaoo)   |

### Quadro de Prioridade

|    Nível   |                    Significado                    |      
|  --------  |   --------------------------------------------    | 
|     1      | Obrigatoriamente deve estar na entrega do projeto |  
|     2      |     Tem relevância para a entrega do projeto      | 
|     3      |     Seria um extra para a entrega do projeto      |  

## Requisitos elicitados por introspecção 

### Requisitos Funcionais

Numeração |                                          Descrição                                      | Nível de prioridade |
 -------- |  ------------------------------------------------------------------------------------   |   ----------------  |
 RF01     |                          Cadastrar conta de administrador.                              |          1          |
 RF02     |                 Recuperar a senha de administrador pelo e-mail cadastrado.              |          1          |
 RF03     |                         Cadastrar dados do administrador.                               |          1          |
 RF04     |                         Visualizar o cardápio digital.                                  |          1          |
 RF05     |                 Visualizar a descrição de um item no cardápio digital.                  |          2          |
 RF06     |                 Visualizar a descrição de um item no cardápio digital.                  |          2          |
          
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
