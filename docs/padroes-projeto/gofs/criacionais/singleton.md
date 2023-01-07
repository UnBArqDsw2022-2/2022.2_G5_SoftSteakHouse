# Singleton

## 1. Introdução
*Singleton* é um padrão que especifica como implementar classes que terão, como o próprio nome sugere, no máximo uma instância. Logo, ao serem utilizadas, esse único objeto não 
será sobrescrito, mantendo as informações das chamadas anteriores.

### 2. Aplicação

Para o acompanhamento da aplicação, é fundamental conseguirmos rastrear as informações (que cliente pediu o quê, para quem etc) através de uma tabela de Log. Entretanto, não há necesidade
de realocar esse objeto a cada novo registro, razão pela qual o Singleton será utilizado.

````
class Logger:

    _instance = None

    def __init__(self):
        "Constructor"

    @classmethod
    def getInstance(cls):
        if cls._instance is None:
            cls._instance = Logger()
        return cls._instance
````
Observe acima como um atributo estático armazena a instância única da classe. Quando essa instância for necessária, deve-se chamar o método público e estático getInstance().
## Histórico de versões
| Data       | Versão |      Descrição       | Autor(a)                                      | Revisor(a) |
|------------| ------ | -------------------- |-----------------------------------------------|------------|
| 04/01/2023 | 1.0    | Criação do documento | [Nícolas Mantzos](https://github.com/ngm1450) | -          |

