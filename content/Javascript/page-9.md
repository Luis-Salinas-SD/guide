  +++
title = "Funcion constructora"
chapter = true
weight = 9
pre = "<b>9. </b>"
+++
### Función Constructura
A continuación se muestra una función constructora de objetos, viendo asi cómo podemos construir un objeto o varios a traves de una función.

> Es importante mencionar que en una **función constructora** el **metodo** de esta debe de iniciar con **this.nombre_metodo**.

- Función Constructora:
~~~
function Curso(titulo, duracion, formato) {
    //! Propiedades/Atributos
    this.titulo = titulo;
    this.duracion = duracion;
    this.formato = formato;

    //! Metodo
    this.inscribir = function (usuario) {
        console.log(usuario + "Está Inscrito");
    }
}
~~~
- Creación de un objeto apartir de una función constructora:
~~~
let cursoJavaScript = new Curso("curso java pro", "5hrs", "Mp4");
let cursoRuby = new Curso("Curso de Ruby Pro");
~~~
- Mandar a llamar el objeto con sus **propiedades/atributos**:
~~~
console.log(cursoJavaScript.titulo, cursoJavaScript.duracion, cursoJavaScript.formato);
console.log(cursoRuby.titulo);
~~~
