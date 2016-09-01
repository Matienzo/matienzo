---
title: Crear repositorios
position: 2
---
Hay dos formas de empezar a trabajar con Git. Una es creando un repositorio y otra es clonando un repositorio existente.

#### Crear nuevo repositorio
Para crear un repositorio utilizamos el comando *git init*.



Una vez inicializado, git comienza a hacerle un seguimiento a todos los cambios que se produzcan en el directorio donde este el repositorio.

<br>

#### Clonar un repositorio existente
La otra forma de comenzar es clonando un repositorio ya existente. Para ello se utiliza el comando *git clone*. 

```sh
$ git clone https://github.com/laravel/laravel.git
Cloning into 'laravel'...
remote: Counting objects: 27277, done.
remote: Total 27277 (delta 0), reused 0 (delta 0), pack-reused 27277
Receiving objects: 100% (27277/27277), 7.63 MiB | 226.00 KiB/s, done.
Resolving deltas: 100% (16592/16592), done.
Checking connectivity... done.
```

Con esto tendríamos el repositorio de Laravel completo en nuestra computadora. Podemos ver toda su historia (+5000 commits, 5 branches, 60 releases).








