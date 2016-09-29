---
title: Javascript 
position: 1.0
description: Introducción
right_code: |
  ~~~ json
  [
    {
      "id": 1,
      "title": "The Hunger Games",
      "score": 4.5,
      "dateAdded": "12/12/2013"
    },
    {
      "id": 1,
      "title": "The Hunger Games",
      "score": 4.7,
      "dateAdded": "15/12/2013"
    },
  ]
  ~~~
  {: title="Response" }

  ~~~ json
  {
    "error": true,
    "message": "Invalid offset"
  }
  ~~~
  {: title="Error" }
---

JavaScript (abreviado JS) es un lenguaje interpretado, orientado a objetos, basado en prototipos, imperativo, debilmente tipado y dinamico.
{: .info }
Principalmente se usa del lado del cliente
{: .info }
Todos los navegadores modernos interpretan el código JavaScript.
{: .info }
Para interactuar con una página web se provee al lenguaje JavaScript de una implementación del Document Object Model (DOM).
{: .info }
Javascript corre del lado del cliente y tambien del lado del servidor (nodejs, io.js, etc)
{: .info }




~~~ javascript
//alerta que muestra el navegador
alert("Hola Mundo");
//mensaje por consola
console.log("Hola Mundo");

//definicion de una funcion para cambiar texto de un elemento del DOM
function cambiarTexto(){
var elemento = document.getElementById("javascriptbooks_list");
elemento.innerHTML= "Cambiando el texto con Javascript Puro";
};

~~~
{: title="Vanilla Js" }




~~~ javascript

function cambiarTexto(){
var elemento = $("#javascriptbooks_list");
elemento.text("Jquery cambió esto");
};


/*otro ejemplo*/
//defino una variable global
var variableGlobal=0;

//añadir eventos de click a un determinado elemento
$("h1").on('click',function(){
  variableGlobal+=1;
  console.log("numero de clicks = "+variableGlobal);
});

~~~
{: title="Jquery" }




