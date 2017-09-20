Branches
================================

* Um branch git reprtesenta uma linha independente de desenvolvimento.
* Cada branch é associado com suas próprias alterações.
* `Master` é o branch principal
* `HEAD` refere-se a extremidado do branch em que você está sobre (o commit mais recente neste branch)

Suponha que você decida adicionar uma nova funcionalidade em seu projeto, e você faça mudanças a seus arquivos enquanto ainda no branch master como temos feito até agora. Então, posteriormente, você deicide remover esta funcionalidade. Ou você teria que mudar todos os seus arquivos para representar o estado anterior antes de você adicionar a funcionalidade ou você teria que voltar atrás até o último commit antes de voc~e começar a adicionar o código de sua funcionalidade no branch master. De qualquer forma, ambas são soluções confusas e consumidoras de tempo. A Resposta para evitar essa situação é branch.

Branch oferece um ambiente separado onde você pode experimentar, por exemplo, adicionando ou deletando funcionalidades usando o mesmo processo git. Ao trabalhar em um branch git o código base no branch master permanece intocado. E isto é bom porque você vai querer abstrair qualquer experimento do seu código base.

`HEAD` é um ponteiro, que aponta para o mais recente commit no branch que você está atualmente trabalhando.

![Branching workflow](feature-branch.png)
