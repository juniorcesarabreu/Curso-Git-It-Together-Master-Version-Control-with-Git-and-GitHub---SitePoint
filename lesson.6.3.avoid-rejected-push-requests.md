Evitando rejeição de requisições push
=====================================

Se seu ambiente de trabalho não tiver o último commit remoto, haverá uma rejeição do seu push. Para corrigir será necessário utilizar o comando pull e depois fazer o push.

```sh
# Foi feito um push no repo remoto por outro usuário, e você não tem ainda esse commit
$ git status
$ git add .
$ git commit -m "Change the color of brand class"
$ git push origin master # Rejeitado, updates forma rejeitados porque o remoto contém trabalho que você não tem localmente
$ git pull origin master # Agora você tem o trabalho remoto, mas não perdeu seu trabalho local
$ git log --pretty=oneline
$ git push origin master # Agora você pode enviar seus commit para o remoto
```
