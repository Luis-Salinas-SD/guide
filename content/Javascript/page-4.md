  +++
title = "Funciones"
chapter = true
weight = 4
pre = "<b>4. </b>"
+++
### Funciones
- La definición de una función (también llamada declaración de función o sentencia de función) consiste de la palabra clave (reservada)  function, seguida por:
  + El nombre de la función (opcional).
  + Una lista de argumentos para la función, encerrados entre paréntesis y separados por comas (,).
  + Las sentencias JavaScript que definen la función, encerradas por llaves, { }.
- Ejemplo:
~~~
function cuadrado(number) {
  return number * number;
}
~~~
En una funcion imprime un numero del 0 hasta el que el usuario quiere:
~~~
var num = prompt("introduce un numero");

function cuenta(num){
    for(var i=1; i<=num; i++){
        document.write(i+"\n");
    }
 }cuenta(num);
~~~
Funcion que convierte cadenas con minusculas a cadenas con mayusculas
~~~
var nom =  prompt("Ingresa tu nombre");
function NombreMayus(nom){
nombre = nom.toUpperCase()
console.log(nombre);
}NombreMayus(nom);
~~~

Funcion que calcula el cuadrado de una funcion
~~~
function cuadrado(numero) {
    return numero * numero;
}
console.log( cuadrado(5));
~~~

Funcion dentro de otra Funcion // closure
~~~
function accion(hablar) {
hablar();
}
function decirHola() {
    console.log("hola amicos")
}
accion(decirHola);
~~~
otro ejemplo de closure
~~~
function accion(hablar) {
hablar()
}
accion(function decirHola(){
    console.log("hola amicos como estan");
    }
);
~~~