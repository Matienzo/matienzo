---
title: Realizando cambios
position: 4
---
Git tiene un índice (index), que funciona como una especie de área de preparación para los
cambios que uno va realizando en los archivos a medida que va trabajando. <br>


Para agregar archivos modificados al área de preparación usamos el comando <strong>*git add*</strong>.
{: .info }

```sh
$ git add .   |   git add <file or directory>   
```

Para quitar cambios del área de preparación, usamos el comando <strong>*git rm*</strong>.
{: .info }
```sh
$ git rm .   |   git rm <file or directory>   
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

Las diferencias entre lo que esta en el directorio de trabajo o en el área de preparación lo podemos ver con <strong>*git diff*</strong>.
{: .info }


~~~ sh
$ git diff
//Este comando muestra las diferencias de los archivos que no estan en el área de preparacion

~~~
{: title="git diff" }

~~~ sh

$ git diff HEAD
//Este comando muestra todas las diferencias de los archivos desde el ultimo commit (sin importar si los cambios estan o no en el área de preparación)
~~~
{: title="git diff HEAD" }





Lists all the photos you have access to. You can paginate by using the parameters listed above.

~~~ javascript
$.get("http://api.myapp.com/books/", { "token": "YOUR_APP_KEY"}, function(data) {
  alert(data);
});
~~~
{: title="jQuery" }

~~~ python
r = requests.get("http://api.myapp.com/books/", token="YOUR_APP_KEY")
print r.text
~~~
{: title="Python" }

~~~ javascript
var request = require("request");
request("http://api.myapp.com/books?token=YOUR_APP_KEY", function (error, response, body) {
  if (!error && response.statusCode == 200) {
    console.log(body);
  }
});
~~~
{: title="Node.js" }

~~~ bash
curl http://sampleapi.readme.com/orders?key=YOUR_APP_KEY
~~~
{: title="Curl" }
