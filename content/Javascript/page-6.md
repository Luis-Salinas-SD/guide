  +++
title = "Scope"
chapter = true
weight = 6
pre = "<b>6. </b>"
+++
### Funciones Flecha

Una expresión de **función flecha** es una alternativa compacta a una expresión de función tradicional, **pero es limitada y no se puede utilizar en todas las situaciones.**
- Funcion convencional:

~~~
function suma(a, b) {
    return a + b;
} console.log(suma(5, 5));
~~~
- Arrow-function
~~~
suma = (a, b) => a + b
console.log(suma(5, 5)); //10
~~~
La sintaxis básica de una _**arrow-function**_ es la siguiente:
~~~
nombre_function = (parametros) => {cuerpo_funcion}
~~~

### Ejemplos:
imprimir los numeros en pantalla hasta el numero que el usuario teclea
~~~
var n = prompt("introduce el numero:");

cuenta = (n) => {
    for (i = 0; i <= n; i++) {
        document.writeln(i);
    }//for
}//arrow-function cuenta
cuenta(n);
~~~
Aqui hay un objeto llamdo **tutor** y dentro de sus propiedades se encunetra una funcion, que lo que hace es imprimir el nombre con ayuda del metodo **setTimeout** despues de cierto tiempo. 

La propiedad que contiene esta funcion es **fullNombre.**
~~~
let tutor = {
    nombre: "Luis",
    apellido: "Salinas",
    fullNombre: function () {
        setTimeout(() => { console.log(this.nombre + " " + this.apellido); }, 1000)
    }
}
// console.log(tutor.apellido);
tutor.fullNombre();
~~~