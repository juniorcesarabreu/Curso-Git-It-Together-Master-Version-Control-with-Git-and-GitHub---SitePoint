SSH para Github
==================================

SSH = Secure Shell

Permite conectar ao Github sem precisar digitar a senha, através de uso de criptografia.

Usuários Mac e Linux, podem usar o próprio terminal, enaquanto usuários Windows precisam instalar Putty, que é cliente SSH gratuito para Windows.

Digite o código abaixo para gerar um par de chaves pública privada, exibir o ID da chave gerada e adicionar a chave ao agente SSH

```sh
ssh-keygen -t rsa -C youremail@github.com

eval "$(ssh-agent -s)"

ssh-add ~/.cch/id_rsa
```

Agora precisamos adicionar a chave pública ao Github. Copie tudo do arquivo ~/.ssh/id_rsa.pub. Vá em Configurações no Github e em SSH Key. Cole a chave e dê um título.

Teste a conexão, digitando exatamente desta forma, não use seu email.

```sh
sst -T git@github.com
```
