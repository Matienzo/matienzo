---
title: Deshaciendo cambios locales
position: 6
---
En caso de que se cometa un error y se desee restaurar un archivo (o todos) al ultimo commit, se usa el comando <strong>*git checkout -- <filename>*</strong>
{: .danger }

~~~ sh
$ git checkout -- <filename>
//Este comando reemplaza los cambios en tu directorio de trabajo con el último commit
~~~
{: title="git diff" }


Por otro lado, si se quiere deshacer todos los cambios locales y commits locales,
{: .danger }

~~~ sh
$ git fetch origin
$ git reset --hard origin/master
~~~
{: title="git diff" }
