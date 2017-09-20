Organizando os branches
=======================================

Listar todos os branches
-------------------------------------

```sh
git branch -a
```

O asterisco * denota o branch atual que estamos trabalhando

Adicionar um novo branch
-------------------------------------

```sh
git branch featureA
```

Para trocar de branch (checkout)
----------------------------------

```sh
git checkout featureA
```

Criando um novo branch e fazendo checkout dele na mesma linha de comando
-----------------------------------

```sh
git checkout -b featureC
```

Para renomear um branch
-----------------------------

git branch -m <Nome atual> <Novo nome>

```sh
git branch -m Extra BranchToDelete
```

Deletar um branch
---------------------------------

Para deletar um branch, ele não pode ser o atual (checked), é necessário fazer checkout, trocar para outro branch.

```sh
git checkout master
git branch -d BranchToDelete
```
