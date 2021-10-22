+++
title = "Bases"
chapter = true
weight = 1
pre = "<b>1. </b>"
+++

# Bases de Javascript

Bienvenido a una breve explicación sobre los temas básicos para entender JavaScript.

# Variables y Constantes

Las variables son espacios de memoria reservados para un valor, este puede ser reasignable(menos en **const**), se pueden declarar con **_"var"_** ó **_"let"_**.

```javascript
let nombre = "Luis";
var apellido = prompt("¿Cual es su apellido?");
```

Las **_constantes_** son espacios de memoria pero el valor no puede ser reasignado.(tambien son variables).

```
const pi = 3.1416;
```

> **const:** no puede cambiar el valor.

> **let:** el scope es local.

> **var:** el scope es global (es mejor dejar de utilizar var).

# Números y Operadores

Operaciones aritmeticas basicas.

```javascript
let suma = 2 + 2; //4
let resta = 2 - 2; //0
let division = 10 / 2; //5
let mult = 2 * 2; //4
let resi = 9 % 2; // residuo
let cuad = 2 ** 3; // 8
console.log(cuad);
```

# Booleans

Los booleanos solo retornar un valor **_true_** o **_false_**.

```javascript
new Boolean(valor);
```

> Valores que retornan **_false_**
> (**_undefined, NaN, null, 0, -0, false_**).

# Operadores de Comparación.

### Igualdad **==** & Identico **===**

```javascript
var igual;
igual = 0 == 0; //true
alert(igual);
```

```javascript
var igual;
igual = "a" === "a";
//true
```

> **===** el comparador identico evalua el tipo de dato y el valor.

### Desigualdad **!==**

```javascript
var desigual;
desigual = "adios" !== "hola"; //true
```

### Mayor que **>**

```javascript
var mayor;
mayor = 6 >= 6; //true
```

### Menor que **<**

```javascript
var menor;
menor = 6 <= 6; //true
```

<a id="chapter-2"></a>

# Operadores Lógicos

Los operadores lógicos se usan típicamente con valores Boolean. En tal caso, regresan un valor Boolean (True ó False) y son los siguientes:

- AND
- OR
- NOT

## Operador AND

- EN EL OPERADOR **_AND_** AMBAS CONDICIONES DEBEN SER VERDADERAS(TRUE) DE LO CONTRARIO RETORNA UN VALOR (FALSE)

```javascript
if (24 === 24 && "hola" === "hola") {
  alert(true);
} else {
  alert(false);
}
//true

if (24 === 24 && "hola" === 13) {
  alert(true);
} else {
  alert(false);
}
// false
```

## Operador OR

- EN EL OPERADOR OR **SOLO UNA CONDICION DEBE SER VERDADERA**

```javascript
if (24 === 24 || "hola" === "hola") {
  alert(true);
} else {
  alert(false);
}
//true

if (24 === 24 || "hola" === "ADIOS") {
  alert(true);
} else {
  alert(false);
}
//false
```

## Operador NOT

- sirve para **negar** una condicion verdadera con el simbolo !

```javascript
!(25 === 25) || 10 < 5;
//false
```
