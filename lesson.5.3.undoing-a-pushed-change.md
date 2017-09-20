Desfazendo uma mudança pushed
=====================================

Para desfazer um commit que foi enviado para o repositório remoto com push, use revert, Isso reverterá todas as alterações para o estado do útlimo commit, inclusive descartará todas as alterações nos arquivos. E necessário um push após para atualizar no repositório remoto.

```sh
git revert HEAD
git push origin master
```
