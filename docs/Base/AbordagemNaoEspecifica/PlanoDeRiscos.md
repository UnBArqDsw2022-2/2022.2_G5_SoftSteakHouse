## Histórico de Versões

|    Data    | Versão |            Descrição           |       Autor     |    Revisor    |
|  --------  |  ----  |            ----------          | --------------- |    -------    |
| 09/11/2022 |  1.0.0 |  Criação do plano de riscos    |   [Caio César](https://github.com/oCaioOliveira)    |       [Taynara](https://github.com/TaynaraCris)       |

## Introdução & Objetivo

O objetivo desse documento é informar detalhadamente os riscos que podem afetar o projeto. Além de categorizar e descrever os mesmos, tendo em vista que existem diversos riscos, afetando diretamente escopo, cronograma, custo e qualidade. Portanto, é preciso definir como serão mantidos os riscos, para identificar e propor ações contra.

## Metodologia

Para caracterização dos risco, foram usados os seguintes componentes:

- **Evento:** Descrição do que pode acontecer.
- **Probabilidade:** A frequência com que pode ocorrer.
- **Impacto:** O quão grave é o seu efeito, caso realmente ocorra.
- **Prevenção:** Como reduzir sua probabilidade.
- **Contenção:** Como reduzir seu impacto, caso realmente ocorra.

### Probabilidade

|    Nível   | Intervalo |            Peso           |       
|  --------  |  ----  |            ----------          | 
| Muito Baixa | 0 <= P <=20% |  1    |  
| Baixa | 20% < P <= 40% |  2   |  
| Moderada | 40% < P <= 60% |  3    |  
| Alta| 60% < P <= 80% |  4    |  
| Muito Alta | 80% < P <= 100% |  5    |  

### Impacto

|    Nível   | Intervalo |            Peso           |       
|  --------  |  ----  |            ----------          | 
| Muito Baixa | Irrelevante para o projeto |  1    |  
| Baixa | Pouca influência no desenvolvimento do projeto |  2   |  
| Moderada | Notável ao projeto, mas sem grandes consequências |  3    |  
| Alta| Dificulta o desenvolvimento do projeto, afetando a qualidade do produto |  4    |  
| Muito Alta | Impossibilita o desenvolvimento do projeto |  5    |  

## Diagrama de riscos do projeto

###  Risco Técnico

| **Tipo** | **Descrição** |
| --- | --- |
| Requisitos | Riscos gerados pela falta de mapeamento e elicitação de requisitos |
| Tecnologias | Riscos gerados pela tecnologia usada |
| Complexidade | Riscos gerados pela falta de conhecimento e pela forma na qual a equipe de desenvolvimento se adapta a tecnologia escolhida |
| Qualidade | Riscos decorrentes da qualidade do produto final |

### Risco de Gerenciamento

| **Tipo** | **Descrição** |
| --- | --- |
| Estimativa | Riscos que podem afetar o tempo de produção do projeto|
| Controle | Riscos relacionados ao controle de atividades |
| Planejamento | Riscos relacionados ao planejamento de confecção do projeto |
| Comunicação | Riscos relacionados às atividades e meio de comunicação, como ruídos ou falta de comunicação da equipe |

### Risco Organizacional

| **Tipo** | **Descrição** |
| --- | --- |
| Recursos | Riscos gerados pela falta de recursos humanos e/ou tecnológicos, como perda ou defeitos em equipamentos ou membros que abandonam o projeto (trancamento) |
| Dependências | Riscos que podem afetar a evolução do projeto impedindo com que membros contribuam|

## Identificação de Riscos

| # | Evento | Probabilidade | Impacto | Prevenção | Contenção |
| - | ------ | ------------- | ------- | --------- | --------- |
| 1 | Falta de comprometimento com o projeto | Média | Alto | Comunicação frequente e efetiva; Alocar membros baseado em seus interesses. | Comunicar com o membro; Engajar membro para o projeto.  |
| 2 | Distribuição de tarefas desbalanceada | Média | Alto | Participação nas sprints; Distribuir balanceadamente considerando a dificuldade das tarefas; Realizar planning poker; Comunicar sobre dificuldades; | Realocação das tarefas; Realizar Planning Poker; |
| 3 | Desistência de um integrante | Média | Alto | Manter a motivação através de comunicação frequente | Realocação das tarefas; Distribuir tarefas baseado nos conhecimentos dos integrantes |
| 4 | Alteração no escopo do projeto | Média | Médio | Elicitação e análise de requisitos efetiva desde o início do projeto; | Documentar bem os novos itens; Validar os novos requisitos; |
| 5 | Má interpretação dos requisitos | Média | Alto | Requisitos bem definidos na documentação; Realizar verificação dos requisitos; Comunicar com a equipe caso existam dúvidas; | Aprimorar documentação dos requisitos |
| 6 | Atraso nas entregas | Média | Alta | Comunicação frequente, especialmente durante as sprints | Realocar tarefas atrasadas; Aumentar prioridade; |
| 7 | Requisitos mal elicitados | Média | Alta | Realizar validação de requisitos efetivamente | Comunicar o grupo; Levantar requisitos |
| 8 | Defeitos na aplicação do projeto | Alta | Média | Realizar testes; Realizar code reviews antes de aceitar PRs sem analisar mudanças; | Alocar membros para o hot fix; |

## 6. Referências

"Gerenciamento dos riscos: O que é, objetivo e processos". Disponível em https://escritoriodeprojetos.com.br/gerenciamento-dos-riscos-do-projeto
