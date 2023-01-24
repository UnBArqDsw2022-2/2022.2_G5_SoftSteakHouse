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
* Corpo da resposta: Uma lista com todos os itens cadastrados no sistema, sendo que cada item é composto de titulo (string obrigatória e única), descricao (string obrigatória), preco (float obrigatório), classificacao (string opcional e única) e link da imagem (string obrigatória).
* Exemplo de entrada: N/A
* Exemplo de resposta:

```
[
    {
        "titulo": "Onion Rings",
        "descricao": "Anéis de cebolas empanadas e fritas",
        "preco": "28.00",
        "classificacao": "ENTRADA",
        "link_imagem": "https://softsteakhouse-images.s3.sa-east-1.amazonaws.com/onion-rings.jpg"
    },
    {
        "titulo": "Macarrão com queijo",
        "descricao": "Prato de macarrão do tipo Spaghetti com queijo mussarela",
        "preco": "38.00",
        "classificacao": "PRATOPRINCIPAL",
        "link_imagem": "https://softsteakhouse-images.s3.sa-east-1.amazonaws.com/spaghetti-queijo.jpg"
    },
    {
        "titulo": "Coxinha de Frango",
        "descricao": "Porção de 10 coxinhas de frango fritas",
        "preco": "17.50",
        "classificacao": "ENTRADA",
        "link_imagem": "https://softsteakhouse-images.s3.sa-east-1.amazonaws.com/coxinha.jpg"
    }
]
```
 
#### POST
 
* Descrição: Irá cadastrar um item no sistema.
* Código de retorno sucesso: 201 Created
* Código de retorno falha: 500 Internal Server Error (depende do erro)
* Entrada: Item composto de titulo (string obrigatória e única), descricao (string obrigatória), preco (float obrigatório), classificacao (string opcional e única) e link da imagem (string obrigatória).
* Corpo da resposta: Uma mensagem informando que o item foi cadastrado com sucesso.
* Exemplo de entrada: 

