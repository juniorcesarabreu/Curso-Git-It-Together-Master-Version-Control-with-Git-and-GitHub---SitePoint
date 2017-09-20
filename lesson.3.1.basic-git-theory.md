Alguma teoria Git
===================================

* Entenda os 3 estados de arquivo em Git
* Entenda as 3 seções de um projeto Git
* Entenda a sintáxe básica do Git
* Entenda o fluxo básico de trabalho do Git

3 principais estados
--------------------------

```txt
Modified   →  Staged  →  Commited
```

* Modified (Modificado)
    Estado dos arquivos no diretório de trabalho que você está atualmente trabalhando sobre.
* Staged (Preparado)
    Estado dos arquivos na área de staged que você tem modificado e adicionado a área de staging (área temporária) para Git tomar um snapshot (cópia de registro).
* Committed (Consolidado)
    Estado dos arquivos após Git ter tomado um snapshot do estado atual e serem armazenados no repo.

3 principais seções de um projeto Git
---------------------------------------

```txt
Modified   →  Staged  →  Commited
    ▲           ▲           ▲
Working      Staging    Repository
diretory      Area
```

* Working diretory = A pasta sobre a qual se está trabalhando atualmente. Contém arquivos no estado modificado.
* Staging Area = Após salvar o arquivo localmente, é necessário dizer ao Git para rastrear as mudanças no arquivo, para que ele possa tomar um snapshot. Isso é feito adicionado o arquivo a staging area.
* Repository = Após o snapshot, o arquivo está comitado e se encontra no repositório Git.

Comandos Git
--------------------------------------

```git
Git <action keyword>

    For example:
git add
git commit
git push
```

Fluxo de trabalho Git básico
------------------------------------

Fluxo de trabalho (Workflow)
    Sequência de passos para completar uma tarefa

Fluxo de trabalho Git básico
    1. Modificar arquivos no diretório de trabalho
    2. Adicionar arquivos para a staging area
    3. Comitar arquivos para o repositório

```txt
        git add     git commit
Modified    →   Staged   →   Commited
    ▲             ▲             ▲
Working        Staging      Repository
diretory        Area
```
