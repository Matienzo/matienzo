---
title: Realizando cambios
position: 4
---
Git tiene un índice (index), que funciona como una especie de área de preparación para los
cambios que uno va realizando en los archivos a medida que va trabajando. <br>
Uno debe agregar los archivos al área de preparación de forma <strong>explícita</strong> (git add y git rm).


Agregando y quitando archivos modificados del área de preparación:.
{: .info }

```sh
$ git add .      
$ git add <file or directory>     
$ git add *.js app/Http/Controllers/Controller.php app/Http/Routes    


$ git rm .  
$ git rm <file or directory>
$ git rm *.json

```

Para saber qué archivos cambiaron desde el último commit usamos el comando <strong>*git status*</strong>. Esto nos permite saber que cambios se hicieron en el directorio de trabajo y cuales estan en el área de preparación.
{: .info }


~~~ sh
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
~~~
{: title="git status" }


Para ver las diferencias o cambios que vamos realizando usamos <strong>*git diff*</strong>.<br>
<strong>git diff</strong>: Muestra las diferencias entre la copia de trabajo y el área de preparación.<br>
<strong>git diff HEAD</strong>: Muestra las diferencias entre la copia de trabajo (esten o no en el área de preparación) y el último commit.
{: .info }

~~~ sh
$ git diff

$ git diff HEAD
~~~
{: title="git diff" }
