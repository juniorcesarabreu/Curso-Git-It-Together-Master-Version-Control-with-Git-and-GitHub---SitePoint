Desfazendo uma mudança comitada (commited)
=========================================

Para desfazer um commit e retornar ao commit anterior ao erro, use:

```sh
git reset --soft HEAD~1
```

A opção --soft deleta o commit mas não altera os arquivo, ou seja, ele fica no estado staged (preparado para commit).

HEAD~1 refere-se ao último commit antes do nosso erro
