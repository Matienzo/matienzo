---
title: Introducción
position: 1
---
![Git Logo](/images/git_logo2.jpg){: .center-image .img-responsive }

#### Qué es Git?
------
Git es un sistema de control de versiones <strong>distribuido</strong>. Fue creado por Linus Torvalds y ha sido utilizado para mantener el kernel de Linux. Es por mucho, el sistema de control de versiones mas usado del mundo.
Esta linea no está en el área de preparación.


VCS Centralizado vs VCS distribuido. <br>
<strong> Centralizado:</strong>  Sólo tiene una copia de los archivos, necesita conectarse al repositorio central para trabajar con el. <br>
<strong> Distribuido:</strong>  Tiene una copia exacta local del repositorio, se puede trabajar localmente con el repositorio (hacer commit, branches, etc)
{: .info }

<img src="https://www.git-tower.com/learn/content/01-git/01-ebook/en/02-mac/07-appendix/02-from-subversion-to-git/centralized-vs-distributed.png" class="center-image" style="display: block;	max-width: 70%;	height: auto;">



<br>

#### Instalación
------
Para instalar Git debemos bajarlo de su página oficial [git-scm.com](https://git-scm.com/ "Página oficial de Git"). Para probar si quedó bien instalado (Windows):

```sh
$ git --version
git version 2.5.1.windows.1
```

Luego, para configurar el usuario local para todos los repositorios locales:

```sh
$ git config --global user.name "[name]"
$ git config --global user.email "[email address]"
```




<!-- Welcome to our API.

This API document is designed for those interested in developing for our platform.

This API is still under development and will evolve.

You'll succeed if you do this.
{: .success }

Here's some useful information.
{: .info }

Something may not happen if you try and do this.
{: .warning }

Something bad will happen if you do this.
{: .error } -->
