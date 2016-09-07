---
title: Confirmando cambios
position: 5
---
Para confirmar los cambios agregados al área de preparación utilizamos el comando <strong>*git commit*</strong>. <br>
Si nos olvidamos de agregar un cambio en el commit podemos usar la bandera <strong>*---amend*</strong> para sumar unos archivos al último commit o incluso cambiar el nombre del commit.
{: .info }

```sh
$ git commit -m "mensaje del commit" .
[master c892c3b] Actualizado - git introduccion
 4 files changed, 20 insertions(+), 56 deletions(-)


$ git commit --amend 
```

Para ver la historia de commits se usa el comando  <strong>*git log*</strong>.
{: .info }

```sh
$ git log
commit 94f304bcafb7ec8a71c6592bc8c3dcc867f058e8
Author: Matias Mancilla <mmancilla@justierradelfuego.gov.ar>
Date:   Wed Sep 7 11:22:43 2016 -0300

    mejorado textos

commit f94ffc61749d8de56533dc6c31cb41e64f8f23e0
Author: Matias Mancilla <Matienzo@users.noreply.github.com>
Date:   Thu Sep 1 12:22:57 2016 -0300

    Update commits.md


commit 97ac9b4a751cefb93bf99dfaaf1dc94368432241
Author: Matias Mancilla <Matienzo@users.noreply.github.com>
Date:   Thu Sep 1 12:22:12 2016 -0300

    Update 04_cambios.md

commit f2a6c84f610e61127c2b841637be94e63906fd37
Author: Matias Mancilla <Matienzo@users.noreply.github.com>
Date:   Thu Sep 1 12:16:42 2016 -0300

    Update and rename asd.md to 04_cambios.md
```
