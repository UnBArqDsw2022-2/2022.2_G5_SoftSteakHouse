# Linguagem de Modelagem Unificada (UML)


## 1. Introdução
No decorrer dos anos 80, o paradigma de orientação a objetos estava encorpando e vivendo seu auge, acompanhado pela consolidação do processo Waterfall de desenvolvimento. Esse, por sua vez, especificava uma longa fase de design na qual diagramas e modelos gráficos dos mais variados seriam criados e repassados para os desenvolvedores efetivamente começarem a escrita do código.

No final da década, entretanto, diversas notações gráficas começaram a surgir a fim de corresponder às expectativas do modelo e paradigma predominantes; boa parte delas inconvertíveis e incomunicáveis entre si, o que dificultava a troca de conhecimentos inter-corporativa entre as equipes. Foi quase no final do século, em 1995, que a primeira proposta de notação unificada, baseada nas notações mais populares e difundidas do período, foi apresentada. Apropriadamente, batizaram-na de <b>Linguagem de Modelagem Unificada (UML)</b>.

Após dois anos de críticas, revisões e aplicações, em 1997 a UML passou a ser gerenciada pela <i>Object Management Group (OMG) </i>, uma organização de padronização gerenciada pela indústria de software.

## 2. Martin Fowler e o fator <i>canivete</i>

Martin  Fowler, em sua obra classíca sobre UML, propôs três formas de uso, ou "perspectivas", da linguagem.

### UML como linguagem de programação ou "UML como fim"

Após a padronização pela OMG, vislumbrou-se durante um período a possibilidade de se gerar código automaticamente a partir dos modelos criados. A ideia era, portanto, adicionar
mais recursos à linguagem para facilitar o processo de conversão para o código final, removendo a fase de codificação prevista no modelo Waterfall e transformando o "meio" em "fim" de imediato. Essas adições acabaram tornando-a complexa e pesada. Atualmente, com toda sua evolução e padronização, a geração de código a partir dela não é tão difundida.


### UML como blueprint ou "UML como meio"

Aqui, a UML é vista como parte integrante de uma longa etapa de design na qual um conjunto de modelos descrevendo diversos aspectos do software seriam desenvolvidos, algo muito característico de processos de desenvolvimento Waterfall ou RUP. Tais modelos seriam, enfim, encaminhados aos desenvolvedores para a escrita do código. Ou seja, não há a pretensão de eliminação da etapa de codificação.

### UML como esboço

UML é utilizada para construir diagramas leves e informais de partes de um sistema a fim de facilitar a comunicação entre desenvolvedores, seja para discutir e analisar alternativas de design para a implementação de uma nova funcionalidade
(Engenharia Avante) ou investigar o funcionamento de uma funcionalidade já implementada (Engenharia Reversa)

## 3. UML hoje
<i>Software em funcionamento mais que documentação abrangente</i> é um dos emblemáticos dizeres do Manifesto Ágil - documento que
pauta boa parte dos métodos de desenvolvimento de software atuais (SCRUM, Kanban, XP...). Em boa parte deles, inexiste uma grande fase de design na qual o UML
seja protagonista. Ao invés disso, o design é visto como algo incremental que evolui a medida que o sistema vai nascendo, ao final de cada iteração. Nesse contexto, a perspectiva de esboço proposta por Fowler é 
a que mais se utiliza, preterindo-se a criação de diagramas pequenos, concisos e informais, muitas vezes em lousas ou folhas de papel, instrumentalizados em nome do entendimento de 
uma funcionalidade, ao invés de documentação parruda em prol da compreensão de todo o sistema.

## Histórico de versões
| Data       | Versão |      Descrição       | Autor(a)                                      | Revisor(a) |
|------------| ------ | -------------------- |-----------------------------------------------|------------|
| 02/12/2022 | 1.0    | Criação do documento | [Nícolas Mantzos](https://github.com/ngm1450) | [Victor Leão](https://github.com/victorleaoo) |


## Referências

GREEN, Daniel. Diagrama de Pacotes: Definição, Componentes e Exemplos. [S. l.], 23 jun. 2021. Disponível em: https://gitmind.com/pt/diagrama-de-pacotes.html. Acesso em: 30 nov. 2022.
