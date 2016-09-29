---
title: Javascript 
position: 1.0
description: Introducción
right_code: |
  ~~~ javascript
  //mensaje de alerta
  alert("Hola Mundo");
  //mensaje por consola
  console.log("Hola Mundo");

  //manipulación DOM
  function cambiarTexto(){
    var elemento = document.getElementById("javascriptbooks_list");
    elemento.innerHTML= "Cambiando el texto con Javascript Puro";
  };
  
  var variableGlobal=0;
  var elemento = document.getElementById("javascriptbooks_list");
 
  //eventos
  elemento.addEventListener("click",function(e){
    variableGlobal+=1;
    console.log("numero de clicks = "+variableGlobal);
  },false);
  ~~~
  {: title="Vanilla JS" }

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




