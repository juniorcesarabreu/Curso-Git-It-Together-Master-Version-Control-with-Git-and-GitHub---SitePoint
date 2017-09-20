Unindo (merge) branch featureC dentro de master com um merge fast forward
===========================================

```sh
$ git branch -a
$ git checkout featureC
$ git add index.html
$ git commit -m "Changed text inside footer"
$ git checkout master
$ git merge featureC # junta o branch featureC ao atual (master), como master não tem nenhum commit que não tenha no branch featureC, será aplicado o fast forward, que é simpesmente apontar o HEAD para este branch
Fast-forward
$ git log --pretty=oneline
# d57e28c235267558963d8fa9c354d7862cd64457 (HEAD -> master, featureC) Changed text inside footer
```
