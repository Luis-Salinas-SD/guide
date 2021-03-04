+++
title = "Funciones"
chapter = true
weight = 4
pre = "<b>4. </b>"
+++

# Funciones

- La definición de una función consiste de la palabra clave (reservada) function, seguida por:
  - El **nombre** de la función (opcional).
  - Una lista de **argumentos** para la función, encerrados entre paréntesis y separados por comas (,).
  - Las **sentencias** JavaScript que definen la función, encerradas por llaves, { }.
- Ejemplo:

```javascript
function cuadrado(number) {
  return number * number;
}
```

## Funciones **declarativas** y **anónimas**

### Funciones Declarativas:

- En las funciones declarativas, utilizamos la palabra reservada **function** al inicio para poder declarar la función:

```javascript
function saludar(nombre) {
  console.log(`Hola ${nombre}`);
}

saludar("Diego");
```

### Funciones Anónimas:

- La declaración se inicia con la palabra reservada (**var, let, const**), donde se generará una variable que guardará un función anónima.

```javascript
var nombre = function (nombre) {
  console.log(`Hola ${nombre}`);
};

nombre(`Diego`);
```

### Ejercicios:

- En una funcion imprime un numero del 0 hasta el que el usuario quiere:

```javascript
var num = prompt("introduce un numero");

function cuenta(num) {
  for (var i = 1; i <= num; i++) {
    document.write(i + "\n");
  }
}
cuenta(num);
```

- Funcion que convierte cadenas con minusculas a cadenas con mayusculas

```javascript
var nom = prompt("Ingresa tu nombre");
function NombreMayus(nom) {
  nombre = nom.toUpperCase();
  console.log(nombre);
}
NombreMayus(nom);
```

- Funcion que calcula el cuadrado de una funcion

```javascript
function cuadrado(numero) {
  return numero * numero;
}
console.log(cuadrado(5));
```

### Closure

Un closure es una función dentro de otra funcion que está disponible sólo dentro del cuerpo de esa fucnión y que tiene accesos a las variables de la función dónde fue declarda.

- sintaxis

```javascript
// funcion padre
function iniciar() {
  let name = "luis";
  // funcion hijo
  function mostrar() {
    console.log(name);
  }
  mostrar();
}
iniciar();
```

#### otros ejemplos de closure

```javascript
// Funcion 1 () Closure
function fun1() {
  fun2();
}
fun1(fun2);
// Funcion 2
function fun2() {
  console.log("Adios mundo");
}
```

```javascript
function accion(hablar) {
  hablar();
}
function decirHola() {
  console.log("hola amicos");
}
accion(decirHola);
```

```javascript
function accion(hablar) {
  hablar();
}
accion(function decirHola() {
  console.log("hola amicos como estan");
});
```
