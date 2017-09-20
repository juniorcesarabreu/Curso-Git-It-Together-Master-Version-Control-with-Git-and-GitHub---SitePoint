Unindo Branches
========================================

Coamndos git
-----------------------------------------

* Merge básico
* UJunta um branch dentro de seu branch atual por exemplo fazer checkout dentro do master e executar o comando merge. Se o branch master tem divergências (i.e. mais commit tem tomado lugar), então juntar o branch dentro master criará um merge commit.
* Por exemplo: `git checkout master`

`git merge branchName`


`git merge`: Juntará branches independentes
`git merge branchName`: Junta o branch

O comando merge junta um branch dentro do branch atual (checkout)

Tipos de merges
-----------------------------------------------

* **Fast forward merges**

* Se o branch master não tem divergências (i.e. nenhum commit adicional ocorreu no branch master), então git apontará para o último commit no branch após o merge

* **No fast forward (--no-ff)**

* Um merge commit representa o merge

* `git merge --no-ff`: Em vez de apenas apontar para o último commit no branch, quando `git merge --no-ff` é passado então um commit do merge ocorre.


* **3 way merge**

* 2 commits são gerados para os dois branches e então eles são unidos e um outro commi é gerado.

* Isto acontece quando o desenvolvimento está ocorrendo em ambos branches simultaneamente e é comum quando muitas pessoas estão trabalhando no mesmo projeto.


Não precisamos indicar o método de merge a usar, pois isto é determinado por um algoritmo. Entretanto, uma exceção para isto é com o merge no fast forward.
