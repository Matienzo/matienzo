---
title: Crear repositorios
position: 2
---
Hay dos formas de empezar a trabajar con Git. Una es creando un repositorio y otra es clonando un repositorio existente. <br>
Una vez tengamos inicializado o clonado un repositorio, git comenzará a hacerle un seguimiento a todos los archivos del repositorio (y a los que se vayan agregando).

#### Crear nuevo repositorio
------
Para crear un repositorio vacío utilizamos el comando <strong>*git init*<strong>.<br>



Inicializar un repositorio vacío en el directorio actual o en un directorio específico:
{: .info }
```sh
$ git init
Initialized empty Git repository in ... (path)

$ git init <directory>
Initialized empty Git repository in <directory>

```

Inicializar un repositorio "---bare". Estos repositorios no tiene copia de trabajo. <br>
<strong> Los repositorios compartidos deben ser siempre ---bare.</strong>
{: .info }
```sh
$ git init --bare <directory>
Initialized empty Git repository in <directory>
```

<br>

#### Clonar un repositorio existente
------
Para clonar un repositorio se utiliza el comando <strong>*git clone*</strong>. Una vez clonado un repositorio, tendremos la copia exacta del repositorio al momento de la clonación, por lo que podremos ver toda su historia.
{: .info }

Ejemplo: Clonar el repositorio oficial de Laravel (alojado en Github)
{: .info }
```sh
$ git clone https://github.com/laravel/laravel.git
Cloning into 'laravel'...
remote: Counting objects: 27277, done.
remote: Total 27277 (delta 0), reused 0 (delta 0), pack-reused 27277
Receiving objects: 100% (27277/27277), 7.63 MiB | 226.00 KiB/s, done.
Resolving deltas: 100% (16592/16592), done.
Checking connectivity... done.
```

Con esto tendríamos el repositorio de Laravel completo en nuestra carpeta local. Podemos ver toda su historia (+5000 commits, 5 branches, 60 releases etc).
