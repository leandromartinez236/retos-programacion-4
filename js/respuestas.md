## ¿Qué es una variable y para qué sirve?

- es una forma de almacenar un valor en la memoria RAM,
  para poder reutilizarlas, calcularlas, etc

## ¿Cuál es la diferencia entre declarar e inicializar una variable?

- Declarar es dar un nombre a la variable ej: `let numero`
- Inicializar es **asignar** un valor a la variable ej: ``

## ¿Cuál es la diferencia entre sumar números y concatenar strings?

- La suma ses realiza unicamente con variables de tipo number
- La concatenacion se realiza uniendo string con otros valores

## ¿Qué operador me permite sumar o concatenar?

- Operador suma: `+`

## Determina el nombre y tipo de dato para almacenar en variables la siguiente

## información:

Nombre `const nombre = 'Esteban'`
Apellido `const apellido = mamani`
Nombre de usuario `const username = 'ecrmamani'`
Edad `let edad = 18`
Correo electrónico `let email = 'estebandamian@gmail.com'`
Mayor de edad `let mayorEdad = 'true'`
Dinero ahorrado `let ahorro = 200000`
Deudas `let = 0`

## Traduce a código JavaScript las variables del ejemplo anterior y deja tu código en un archivo nuevo.

`const persona = { nombre: 'Ulises', apellido. 'acosta', username: 'acosta', edad: 18, email: 'ulisesacosta@gmail.com', mayorEdad: true, ahorros: 1000, deudas: 2000, }`

## Calcula e imprime las siguientes variables a partir de las variables del ejemplo anterior:

- Nombre completo (nombre y apellido)
  `const nombreCompleto = persona.nombre + ' ' + persona.apellido`
- Dinero real (dinero ahorrado menos deudas)
  `const patrimonio = persona.ahorro - persona.deudas`

## ¿Qué es una función?

- Es un conjunto de instrucciones agrupados en un bloque de codigo

## ¿Cuándo me sirve usar una función en mi código?

- Me sirve para dividir mis tareas en diferentes que realizan una unica tarea

## ¿Cuál es la diferencia entre parámetros y argumentos de una función?

- Parametros son cuando inicializamos la funcion
- Argumentos son cuando llamano a la funcion

## Convierte el siguiente código en una función, pero, cambiando cuando sea necesario las variables constantes por parámetros y argumentos en una función

`const name = "Juan David";
const lastname = "Castro Gallego";
const completeName = name + lastname;
const nickname = "juandc";

console.log("Mi nombre es " + completeName + ", pero prefiero que me digas " + nickname + ".");`

`function presentacion (completeName, nikName) { const frase = 'Mi nombre es ${completeName}, pero prefiero que me digas ${nikName}.'
}

## presentacion(completeName, nikName); console.log(res)`

## ¿Qué es una condicional?

- Los condicionales es una forma de controlar el flujo de ejecucion de mi codigo. Por el lado verdadero y el falso

## ¿Qué tipos de condicionales existen en JavaScript y cuáles son sus diferencias?

- Existe 4 tipos: if else, else if, switch y if ternario. Cuando tenemos varios else if anidados nos conviene usar switch

## ¿Puedo combinar funciones y condicionales?

- Si

## Replica el comportamiento del siguiente código que usa la sentencia switch utilizando if, else y else if:

`const tipoDeSuscripcion = "Basic";

switch (tipoDeSuscripcion) {
case "Free":
console.log("Solo puedes tomar los cursos gratis");
break;
case "Basic":
console.log("Puedes tomar casi todos los cursos durante un mes");
break;
case "Expert":
console.log("Puedes tomar casi todos los cursos durante un año");
break;
case "ExpertPlus":
console.log("Tú y alguien más pueden tomar TODOS los cursos durante un año");
break;
default:
break;
}`

`if (tipoDeSubscripcion === 'Free') { console.log("Solo puedes tomar los cursos gratis"); } else if (tipoDeSubscripcion === 'Basic') { console.log("Puedes tomar casi todos los cursos durante un mes"); }else if (tipoDeSubscripcion === 'Expert') { console.log("Puedes tomar casi todos los cursos durante un año"); }else if (tipoDeSubscripcion === 'ExpertPlus') { console.log("Tú y alguien más pueden tomar TODOS los cursos durante un año"); }`

## Replica el comportamiento de tu condicional anterior con if, else y else if, pero ahora solo con if (sin else ni else if).

`if (tipoDeSubscripcion === 'Free') console.log("Solo puedes tomar los cursos gratis");`
`if (tipoDeSubscripcion === 'Basic') console.log("Puedes tomar casi todos los cursos durante un mes");`
`if (tipoDeSubscripcion === 'Expert') console.log("Puedes tomar casi todos los cursos durante un año");`
`if (tipoDeSubscripcion === 'ExpertPlus') console.log("Tú y alguien más pueden tomar TODOS los cursos durante un año");`

## Bonus: si ya eres una experta o experto en el lenguaje, te desafío a comentar cómo replicar este comportamiento con arrays y un solo condicional.

`const subs = ['Free', 'Basic', 'Expert', 'ExpertPlus']`
`const mensaje = ['mens1', 'mens2', 'mens3', 'mens4']`
`const pos = subs.indexOf(tipoDeSubscripcion)`
`if (pos !== -1) { `console.log()` }`

## ¿Qué es un ciclo?

- Es cuando se repite varias veces un mismo codigo

## ¿Qué tipos de ciclos existen en JavaScript?

- Existen 3 tipos de ciclos **while**, **for** y **do while**

## ¿Qué es un ciclo infinito y por qué es un problema?

- Es cuando el codigo no se detiene y pasa porque no ponemos un "limite"

## Puedo mezclar ciclos y condicionales?

- Si

## Replica el comportamiento de los siguientes ciclos for utilizando ciclos while:

for (let i = 0; i < 5; i++) {
console.log("El valor de i es: " + i);
}
for (let i = 10; i >= 2; i--) {
console.log("El valor de i es: " + i);
}

while(i =)

## Escribe un código en JavaScript que le pregunte a los usuarios cuánto es 2 + 2. Si responden bien, mostramos un mensaje de felicitaciones, pero si responden mal, volvemos a empezar.

## Pista: puedes usar la función prompt de JavaScript.

const preg = Number(prompt('Cuanto es 2 + 2 = ?'))

if(preg === 4) {
alert('Felicitaciones')
}else {
alert('Respuesta incorrecta')
}

## ¿Qué es un array?

- Es como un almacen donde podemos guardar string, numeros etc.

## ¿Qué es un objeto?

- Es una entidad con propiedades y tipos

## ¿Cuándo es mejor usar objetos o arrays?

- El array se usa más para guardar distintas cosas
- El objeto se lo usa cuando quieres saber más sobre algo, es como tener la descripcion de un producto

## ¿Puedo mezclar arrays con objetos o incluso objetos con arrays?

- En los objetos no pueden haber arrays, pero si puede haber un objeto dentro de un array.

## Crea una función que pueda recibir cualquier array como parámetro e imprima su primer elemento.
