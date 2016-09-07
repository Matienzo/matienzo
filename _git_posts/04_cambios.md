---
title: Realizando cambios
position: 4
---
Para saber qué archivos cambiaron desde el último commit usamos el comando <strong>*git status*</strong>.
{: .info }
```sh
$ git status
On branch master
Your branch is up-to-date with 'origin/master'.
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        modified:   _git_posts/01_git_introduccion.md


Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   _git_posts/02_creando_repositorio.md
        modified:   _git_posts/03_workflow.md
        modified:   _git_posts/04_cambios.md

```

Para agregar cambios al "staging area" (área de preparación), usamos el comando <strong>*git add*</strong>.
{: .info }

```sh
$ git add .   |   git add <file or directory>   
```

Para quitar cambios del área de preparación, usamos el comando <strong>*git rm*</strong>.
{: .info }
```sh
$ git rm .   |   git rm <file or directory>   
```