```
{
    "titulo": "Coxinha de Frango",
    "descricao": "Porção de 10 coxinhas de frango fritas",
    "preco": "17.50",
    "classificacao": "ENTRADA",
    "link_imagem": "https://softsteakhouse-images.s3.sa-east-1.amazonaws.com/coxinha.jpg"
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
* Entrada: Item composto de titulo (string obrigatória e única), descricao (string obrigatória), preco (float obrigatório), classificacao (string opcional e única) e link da imagem (string obrigatória).
* Corpo da resposta: Uma mensagem opcional informando que o item foi editado com sucesso.
* Exemplo de entrada:

```
{
    "titulo": "Coxinha de Frango",
    "descricao": "Porção de 10 coxinhas de frango fritas",
    "preco": "17.50",
    "classificacao": "ENTRADA",
    "link_imagem": "https://softsteakhouse-images.s3.sa-east-1.amazonaws.com/coxinha.jpg"
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
* Entrada: Item composto de titulo (string obrigatória e única), descricao (string obrigatória), preco (float obrigatório), classificacao (string opcional e única) e link da imagem (string obrigatória).
* Corpo da resposta: Uma mensagem informando que o item foi deletado com sucesso.
* Exemplo de entrada:

```
{
    "titulo": "Coxinha de Frango",
    "descricao": "Porção de 10 coxinhas de frango fritas",
    "preco": "17.50",
    "classificacao": "ENTRADA",
    "link_imagem": "https://softsteakhouse-images.s3.sa-east-1.amazonaws.com/coxinha.jpg"
}
```

* Exemplo de resposta:

```
Item deletado com sucesso.
```

### /adicionais

#### GET

* Descrição: Irá retornar uma lista com todos os adicionais cadastrados no sistema.
* Código de retorno sucesso: 200 OK 
* Código de retorno falha: 500 Internal Server Error (depende do erro)
* Entrada: N/A
* Corpo da resposta: Uma lista com todos os adicionais cadastrados no sistema, sendo que cada adicional é composto de nome (string obrigatória e única) e preco (float obrigatório).
* Exemplo de entrada: N/A
* Exemplo de resposta:

```
[
    {
        "nome": "Cheddar e Bacon",
        "preco": "8.99"
    },
    {
        "nome": "Coca Lata",
        "preco": "8.00"
    },
    {
        "nome": "Guaraná Lata",
        "preco": "8.00"
    }
]
```
 
#### POST
 
* Descrição: Irá cadastrar um adicional no sistema.
* Código de retorno sucesso: 200 OK 
* Código de retorno falha: 500 Internal Server Error (depende do erro)
* Entrada: Um adicional composto de nome (string obrigatória e única) e preco (float obrigatório).
* Corpo da resposta: N/A
* Exemplo de entrada:

```
{
    "nome": "Cheddar e Bacon",
    "preco": "8.99"
}
```

* Exemplo de resposta:

```
Adicional cadastrado com sucesso.
```

#### PUT
 
* Descrição: Irá editar um adicional no sistema.
* Código de retorno sucesso: 200 OK 
* Código de retorno falha: 500 Internal Server Error (depende do erro)
* Entrada: Um adicional composto de nome (string obrigatória e única) e preco (float obrigatório).
* Corpo da resposta: N/A
* Exemplo de entrada:

```
{
    "nome": "Cheddar e Bacon",
    "preco": "8.99"
}
```

* Exemplo de resposta:

```
Adicional editado com sucesso.
```

#### DELETE
 
* Descrição: Irá deletar um adicional no sistema.
* Código de retorno sucesso: 200 OK 
* Código de retorno falha: 500 Internal Server Error (depende do erro)
* Entrada: Um adicional composto de nome (string obrigatória e única) e preco (float obrigatório).
* Corpo da resposta: N/A
* Exemplo de entrada:

```
{
    "nome": "Cheddar e Bacon",
    "preco": "8.99"
}
```

* Exemplo de resposta:

```
Adicional deletado com sucesso.
```

### /admins

Os administradores utilizarão o sistema definido pelo próprio Django, ou seja, a parte de login e cadastro será direto pela API, o framework libera um sistema de autentificação já construído dentro das suas funcionalidades.

### /mesas

#### GET

* Descrição: Irá retornar uma lista com todos as mesas cadastradas no sistema.
* Código de retorno sucesso: 200 OK 
* Código de retorno falha: 500 Internal Server Error (depende do erro)
* Entrada: N/A
* Corpo da resposta: Uma lista com todas as mesas cadastradas no sistema, sendo que cada mesa é composto de id, nomeTipo (string obrigatória), qtdCadeiras (inteiro positivo obrigatório) e qtdMesas (inteiro positivo obrigatório).
* Exemplo de entrada: N/A
* Exemplo de resposta:

```
[
    {
        "id": "1",
        "nomeTipo": "Mesa #2",
        "qtdCadeiras": "2",
        "qtdMesas": "6"
    },
    {
        "id": "2",
        "nomeTipo": "Mesa #4",
        "qtdCadeiras": "4",
        "qtdMesas": "3"
    }
]
```
 
#### POST
 
* Descrição: Irá cadastrar uma mesa no sistema.
* Código de retorno sucesso: 200 OK 
* Código de retorno falha: 500 Internal Server Error (depende do erro)
* Entrada: Uma mesa composta de auto-incrementável no banco de dados, nomeTipo (string obrigatória), qtdCadeiras (inteiro positivo obrigatório) e qtdMesas (inteiro positivo obrigatório).
* Corpo da resposta: N/A
* Exemplo de entrada:

```
{
    {
        "nomeTipo": "Mesa #2",
        "qtdCadeiras": "2",
        "qtdMesas": "6"
    }
}
```

* Exemplo de resposta:

```
Mesa cadastrada com sucesso.
```

#### PUT
 
* Descrição: Irá editar uma mesa no sistema.
* Código de retorno sucesso: 200 OK 
* Código de retorno falha: 500 Internal Server Error (depende do erro)
* Entrada: Uma mesa composta de auto-incrementável no banco de dados, nomeTipo (string obrigatória), qtdCadeiras (inteiro positivo obrigatório) e qtdMesas (inteiro positivo obrigatório).
* Corpo da resposta: N/A
* Exemplo de entrada:

```
{
    {
        "nomeTipo": "Mesa #2",
        "qtdCadeiras": "2",
        "qtdMesas": "3"
    }
}
```

* Exemplo de resposta:

```
Mesa editada com sucesso.
```

#### DELETE
 
* Descrição: Irá deletar uma mesa no sistema.
* Código de retorno sucesso: 200 OK 
* Código de retorno falha: 500 Internal Server Error (depende do erro)
* Entrada: Uma mesa composta de auto-incrementável no banco de dados, nomeTipo (string obrigatória), qtdCadeiras (inteiro positivo obrigatório) e qtdMesas (inteiro positivo obrigatório).
* Corpo da resposta: N/A
* Exemplo de entrada:

```
{
    {
        "nomeTipo": "Mesa #2",
        "qtdCadeiras": "2",
        "qtdMesas": "3"
    }
}
```

* Exemplo de resposta:

```
Mesa deletada com sucesso.
```

### Histórico de Versões

| Data  | Versão | Descrição | Autor | Revisor |
| --- | --- | --- | --- | --- |
| 11/12/2022 | 0.1 | Criação do documento | [Caio César](https://github.com/oCaioOliveira) | [Victor Leão](https://github.com/victorleaoo) |
| 11/12/2022 | 0.2 | Adição do endpoint /itens | [Caio César](https://github.com/oCaioOliveira) | [Victor Leão](https://github.com/victorleaoo) |
| 11/12/2022 | 0.3 | Adição do endpoint /admins | [Caio César](https://github.com/oCaioOliveira) | [Victor Leão](https://github.com/victorleaoo) |
| 11/12/2022 | 1.0 | Atualização de template | [Caio César](https://github.com/oCaioOliveira) | [Victor Leão](https://github.com/victorleaoo) |
| 23/01/2023 | 1.1 | Adição do endpoint /mesas | [Victor Leão](https://github.com/victorleaoo) | - |