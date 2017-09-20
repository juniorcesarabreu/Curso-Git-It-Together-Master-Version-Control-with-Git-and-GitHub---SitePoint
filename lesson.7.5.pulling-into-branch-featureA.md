
```sh
$ git checkout featureA
$ git add index.html
$ git commit -m "Edited paragraph"
$ git pull origin featureA # Conflito, pois há alterações no repositório remoto ausentes no repositorio local, corrija os conflitos manualmente
$ git add index.html
$ git commit -m "Incorporated <p> changes"
$ git push origin featureA
```
