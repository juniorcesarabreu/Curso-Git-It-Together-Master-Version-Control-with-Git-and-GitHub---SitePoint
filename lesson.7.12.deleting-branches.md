Deletando branches
=========================================

```sh
$ git branch -a
#   featureA
#   featureB
#   featureC
# * master
#   remotes/origin/featureA
#   remotes/origin/featureB
#   remotes/origin/master

$ git branch -d featureC # Deleta o branch local
# Deleted branch featureC (was c96e4cd).

$ git branch -d featureB
# Deleted branch featureB (was e25dd32).
$ git branch -a
#   featureA
# * master
#   remotes/origin/featureA
#   remotes/origin/featureB
#   remotes/origin/master

$ git push origin --delete featureB # Deleta o branch remoto
# To https://github.com/juniorcesarabreu/Git-Course-Demo.git
#  - [deleted]         featureB

$ git branch -a
#   featureA
# * master
#   remotes/origin/featureA
#   remotes/origin/master

```
