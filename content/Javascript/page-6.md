  +++
title = "Scope"
chapter = true
weight = 6
pre = "<b>6. </b>"
+++
### Scope
El scoupe es una colección de variables, funiones y objetos al alacnce del codigo.

exiten dos tipos:
- Global scoupe [variables globales]
Las variables globales se pueden mandar a llamar en cualquier parte del programas.

- local scoupe [Variables locales]
Adiferencia de las globales, las locales solo se pueden declarar en la funciones y pueden ser mandadas a llamar
en la misma.

~~~
var nombre = "Luis";//scoupe global

function hola() {
    alert("hola " + nombre);
}hola();

function adios(){
    let nombre = "Ana"; //scoupe local
    alert("adios " + nombre);
}adios();
~~~
- CONST: Es una constante la cual NO cambiara su valor en ningún momento en el futuro.
- VAR: Es una variable que SI puede cambiar su valor y su scope es local (dentro de una función o del bloque global).
- LET: Es una variable que también podrá cambiar su valor, pero solo funcionará en el bloque donde fue declarada (ciclos o  condiciones) su alcance es mucho menor que var.

