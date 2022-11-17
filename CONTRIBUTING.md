# Contributing


## Introdução

Este guia tem por objetivo definir as regras para criação de *Branches*, *Pull Requests* e *Commits* no projeto PO UI.
Para seguir o guia é fundamental o conhecimento da [ferramenta Git](https://git-scm.com/book/en/v2).

## Regras para criação da *Branch*

Antes de criar uma nova *branch* deve-se assegurar de estar na *branch main* do projeto.
Caso já esteja na *main* rode o comando:

```
git pull
```

Se não retornar nenhum erro ela estará atualizada e é hora de criar a *branch*. Para isso rode o comando:

```
git checkout -b <COMPONENTE>/<ISSUE>
```

Onde o `<COMPONENTE>` deve conter o nome do componente e não o projeto onde ele se encontra. E a `<ISSUE>` é o número da ocorrência a qual se refere a alteração.
Exemplos:

Caso a ISSUE seja gerada no GitHub:
```
git checkout -b po-button/235
```

Caso não exista uma ISSUE definida, crie a *branch* com o nome do desenvolvedor ou o nome do time e não esqueça de detalhar o que está sendo sugerido na descrição da *Pull Request*. Para isso rode o comando:

```
git checkout -b <COMPONENT>/<DEV|TEAM>
```

Exemplo:

```
git checkout -b po-button/fulano
```

## As políticas para criação de *Commits*, *Issue* e *Pull Request* se encontram nos seguintes links

- [Commits](docs/PoliticasDeTrabalho/PoliticaDeCommit.md)
- [Issue](docs/PoliticasDeTrabalho/PoliticaDeIssue.md)
- [Pull Request](docs/PoliticasDeTrabalho/PoliticasDePullRequest.md)



### Issue Checklist

Deve-se ir atualizando o status de cada issue no ZenHub.

