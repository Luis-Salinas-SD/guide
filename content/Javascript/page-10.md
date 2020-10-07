+++
title = "Clases"
chapter = true
weight = 10
pre = "<b>10. </b>"
+++
### Clases
Las clases de javascript, introducidas en ECMAScript 2015, son una mejora sintáctica sobre la herencia basada en prototipos de JavaScript. La sintaxis de las clases no introduce un nuevo modelo de herencia orientada a objetos en JavaScript. Las clases de JavaScript proveen una sintaxis mucho más clara y simple para **crear objetos y lidiar con la herencia.**

- Las **clases** son un modelo a seguir
- Un **objeto** es una instancia de una clase
- Los **atributos** son las caracateristicas o propiedades de objetos
- Los **métodos** son acciónes (funciones) que un objeto puede realizar
### Declaración de una clase
- Las clases no reciben parametros.
- Las clases tienen un metodo especial que se llama **constructor** y recibe las propiedades del objeto, este se ejecuta en el momento de instanciar la clase.

~~~
// ++++++++++ clase ++++++++++
class Perro{
    // ++++++++++ constructor ++++++++++
    constructor(nombre,genero){
        //atributos
        this.nombre = nombre;
        this.genero = genero;
    }// ++++++++++ constructor ++++++++++

    //++++++++++ Metodo ++++++++++
    ladrad(){
        console.log("Guaf Guaf");
    }//++++++++++ Metodo ++++++++++
    
}// ++++++++++ clase ++++++++++

const simba = new Perro("simba","macho");
console.log(simba);	//mandar a llamar al objeto
simba.ladrad();	// mandar a llamar al metodo
~~~

### Herencia

Para utilizar herencia se necesita la palabra reservada **extends** seguido de la clase padre o de la que quiere que herede.

la palabra reservada **super()** manda a llamar al constructor de la calse padre.
~~~
class Perro {
    // ++++++++++ constructor ++++++++++
    constructor(nombre, genero) {
        //atributos
        this.nombre = nombre;
        this.genero = genero;
    } // ++++++++++ constructor ++++++++++

    //++++++++++ Metodo ++++++++++
    ladrad() {
        console.log(` guaf guaf mi nombre es ${this.nombre}`);
    }
    caminar(){
        console.log("Toy caminando");
    }
    //++++++++++ Metodo ++++++++++
} // ++++++++++ clase ++++++++++

const simba = new Perro("simba", "macho");
console.log(simba);//! mandar a llamar al objeto
simba.ladrad();//! mandar a llamar al metodo


// ############ HERENCIA ##########
class Gato extends Perro{
    constructor(nombre, genero, color){
        super(nombre, genero);
        this.color = color;
    }
    ladrad(){
        console.log(`miau miau mi nombre es ${this.nombre}`);
    }
}
const beto = new Gato("beto","hembra","blanco");
console.log(beto);
beto.ladrad();
beto.caminar();
~~~

