Adicionar commit e push para Git

Para incializar um repositório Git:
```sh
git init
```

Para sincronizar com o repositório remoto Git: Origin é o nome dado ao repositório remoto por padrão, e não tem nenhum significado especial.
```sh
git remote add origin https://github.com/juniorcesarabreu/Git-Course-Demo.git
git remote -v
```

Para checar o estado use o comando status:
```sh
git status
```

Para adicionar os arquivos para a staging area, use o comando add: O ponto indica para adicionar todos os arquivos.
```sh
git add .
```

Para comitar use commit: As mensagens do commit devem sempre fazer sentido, para facilitar quando tiver que rever o trabalho
```sh
git commit -m "initial commit, pushing theme over to github"
```

Para armazenar no repositório remoto no github, use push:
```sh
git push origin master
```
