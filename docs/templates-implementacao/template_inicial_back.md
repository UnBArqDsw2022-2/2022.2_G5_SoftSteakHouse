# Template Inicial para Implementação do Back-end

Esse template tem como objetivo principal determinar como deverão ser feitos os endpoints da API que servirá a equipe de Front-end, para esclarecer melhor a imagem do sistema para a equipe que o criará.

## Endpoints

Esta seção irá explicar sobre os endpoints iniciais que serão criados pela equipe, determinando as entradas e saídas das funcionalidades.

### /itens

#### GET

* Descrição: Irá retornar uma lista com todos os itens cadastrados no sistema.
* Código de retorno sucesso: 200 OK 
* Código de retorno falha: 500 Internal Server Error (depende do erro)
* Entrada: N/A
* Corpo da resposta: Uma lista com todos os itens cadastrados no sistema, sendo que cada item é composto de titulo (string obrigatória e única), descricao (string obrigatória) e preco (float obrigatório).
* Exemplo de entrada: N/A
* Exemplo de resposta:

```
[
    {
        "titulo": "Batata Frita",
        "descricao": "Batata colhida nos campos da Inglaterra e frita no óleo dos pastéis da semana passada.",
        "preco": 18.99
    },
    {
        "titulo": "Feijão com Arroz",
        "descricao": "Comida tradicional brasileira e especialidade do chefe Nobody Yes Door.",
        "preco": 45.99
    },
    {
        "titulo": "Macarrão da Roça",
        "descricao": "Macarrão que a avó do chefe mandou ontem.",
        "preco": 54.99
    }
 ]
 ```
 
#### POST
 
* Descrição: Irá cadastrar um item no sistema.
* Código de retorno sucesso: 201 Created
* Código de retorno falha: 500 Internal Server Error (depende do erro)
* Entrada: Item composto de titulo (string obrigatória e única), descricao (string obrigatória) e preco (float obrigatório).
* Corpo da resposta: Uma mensagem informando que o item foi cadastrado com sucesso.
* Exemplo de entrada: 

```
{
    "titulo": "Batata Frita",
    "descricao": "Batata colhida nos campos da Inglaterra e frita no óleo dos pastéis da semana passada.",
    "preco": 18.99
}
```

* Exemplo de resposta:

```
Item cadastrado com sucesso.
```

#### PUT
 
* Descrição: Irá editar um item já cadastrado no sistema.
* Código de retorno sucesso: 204 No Content
* Código de retorno falha: 500 Internal Server Error (depende do erro)
* Entrada: Item composto de titulo (string obrigatória e única), descricao (string obrigatória) e preco (float obrigatório).
* Corpo da resposta: Uma mensagem opcional informando que o item foi editado com sucesso.
* Exemplo de entrada:

```
{
    "titulo": "Batata Frita",
    "descricao": "Batata colhida nos campos da Inglaterra e frita no óleo dos pastéis da semana passada.",
    "preco": 18.99
}
```

* Exemplo de resposta:

```
Item editado com sucesso.
```

#### DELETE
 
* Descrição: Irá deletar um item já cadastrado no sistema.
* Código de retorno sucesso: 200 OK
* Código de retorno falha: 500 Internal Server Error (depende do erro)
* Entrada: Item composto de titulo (string obrigatória e única), descricao (string obrigatória) e preco (float obrigatório).
* Corpo da resposta: Uma mensagem informando que o item foi deletado com sucesso.
* Exemplo de entrada:

```
{
    "titulo": "Batata Frita",
    "descricao": "Batata colhida nos campos da Inglaterra e frita no óleo dos pastéis da semana passada.",
    "preco": 18.99
}
```

* Exemplo de resposta:

```
Item deletado com sucesso.
```

### Histórico de Versões

| Data  | Versão | Descrição | Autor | Revisor |
| --- | --- | --- | --- | --- |
| 11/12/2022 | 0.1 | Criação do documento | [Caio César](https://github.com/oCaioOliveira) | [Victor Leão](https://github.com/victorleaoo) |
| 11/12/2022 | 0.2 | Adição do endpoint /itens | [Caio César](https://github.com/oCaioOliveira) | [Victor Leão](https://github.com/victorleaoo) |
