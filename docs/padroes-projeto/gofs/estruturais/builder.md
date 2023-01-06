# Builder

## 1. Introdução
*Builder* é um padrão de projeto primariamente utilizado para facilitar a instanciação de objetos com muitos atributos, muitos deles opcionais e que, caso não sejam informados,
devem ser inicializados com um valor default. Assim, a multiplicidade de métodos construtores que obrigaria o desenvolvedor a conhecer a ordem dos parâmetros é 
substituída por uma chamada "principal" seguida de "n" métodos set, um para cada atributo passado.


### 2. Exemplo - Ingrediente

Além do volume de atributos, o recorrente desconhecimento (ou irrelevância) de muitos deles no momento da instanciação também evoca o uso desse padrão de projeto. Na aplicação, por exempo, somente o nome e a descrição de um objeto do tipo
Ingrediente podem ser relevantes em um primeiro momento, ficando dados nutricionais como o nível de carboidrato ou proteína em segundo plano.

```
from abc import ABCMeta, abstractmethod

class IngredienteBuilder(metaclass=ABCMeta):

    @staticmethod
    @abstractmethod
    def setNome():
        "Set nome"

    @staticmethod
    @abstractmethod
    def setDescricao():
        "Set descricao"

    @staticmethod
    @abstractmethod
    def setCarboidrato():
        "Set carboidrato"

    @staticmethod
    @abstractmethod
    def setProteina():
        "Set carboidrato"
        
    @staticmethod
    @abstractmethod
    def setLipídeo():
        "Set lipideo"
    
    @staticmethod
    @abstractmethod
    def setLipídeo():
        "Set calorias"    

class ConcreteBuilder(IngredienteBuilder):

    def __init__(self):
        self.product = Product()

    def build_part_a(self):
        self.product.parts.append('a')
        return self

    def build_part_b(self):
        self.product.parts.append('b')
        return self

    def build_part_c(self):
        self.product.parts.append('c')
        return self

    def get_result(self):
        return self.product

class Product():
    "The Product"

    def __init__(self):
        self.parts = []

class Director:
    "The Director, building a complex representation."

    @staticmethod
    def construct():
        "Constructs and returns the final product"
        return Builder()\
            .build_part_a()\
            .build_part_b()\
            .build_part_c()\
            .get_result()

# The Client
PRODUCT = Director.construct()
print(PRODUCT.parts)
```

### 1.2 Dependências

Há uma dependência entre duas classes <i>X</i> e <i>Y</i> quando <i>X</i> declara um parâmetro ou variável local do tipo <i>Y</i> ou quando um método de <i>X</i> lança uma exceção do tipo <i>Y</i>. É considerada uma modalidade menos forte de
relacionamento do que heranças e associações e, no diagrama de classes, é representada como uma seta tracejada, de extremidade fechada e orientada de <i>X</i> para <i>Y</i>.

## 2. Metodologia

Após a definição das tecnologias que serão utilizadas no desenvolvimento, seus objetivos e sua arquitetura, houve um mapeamento das entidades fundamentais da aplicação e das classes necessárias à sua manipulação (<i>services, repositories, controllers, utils </i> etc). Por fim, foram estabelecidos os
tipos de relacionamento supracitados, consultando os membros do grupos e o backlog do produto para validação.

## 3. Diagrama
![Diagrama de classes](../../assets/novo_diagrama_classes_softstackhouse.jpeg)


## Histórico de versões
| Data       | Versão |      Descrição       | Autor(a)                                      | Revisor(a) |
|------------| ------ | -------------------- |-----------------------------------------------|------------|
| 01/12/2022 | 1.0    | Criação do documento | [Nícolas Mantzos](https://github.com/ngm1450) | [Victor Leão](https://github.com/victorleaoo) |
| 04/01/2023 | 1.1    | Modificação do Diagramada de Classes | [Hian Praxedes](https://github.com/HianPraxedes) | |


## Referências

GREEN, Daniel. Diagrama de Pacotes: Definição, Componentes e Exemplos. [S. l.], 23 jun. 2021. Disponível em: https://gitmind.com/pt/diagrama-de-pacotes.html. Acesso em: 30 nov. 2022.
