Visualize seu Git log
========================================

Além de `git log` e `git log --pretty=oneline` há outras formas de visualizar a história dos commits.

Para exibir por autor:
```sh
git log --author=juniorcesarabreu
```

Para exibir em representação de árvore:
```sh
git log --graph --decorate -- oneline
```

Para limitar o número de commits na visualização, use `-n` seguido do número limite:
```sh
git log -n 1
```

Para exibir as alterações ocorrida nos arquivos em um commit, use show seguido pelo número de identificação do commit:
```sh
git show 3e49998b9ccd7d7d47a7e10b4810f4f5d5aeda1d
```

Para exibir as diferenças entre dois branches use `diff`:
```sh
git diff master featureA
```
