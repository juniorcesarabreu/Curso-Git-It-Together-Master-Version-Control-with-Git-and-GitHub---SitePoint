Desfazendo uma mudança de estado preparado (staged)
============================================

Para desfazer uma mudança de um arquivo que foi colocado na area de staging com o comando add, use o comando reset. Isto removerá os arquivos da area de staging. Mas os arquivos ainda continuarão modificados e precisam ser editados manualmente.

```sh
 git reset HEAD index.html
```
