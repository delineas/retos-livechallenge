# Retos LiveChallenge



> En la parte final, las míticas FAQ



## Reto 1: El árbol de jotason a HTML



> Crear una función que convierta un árbol de JSON en una lista de HTML.



Este podría ser el JSON para utilizar:

````js
const tree = {
  tag: "ul",
  children: [
    {
      text: "Primer elemento"
    },
    {
      text: "Cáspita, otro elemento"
    },
    {
    	text: "El último"
    }
  ]
};
````



La función sería algo como esto:

````
convertJsonToHtml(tree)
````



Y el resultado final sería:

````html
<ul>
	<li>Primer elemento</li>
	<li>Cáspita, otro elemento</li>
	<li>El último</li>
</ul>
````





**Requisitos**

- El resultado final es una cadena de texto, no es necesario colocarla en una web.
- Consideramos que el árbol de JSON es correcto.
- El árbol original no tiene elementos anidados.



**Cómo hacerlo**

- Cualquier lenguaje de programación es válido.



### Extras

El reto ya estaría finalizado, pero si quieres ir más allá tienes opciones:

1. Ampliar la función para añadir un parámetro con la indentación del las etiquetas `<li>` (los espacios colocados antes de esa etiqueta)
2. Permitir elementos anidados usando la propiedad `children` 
3. Añadir una propiedad para cada `<li>` que permita definir la `class`.



**Ejemplo de árbol complejo para los extras**

````js
const tree = {
  tag: "ul",
  children: [
    {
      text: "Primer elemento"
    },
    {
      text: "Cáspita, otro elemento",
      children: [
        {
          tag: "ul",
          children: [
            {
              text: 'Primer heredero del cáspita'
            },
            {
              text: 'Último heredero del cáspita'
            }
          ]
        }
      ]
    },
    {
    	text: "El último"
    }
  ]
};
````





Reto inspirado en el de [IOSamuel](https://github.com/iosamuel/algorithms/tree/master/jsonTreeToHTMLList).



## Reto 2: Un widget de cuenta atrás



> Crear una cuenta atrás de 20 segundos.



**Requisitos**

- En una web tener un contador hacia atrás de 20 segundos. 
- La cuanta atrás arranca cuando cargas la página.
- Se tiene que ver como baja el contador, solo segundos (20, 19, 18...)
- Cuando llega a 0 se para.
- No hace falta un estilo de diseño concreto, ¡imaginación al poder!



**Cómo hacerlo**

- En un fichero HTML con JavaScript 
- En un pen de codepen.io



### Los extras

El reto ya estaría finalizado, pero si quieres ir más allá tienes opciones:

1. Que salte confetti al acabar el contador (te recomiendo usar [confettijs](https://github.com/mathusummut/confetti.js))
2. Que el contador también muestre los milisegundos.
3. Añadir botón de empezar, parar y volver al inicio (resetear).



## Las míticas FAQ

Todas tus preguntas tienen respuesta.

(No, no te voy a dar el PIN de la tarjeta :P)





**¿En qué consiste?**

Propongo dos retos de programación sencillos para que podáis resolverlos de aquí al próximo 19 de Febrero.

Resolveré los dos en el directo que celebraremos ese día. 

Estás invitado a presentar tu solución al resto de participantes. Un momento ideal para salir de la zona del confort (sacar el culo de sofá, como digo yo) y hacerlo en una **comunidad coqueta y amistosa**.



**¿Cómo participo?**

Cada reto tiene un punto de partida y unos requisitos básicos.

Puedes hacerlo de forma individual o con otra *malandriner* de la comunidad. 



**¿De qué van los retos?**

Uno tiene que ver con estructuras de datos. Puedes resolverlo en cualquier lenguaje de programación.

El otro se centra en un widget con JavaScript para la web.



**¿Hay que hacer todos los retos con todos los extras?**

No, disfruta y llega hasta donde puedas. Lo importante es aprender y pasarlo bien.



**¿Qué son los extras?**

El reto está completo sin los extras. 

Pero si quieres seguir disfrutando, que no te falte motivación. Son requisitos añadidos que hacen más completo el reto.



**¿Qué gano participando?**

Primero, lo que vas a aprender. 

Segundo, insignias de la gamificación de la Zona Premium. 

Tercero, mi eterno agradecimiento. 

Cuarto, seguro que ganas un buen rato compartiendo tu experiencia con la comunidad.



Si tienes dudas, [pásate por aquí](https://www.danielprimo.io/contacto).
