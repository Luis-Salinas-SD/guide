+++
title = "Ciclos"
chapter = true
weight = 3
pre = "<b>3. </b>"
+++

# Ciclos

## Ciclo For

El bucle FOR se utiliza para repetir una o más instrucciones un determinado número de veces. De entre todos los bucles, el FOR se suele utilizar cuando sabemos seguro el número de veces que queremos que se ejecute. La sintaxis del bucle for se muestra a continuación.

```javascript
for (inicialización; condición; actualización) {
  //sentencias a ejecutar en cada iteración
}
```

- imprime una serie del 1 al 10

```javascript
for (var i = 1; i <= 15; i++) {
  alert(i);
}
```

- imprime los multiplos de 7

```javascript
for (let i = 0; i < 50; i++) {
  if (i % 7 === 0) {
    console.log(i);
  }
}
```

**_uso de continue_**

- continue = ignora la sentencia
- no imprimir los multiplos de 7

```javascript
for (let i = 0; i < 50; i++) {
  if (i % 7 === 0) {
    continue;
    console.log(i);
  }
  console.log(i);
}
```

- no imprime los multiplos de 5

```javascript
for (let i = 0; i < 10; i++) {
  if (i % 5 === 0) {
    continue;
  }
  console.log(i);
}
```

- breake = romper el ciclo despues de llegue a 5

```javascript
var n = 0;
for (let i = 0; i < 50; i++) {
  if (i % 7 === 0) {
    console.log(i);
    n++;
  }
  if (n >= 5) {
    break;
  }
}
```

## Ciclo DO-WHILE

El ciclo do-while primero realiza la acción y despues evalua la condicion.

- sintaxis

```javascript
do sentencia;
while (condición);
```

Números del 1 al 5

```javascript
//numeros del uno al 5
let num = 0;
do {
  console.log(num);
  num++;
} while (num <= 5);
```

Mini-loggin

```javascript
//mini login (solo logica)
var password = "Luis";
var pas;
do {
  var pas = prompt("Constraseña");
} while (password !== pas);
```

## Ciclo WHILE

el ciclo while mientras se cumpla la condicion realiza la sentencia.

- sintaxis

```javascript
while (condicion) sentencia;
```

```javascript
//!Ceunta regresiva del 10 al 0
var numero = 11;
while (numero <= 10) {
  //   alert(numero);
  numero--;
  console.log(numero);
  if (numero === 0) {
    break;
  }
}

//Ejercicio:
var edad = prompt("Dime tu edad");
var num = parseInt(edad, 10);
console.log(num);
```

- SWITCH

```javascript
var answer = prompt("Dame un numero del 1 al 3");
switch (answer) {
  case "1":
    alert("Bad Bunny");
    break;
  case "2":
    alert("50 cent");
    break;
  case "3":
    alert("Maluma");
    break;
  default:
    alert("tienes que colocar un numero del 1 al 3");
    break;
}
```
