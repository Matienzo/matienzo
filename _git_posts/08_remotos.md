---
title: Trabajando con Repositorios Remotos
position: 8
---
Para poder compartir los cambios que hemos hecho en un repositorio local debemos subirlo a un repositorio compartido. Estos repositorios se llaman repositorios remotos y sirven para traernos cambios (pull) y subir nuestros cambios (push).


Registrar un repositorio remoto llamado "desa" y luego consultar todos los repositorios remotos:
{: .info }

~~~ sh
$ git remote add desa //192.168.40.6/sistemas/Laravel5/intranet5.git

$ git remote -v
desa  //192.168.40.6/sistemas/Laravel5/intranet5.git (fetch)
desa  //192.168.40.6/sistemas/Laravel5/intranet5.git (push)

$ git remote rm desa

~~~


Para subir cambios locales (de la rama master) al repositorio remoto (en este caso origin):
{: .info }

~~~ sh
$ git push origin master
Counting objects: 437, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (314/314), done.
Writing objects: 100% (437/437), 1.34 MiB | 0 bytes/s, done.
Total 437 (delta 72), reused 0 (delta 0)
To //192.168.40.6/sistemas/Laravel5/intranet5.git
 * [new branch]      master -> master
~~~


Para traer cambios del repositorio remoto a nuestro repositorio local:
{: .info }

~~~ sh
$ git pull origin master

$ git fetch origin master
~~~

Git pull: Hace un git fetch && git merge<br>
Git fetch: Trae cambios sin hacer merge
{: .success }
