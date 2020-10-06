  +++
title = "Objetos - JSON"
chapter = true
weight = 8
pre = "<b>8. </b>"
+++
### Objetos - JSON

Declaración de un objeto JSON

Puede recibir diferentes valores como:
- arreglos
- objetos
- funciones (metodos)
- booleans
- enteros
- strings
~~~
let video = {
    titulo: "piloto",
    duración: 2,
    formato: "avi",
    //!arreglo
    arreglo: ["uno", "dos", "tres"],
    //!metodo
    inscribir: function (usuario) {
        console.log(usuario + " Esta inscrito");
    }
}
~~~
> Dentro de una objeto **las variables** son llamada **propiedades o atributos.**

> Dentro de un objeto **las funciones** son llamadas **metodos**.

De acuerdo al objeto anterior esto es lo que podemos hacer.
~~~
//! invocar una propiedad del objeto.
console.log(video.arreglo);

//! Invocar el metodo
video.inscribir("Juan");

//! Editar alguna propiedad de nuestro objeto
video.titulo = "Prueba";
console.log(video.titulo);

//! Editar alguna metodo de nuestro objeto
video.inscribir = function () {
    console.log("hola soy la funcion editada");
}
~~~