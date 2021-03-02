+++
title = "Condicionales"
chapter = true
weight = 2
pre = "<b>2. </b>"
+++

### Condicional **_if_** y **if-else**

Si la primer condicion se cumple, la siguiente no se ejecuta, pero si la primera condición no se cumple se ejecuta la segunda en el if(){}else{}

- condicion **_if_**

```javascript
if (24 === 24 || "hola" === "hola") {
  alert(true);
} else {
  alert(false);
}
//true
```

- condicion **_if( ){ }else{ }_**

```javascript
//! Condicional if()else
let nota = 10;
if (nota <= 7) {
  console.log("malo");
} else if (nota == 8) {
  console.log("regular");
} else if (nota == 9) {
  console.log("bueno");
} else {
  console.log("Excelente");
}
```
