---
title: Deshaciendo cambios
position: 6
---
En cualquier momento se puedes querer deshacer algún cambio realizado. Git ofrece varios comandos para deshacer algún cambio realizado como <strong>*git checkout*</strong> o <strong>*git reset*</strong>. <br>
El comando *git status* muestra como deshacer cambios.
{: .info }

Hay que tener cuidado porque no siempre se puede volver atrás después de algunas de estas operaciones y se pueden perder datos.
{: .error }

Deshacer los cambios de la copia local al último commit <strong>*git checkout*</strong><br>
Esta operación no se puede revertir:
{: .info }

~~~ sh
$ git checkout -- <filename>

$ git checkout

~~~

Por otro lado, si se quiere deshacer todos los cambios locales y commits locales:
{: .danger }

~~~ sh
$ git fetch origin
$ git reset --hard origin/master
~~~


En caso de que se cometa un error y se desee restaurar un archivo (o todos) al ultimo commit, se usa el comando <strong>git checkout -- <filename> </strong><br>
{: .info }
~~~ sh
$ git checkout <filename>

~~~
