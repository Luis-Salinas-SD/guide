+++
title = "Bases"
chapter = true
weight = 1
pre = "<b>1. </b>"
+++

# Bases de Javascript
### Bienvenido a una breve explicación sobre lo basico para entender JavaScript

### Variables y Constantes <a id="chapter-1"></a>
Este texto es un parrafo 
- Las variables son espacios de memoria reservados para un valor, este puede ser reasignalble, se pueden declarar con **_"var"_** ó **_"let"_**.

```
let nombre = "Luis";
var apellido = prompt('¿Cual es su apellido?');
```

- Las **_constantes_** son espacios de memoria pero el valor no puede ser reasignado.(tambien son variables).

```
const pi = 3.1416;
```

### Números y Operadores

- Operaciones aritmeticas basicas.

```
let suma = 2+2; //4
let resta = 2-2; //0
let division = 10/2; //5
let mult = 2*2; //4
let resi = 9%2; // residuo
let cuad = 2**3; // 8
console.log(cuad);
```

### Booleans

- Los booleanos solo retornar un valor **_true_** o **_false_**.

```
new Boolean(valor)
```

> Valores que retornan **_false_**
> (**_undefined, NaN, null, 0, -0, false_**).

### Operadores de Comparación. 

- igualdad ==

```
var igual;
igual = 0 == 0 //true
alert(igual);
```

```
var igual;
igual= ('a' === 'a'); //true
```

- desigualdad !==

```

var desigual;
desigual = ('adios' !== 'hola'); //true
```

- Mayor que >

```

var mayor;
mayor = (6 >= 6); //true
```

- Menor que <

```

var menor;
menor = (6 <=6 ); //true
```
<a id="chapter-2"></a>
### Operadores Lógicos


- Los operadores lógicos se usan típicamente con valores Boolean. En tal caso, regresan un valor Boolean (True ó False) y son los siguientes:
- AND
- OR
- NOT

 #### Operador AND
- EN EL OPERADOR ***AND*** AMBAS CONDICIONES DEBEN SER VERDADERAS(TRUE) DE LO CONTRARIO RETORNA UN VALOR (FALSE)
 ~~~
//*++++++++++++++++++++++++++++++++++++++++++++++++++ AND +++++++++++++++++++++++++++++++++++++++++++++++++++++
//# EN EL OPERADOR AND AMBAS CONDICIONES DEBEN SER VERDADERAS(TRUE) DE LO CONTRARIO RETORNA UN VALOR (FALSE)
if(24 === 24 && "hola" === "hola"){
    alert(true);
  }else{
    alert(false);
  }
//true

if(24 === 24 && "hola" === 13){
    alert(true);
  }else{
    alert(false);
  }
  // false
 ~~~

  #### Operador OR
- EN EL OPERADOR OR SOLO UNA CONDICION DEBE SER VERDADERA
~~~
//! Operador ++++++++++++++++++++++++++++++++++++++++++ OR +++++++++++++++++++++++++++++++++++++++++++++++++++++
//# EN EL OPERADOR OR SOLO UNA CONDICION DEBE SER VERDADERA

if(24 === 24 || "hola" === "hola"){
    alert(true);
  }else{
    alert(false);
  }
//TRUE

if(24 === 24 || "hola" === "ADIOS"){
    alert(true);
  }else{
    alert(false);
  }
  //FALSE
~~~
 #### Operador NOT

- sirve para ***negar*** una condicion verdadera con el simbolo !
~~~
  //$ ++++++++++++++++++++++++++++++++++++++++++++++++ NOT +++++++++++++++++++++++++++++++++++++++++++++++++++++
  //# sirve para negar una condicion verdadera con el simbolo !
!(25 === 25) || (10 < 5)
//false
~~~