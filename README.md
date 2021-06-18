# LiveChallenge #2: ¡Ven a la FiestAPI!

> La vida es un reto.
> 
> El código también.
> 
> Participa con el resto de malandriners en un reto de programación que no conoce la zona de confort.

## ¿De qué va esto?

Se proponen tres retos de programación que hay que resolver en un tiempo límite.

Cada reto suma una puntuación que será tenida en cuenta en el LiveChallenge en directo donde se podrán presentar las propuestas.

El reto está abierto a cualquier suscriptor/a activo de la Zona Premium de danielprimo.io.

Al final tienes las FAQ con todos los detalles concretos.

La fecha final de entrega es el 25 de Junio a las 18:00.

## ¿Cuál es el reto técnico?

Vamos a trabajar con una API, un sistema externo que nos devuelve una información cuando se la pedimos.

Usaremos una API abierta de la de la empresa TMB. Nos ofrece todo tipo de información de los transportes del área metropolitana de Barcelona. Es el mundo real, con sus líneas, recorridos, tiempos y rutas.

Nada de API de Chuck Norris ni de Chiquito. Aquí queremos ver cosas de verdad.

La TMB tiene un portal para developers donde puedes darte de alta gratuitamente para conseguir tu API Key.

[Acceso al portal de developers](https://developer.tmb.cat/)

↗️ [Vídeo explicando el proceso](https://premium.danielprimo.io/cursos/leyendo-codigo/asi-se-comienza-a-consumir-una-api)

Este es un ejemplo muy sencillo de cómo conectarse de forma correcta, puedes lanzarlo en la consola del navegador. Verás como la respuesta coincide con la descripción de este recurso en la [documentación](https://developer.tmb.cat/api-docs/v1/transit#operation/parades_linia).

```javascript
let api_url = "https://api.tmb.cat/v1/transit/linies/bus/213/parades?app_id=TU_API_ID&app_key=TU_API_KEY"

fetch(
  api_url
).then(
  res => res.json()
).then(
  console.log
)
```

Nota: No usaremos el material que se descarga, solo serán válidos los retos presentados contra la API.

## Reto 1: Listado de líneas de metro y estaciones

El reto consiste en mostrar en pantalla un selector con todas las líneas de Metro activas de la TMB.

Una vez seleccionada una línea debes mostrar el listado de los nombres de paradas de esa línea.

Al cambiar de opción en el selector, se renueva el listado de paradas.

**Pista**: [Aquí](https://developer.tmb.cat/api-docs/v1/transit#operation/parades_linia).

**Cómo hacerlo**

*   Cualquier lenguaje de programación es válido. En la captura ves una solución con LeafletJS, JavaScript, HTML y CSS.

**Ejemplo visual**

![](https://user-images.githubusercontent.com/1122071/121817873-50e70980-cc84-11eb-8a80-4f72bfc3633e.gif)

🏆 Este reto sumará 1 punto si es presentado correctamente.

## Reto 2: Líneas en el mapa

Tenemos un selector de líneas de Metro disponibles para la TMB.

Al elegir una de ellas debe pintarse la ruta en el mapa.

**Pista**: Ten en cuenta que en el resultado de la API en cada petición de línea devuelve algo que es compatible con un formato de datos que reconocen muchos mapas.

**Mapas de Leaflet**

Usaremos Leaflet como referente para crear los mapas.

Tenemos un [curso completo](https://premium.danielprimo.io/cursos/leafletjs) en la Zona Premium donde podrás ver las bases de este sistema.

Puedes resolverlo también con Google Maps o cualquier otro proveedor que permita trabajar con mapas para la web.

**Cómo hacerlo**

*   Cualquier lenguaje de programación es válido. En la captura ves una solución con LeafletJS, JavaScript, HTML y CSS.

**Ejemplo visual**

![](https://user-images.githubusercontent.com/1122071/121818140-b12a7b00-cc85-11eb-94f8-21edc85993f7.gif)

🏆 Este reto sumará 1 punto si es presentado correctamente.

## Reto 3: Paradas de Bus y tiempo de espera

Crearemos un mapa con una caja de texto donde podremos introducir el código de una parada del bus.

Al terminar de completar el código debe pintarse en el mapa la localización de la parada y mostrar información en pantalla de cuánto tiempo falta para que lleguen los próximos buses.

**Pista**: La información de las paradas se consigue del servicio "Transit" de la API de la TMB. La del tiempo de espera del servicio "iBus" de la API de la TMB.

**Cómo hacerlo**

*   Cualquier lenguaje de programación es válido. En la captura ves una solución con LeafletJS, JavaScript, HTML y CSS.

**Ejemplo visual**

![](https://user-images.githubusercontent.com/1122071/121818057-40835e80-cc85-11eb-9756-23a45f891bb0.gif)

🏆 Este reto sumará 2 puntazos si es presentado correctamente.

## LiveChallenge en directo con premios

Las propuestas podrán presentarse en directo el 25 de Junio.

🏆 Si se presenta el código en directo se sumará 1 punto.

Se sortearán tres cheques regalo de Amazon entre los participantes. Cada punto es un boleto en el sorteo.

➡️ Para participar debes enviar tus propuestas de solución en [este formulario](https://forms.gle/gFyYpstdtCZyPTj59) antes de las 17:00 horas (horario de Madrid) del 25 de Junio de 2021.

# Las míticas FAQ

Todas tus preguntas tienen respuesta.

**¿Quién puede participar?**

Suscriptores en activo a la Zona Premium de danielprimo.io.

**¿En qué consiste?**

Propongo tres retos de programación que se resolverán en directo.

Estás invitado a presentar tu solución al resto de participantes. Un momento ideal para salir de la zona del confort (zona del sofá) y hacerlo en una **comunidad coqueta y amistosa**.

**¿Cómo participo?**

Cada reto tiene un punto de partida y unos requisitos básicos. Debes enviar tus soluciones a  [este formulario](https://forms.gle/gFyYpstdtCZyPTj59) antes de las 17:00 horas (horario de Madrid) del 25 de Junio de 2021.

**¿De qué van los retos?**

Queremos mejorar en el manejo de dos tecnologías esenciales para entender la web moderna: las API y los mapas.

**¿Hay que hacer todos los retos?**

No. Puedes quedarte con el primero, o solo con el segundo o con el tercero o con varias combinaciones.

Los puntos te dan oportunidades a ganar el premio en la sesión en directo.

**¿Cómo funciona el sistema de puntos?**

El reto 1 y el reto 2 suman 1 punto cada uno.

El reto 3 suma 2 puntos.

Las soluciones deben ser correctas para sumar esa puntuación.

Se suma 1 punto más si presentas la solución de los retos que tengas realizados en la sesión en directo del 25 de Junio.

**¿Qué gano participando?**

Primero, lo que vas a aprender.

Segundo, insignias de la gamificación de la Zona Premium.

Tercero, seguro que ganas un buen rato compartiendo tu experiencia con la comunidad.

Cuarto, la posibilidad de ganar un cheque regalo de Amazon. Se sortearán 3 de 25€ cada uno entre los participantes. Cuantos más puntos, más posibilidades de que te toque el cheque.

Un premio por persona.

**¿Qué pasará con las soluciones?**

Serán publicadas en la web para ocio y disfrute de la comunidad y el resto del mundo. Esto no es obligatorio, claro.

**¿Qué es una API?**

En [YouTube](https://www.youtube.com/watch?v=QsrWtqnQGMc) respondo a la pregunta.

Para probar la API también puede interesarte las 3 primeras lecciones del curso de [Pruebas y diseño de APIs con Postman](https://premium.danielprimo.io/cursos/postman).

Aunque en el reto no es necesario, puedes ver como rreamos una en el curso [Crea una API REST artesana con PHP](https://premium.danielprimo.io/cursos/crea-una-api-rest-artesana-con-php).

## Recursos

*   [Documentación de la API de TMB](https://developer.tmb.cat/api-docs/v1)
*   [Curso de LeafletJS](https://premium.danielprimo.io/cursos/leafletjs)

Cualquier duda, sabes donde encontrarme. Dani.
