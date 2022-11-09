## Histórico de Versões


|    Data    | Versão |            Descrição           |       Autor     |    Revisor    |
|  --------  |  ----  |            ----------          | --------------- |    -------    |
| 09/11/2022 |  1.0.0 | Criação da política de commits |   Caio César    |       -       |
 
## Commit

Os commits devem seguir um padrão:

### Princípios:

#### Commits atômicos
Sempre dividir em pequenos e significativos commits, fazendo com que cada commit tenha apenas uma funcionalidade e que seja possível entender o que foi feito sem precisar analisar o código ou documento alterado.

#### Tipos:
```Para inserir um emoji, basta digitar: ":nome_do_emoji:". Exemplo: ":bulb:"```

[***Lista de emojis disponíveis em markdown***](https://gist.github.com/rxaviers/7360908)

- :rocket: quando alterar código do front-end ```:rocket:```
- :floppy_disk: quando alterar código do back-end ```:floppy_disk:```
- :pencil: quando alterar documentação ```:pencil:```

### Formato:
```
<tipo>(#número da issue): assunto
```

#### Assunto:
- Deve possuir no máximo 50 caracteres
- Devem estar em letras minúsculas

*Exemplo de commit:*
```
git commit -m ":pencil:(#02): corrigir erros de digitação"
```
