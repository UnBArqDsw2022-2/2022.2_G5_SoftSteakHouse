# GoF Comportamental - Estado

## Introdução

O padrão de projeto State permite que para situações diferentes de um mesmo objeto, ele exerça funções ou ações distintas.

Ele faz parte da categoria de GoFs Comportamentais, que, como pode ser conferido no artefato de [GoFs](https://unbarqdsw2022-2.github.io/2022.2_G5_SoftSteakHouse/#/padroes-projeto/iniciativas_extras/gofs), são voltados para alterações no nível de comportamento dos objetos, auxiliando, por exemplo, usar vários algoritmos diferentes, cada um apropriado para um determinado contexto.

## Metodologia

Esse padrão de projeto se basea no conceito de máquinas de estados, onde são definidos cada estado e seus possíveis comportamentos. Um objeto executará diferentes ações a depender de seu estado, podendo finalizar o fluxo antes de passar por todos seus passos.

Apesar de não implementado no projeto, pode vir a ser de grande ajuda visto que para um pedido ser criado, o cliente pode passar por diversos passos que podem ou não ser obrigatórios.

## Aplicação (Exemplo) no projeto

Assim, como explicado, os estados devem ser definidos juntos com suas implementações em classes destintas. Esse processo visa chamar ou não um método dependendo de parâmetros.

Dessa forma, no projeto Soft StakeHouse, o State poderia ser usado no pedido de um prato em um restaurante. Nesses cenários, temos várias váriaveis que podem fazer ou não necessário a execução de ações, como, por exemplo:
- Agendamento de mesa para caso do restaurante estiver com número elevado de clientes;
- Cadastro de formas de pagamento, caso não tenha nenhum cadastrado;
- Entrega do pedido, caso não vá comer presencialmente ou buscar sua comida;

## Código (exemplo)

```
class FavoritePaymentMethod is
    field state: string
    // ...
    method SetPaymentMethod() is
        switch (state)
            "has-node":
                createPaymentMethods();
                state = "not-chosed";
                break
            "not-chosed":
                setFavoritePaymentMathod();
                state = "chosed";
                break
            "chosed":
                // Não fazer nada.
                break
```

## Histórico de Versões

|    Data    | Versão |            Descrição           |       Autor     |    Revisor    |
|  --------  |  ----  |            ----------          | --------------- |    -------    |
| 05/01/2023 |  1.0.0 |  Criação do artefato | [Marcos Felipe](https://github.com/marofelipe) | [Victor Leão](https://github.com/victorleaoo) |

## Referências

REFACTORING GURU. State. Disponível em: https://refactoring.guru/pt-br/design-patterns/state. Acesso em: 05 jan. 2023.
