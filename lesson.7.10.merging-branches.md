Unindo branch featureB dentro de featureA
=========================================

```sh
$ git checkout featureA
$ git merge featureB # Como ambos os branch estavam em desenvolvimento, o algoritmo determinou a criação de um novo commit, sendo um 3 way merge portanto
# Auto-merging index.html
# Merge made by the 'recursive' strategy.
$ git log --pretty=oneline
# 33990a20a2a076e51cff2a54b324498aade8f498 (HEAD -> featureA) Merge branch 'featureB' into featureA
# e25dd32b65f4a932292ab504a7e104570dffe237 (origin/featureB, featureB) Edited paragraph on feature B
# f201f3618b9ed6e6bcdf45fc40983cf002504371 (origin/featureA) Incorporated <p> changes
# 2b7677be5cb97f5725c135cbfa9a7b62cc101bb2 Edited paragraph
# d99749706d5913947040da781a6d7c6b610256d6 Change text Lara
# d48d717e3366b6fdc6545dbb77af93559426118a Initial commt on feature B
# ff324385b3d89fc502897c440bc1509c3742eaa3 Initial commit on feature A
# 9f0b6a5ef9fe78c47d62e8ce89e100b9ecfa94f2 (origin/master) Kept mustard color
# 1bfdb43a94f43042a32cfb71f48eb04bd11b12c0 Change color to a mustard shade
# 733d71ee7bcab9460a25d29cfc9d0587a37e2b3f Change color to another by Lara
# 95fde523e369c84b8acf3700b1369463cf423ef9 Merging remote changes by Lara
# c248be31a169a8dddd7d21a7ccf7ac29141711a1 Change the color of brand class
# 9a9310c30bbd62af87fb308aae51ed38295c0f6d Final edit by Lara
# ba31b0fbd6ad092c3a621cecd067bbc72d7dc6ed 3rd edit by Lara
# 650def197a9067da41f10e633c6f427d912ff9ee 2nd edit by Lara
# adbdd4d871b31bed31f9ce0bd37cb876fb9d12a1 1st edit by Lara
# b8d28267e5ae2437dd623e32af223233486ebd9d Revert "Commiting our third mistake, we left the other two in place"
# 8e2eeafee2056b1ac04c23803243fb451744fbb6 Commiting our third mistake, we left the other two in place
# 3e49998b9ccd7d7d47a7e10b4810f4f5d5aeda1d Change itens after carousel
# b6d8d937d27d3f78a3f5a6b6081ea4bed1b14ad2 Changed title, subtitle and navbar itens
# 68d0779b40856a765c9ef5d97c356c46df57f025 initial commit, pushing theme over to github

```
