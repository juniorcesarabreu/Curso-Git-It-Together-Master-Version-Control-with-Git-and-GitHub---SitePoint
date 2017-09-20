Unindo (merge) branch featureC dentro de master com um merge no fast forward
===========================================

```sh
$ git status
$ git add .
$ git commit -m "Changed footer text color and font size"
$ git checkout master
$ git merge --no-ff featureC
# Merge made by the 'recursive' strategy.
$ git log --pretty=oneline
# a7cc26daf7520b3ffbdb1ec792812fd677c34bca (HEAD -> master) no -ff Merge branch 'featureC'
# c96e4cd2ea5bdccee4babf605c7f2118e696e43e (featureC) Changed footer text color and font size
# d57e28c235267558963d8fa9c354d7862cd64457 Changed text inside footer

```
