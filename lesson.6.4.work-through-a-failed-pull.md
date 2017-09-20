Trabalhando através de requisição pull falhada
=================================================

Quando ocorrer conflitos de informação em uma mesma parte do mesmo arquivo, Git selecionará estes conflitos e pedirá para resolvê-los manualmente em seu editor de códigos.

```sh
$ git add .
$ git commit -m "Change color to a mustard shade"
$ git push origin master # Rejeitado
$ git pull origin master # Conflito, corrija os conflitos e então commit o resultado
```

Exemplo de um conflito
```css
.brand {
<<<<<<< HEAD
    color: #fab11c !important;
=======
    color: #40e0d0 !important;
>>>>>>> 733d71ee7bcab9460a25d29cfc9d0587a37e2b3f
}
```

HEAD denota o commit em nosso próprio branch e abaixo está o commit remoto.

Você e sua equipe decidirão qual código deixar e excluirão o resto em seu editor. Após editar será necessário fazer um novo commit.

```sh
$ git status # Git avisa que há caminhos não unidos
$ git add .
$ git commit -m "Kept mustard color"
$ git push origin master
```

É boa prática geralmente, fazer um pull em qualquer trabalho antes de fazer um push para pegar a alterações mais recente do repo remoto.
