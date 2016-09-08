---
title: Buenas Practicas
position: 9
---
#### Realizar commits de cambios relacionados
------
Un commit debe englobar cambios relacionados. Por ejemplo, para arreglar 2 errores o bugs diferentes se deberian producir dos commits diferentes. Commits pequeños hacen mas facil la lectura para otros desarrolladores. Con la ayuda del área de preparación git hace facil la creación de commits pequeños.


#### Hacer commits regularmente
------
Tener commits pequeños y subirlos regularmente ayuda a la facilidad de integrar cambios y resolver conflictos.




#### No hacer commits con cambios "a la mitad"
------
Se deben commitear cambios cuando el código esté completo. Esto no significa que se tiene que completar una nueva característica para hacer un commit. Se puede dividir un cambio en varias partes y commitear separado.


#### Probar bien los cambios antes de commitearlos
------
Se debe resistir a la tentación de algo que "parece" que está bien. Esto es mas importante si subimos los cambios a un repositorio remoto.


#### Escribir buenos mensajes de commits
------
Para escribir buenos mensajes se recomienda preguntarse: <br>
- Cual es la motivacion del cambio?<br>
- Como difiera de la implementación anterior?<br>
A su vez, debe estar escrito en presente.


#### Usar ramas
------
Las ramas son una de las características mas importantes de git. Se deben usar siempre desde el día cero para nuevos cambios, reparación de errores, nuevas ideas, etc.<br>
Muchos utilizan 3 ramas: Development, Master y HotFix o Feature.
