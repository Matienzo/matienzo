---
title: Trabajando con Ramas
position: 7
---
Las ramas son utilizadas para desarrollar funcionalidades aisladas unas de otras. La rama master es la rama "por defecto" cuando creas un repositorio.
{: .info }

![Git Logo](/images/branch.png){: .center-image .img-responsive }


Crear una nueva rama llamada "feature_x"
{: .info }
~~~ sh
$ git checkout -b feature_x
~~~

Volver a la rama master
{: .info }
~~~ sh
$ git checkout master
~~~

Para fusionar otra rama a tu rama activa (por ejemplo master), utiliza *git merge*
{: .info }
~~~ sh
$ git merge <branch>
~~~


Eliminar la rama
{: .info }
~~~ sh
$ git branch -d feature_x
~~~

Una rama nueva no estará disponible para los demás a menos que subas (push) la rama a tu repositorio remoto
{: .error }
