---
title: "☕️ #90.2 - Crónica de Bilbostack '25"
slug: cafe-90-cronica-bilbostack-2025
date: "2025-01-31T08:00:00+00:00"

programas: "Café OnTheNubs"
etiquetas:

cover:
  image: 'images/featured.webp'
  relative: true

colaboradores:
  - capitangolo
  - laura mosteiro
  - lasdelpulpo

youtube: 49ycmXrtNtI
---

Como [comentábamos a principios de mes](https://www.notion.so/89-Entrevista-a-Bilbostack-16f6a5a67719802cb10ac080fb02e8dd?pvs=21), [Bilbostack](https://bilbostack.com/) es una conferencia anual sobre tecnología que se celebra en Bilbao. Este año ha tenido lugar el 25 de enero en el Palacio Euskalduna.

{{< figure src="images/bilbostack-logo-permalink.webp" >}}


## Edición de 2025

Otro año más, hemos visitamos la capital del Nervión para asistir a este evento tecnológico. Y, como nos tienen acostumbrados, el nivel de las ponencias y la organización ha sido altísimo.

{{< figure src="images/bilbostack-palacio-eusaklduna.webp" >}}

Como nota general, han abundado las referencias culturales a Elon Musk, Twitter y el nuevo gobierno de Trump, para deleite del público 🙂.

El formato fue muy parecido al que ya quedó establecido hace dos ediciones, a saber:

- Dos *tracks* con 4 charlas cada uno en horario de 9:30 a 14:00.
- *Txosnas* bajo el Puente Euskalduna + sidra y paella gratis.
- Juegos populares vascos.
- Concierto popular.

Fue todo un detalle que la acreditación incorporara el horario (y que estuviera hecha de algodón reciclado):

{{< figure src="images/bilbostack-tracks.webp" >}}

Puede parecer chocante el realizar actividades debajo de un puente, pero es una solución ideal para estar al aire libre y a resguardo de la lluvia:

{{< figure src="images/bilbostack-puente.webp" >}}

Este año la parte de deportes tradicionales se cubrió con una exhibición de [*aizkolaritza*](https://es.wikipedia.org/wiki/Aizcolari), deporte que trata de cortar troncos con hachas. Nos mostraron dos tipos de competiciones: Al menor número de cortes necesarios para atravesar un tronco, y a ver quién partía antes cuatro troncos. Fue interesante cómo los nudos en la madera del tronco cambiaban el podium totalmente, pudiendo retrasar al *aizkolari* que estuviera en cabeza hasta el último puesto.

La narración que acompañaba a la demonstración rebosaba mucho cariño, se nota el orgullo que tienen los vascos por sus tradiciones y lo feliz que les hace darlas a conocer.

{{< figure src="images/bilbostack-deportes.webp" >}}


## ¿Qué nos llamó la atención de cada charla?

Si algo tuvieron en común las charlas, es que los ponentes eran *top-tier*, trataron temas muy interesantes, y dieron un montón de información.

A continuación hemos querido reseñar y compartir algunas ideas que resonaron especialmente con nosotros, dentro de aquellas charlas a las que pudimos atender.


### [**El Boom de la IA Generativa - Nerea Luis Mingueza**](https://bilbostack.com/speakers/nerea-luis/#talk)

Nos dio la impresión de que Nerea venía del futuro. Nos puso al día en el estado del arte de la inteligencia artificial, dejando a un lado la burbuja en la que vivimos y centrándose en una gran cantidad de casos de uso para los que la inteligencia artificial de verdad está marcando una diferencia.

Por ejemplo, gemelos digitales para hacer investigación sobre el cambio climático o genética; actores multi idioma, para que una persona pueda hablar varios lenguajes; herramientas para hacer prototipos; o inteligencias artificiales que son capaces de procesar y correlacionar grandes cantidades de datos para hacer resúmenes y esquemas.

Aparte de repasar los nuevos avances, también dedicó tiempo a hablar de otros temas de los que se habla menos, pero son igual de importantes. Como por ejemplo la responsabilidad de los datos, o la seguridad.

Nerea terminó la charla con la pregunta: ¿Cuánto va a valer nuestro trabajo? Si la inteligencia artificial hace nuestro trabajo, ¿qué hacemos nosotros?


### [Bases de Datos en Memoria - Katia Aresti](https://bilbostack.com/speakers/katia-aresti/#talk)

Katia dio un repaso muy completo de los casos de uso de las bases de datos en memoria, que se usan habitualmente para *cachear* tuplas de clave-valor de tal forma que luego se puedan consultar a gran velocidad.

También explicó que o bien para acercar los datos a las réplicas de las aplicaciones, o para garantizar alta disponibilidad, lo normal es desplegar estas bases de datos de manera distribuida. De tal forma que la misma información esté siempre disponible en al menos dos nodos del cluster.

Agradecimos mucho, que aunque hacía muchas referencias a *Infinispan*, el proyecto en el que ella trabaja, también hacía muchas comparativas con otras soluciones populares, y todos los conceptos que explicaba eran aplicables de manera genérica a cualquier solución.


### [¡El Futuro de la Web! - Miguel Ángel Durán García (**midudev)**](https://bilbostack.com/speakers/miguel-angel-duran/#talk)

Somos muy fans de los tutoriales miudev en YouTube y del arte que tiene para explicar conceptos de programación. Nos encanta lo efectivo que es remarcando los conceptos importantes y con los ejemplos prácticos que presenta. Por lo que teníamos muchas ganas de atender a esta charla.

Miguel empezó rompiéndonos los esquemas. Presentó unos cuantos problemas web que estamos acostumbrados a solucionar con javascript (a veces de manera un poco guarrilla), para luego enseñarnos que hoy en día se pueden solucionar sin necesitar nada más que  HTML. Y es que los navegadores están evolucionando continuamente para que el desarrollo web sea cada vez sea más fácil, además se coordinan para implementar las mismas mejoras a la vez.

Nos quedamos con la sensación de estar viendo a un mago, boquiabiertos cada vez que enseñaba algo.

Remarcó varias cosas que él creía que iban a marcar una diferencia en el desarrollo web.

Por ejemplo, transiciones entre páginas web al estilo de “Magic Move” de Keynote. Si una imagen está presente en la página inicial y la página destino, automáticamente se anima la posición y escala de esa imagen.

O la propuesta de que todas las funcionalidades nuevas de javascript se desarrollen en TypeScript, y que ese código se transpile en un Javascript Sugar mucho más ligero que es el que ejecuten los navegadores web. De esa forma los desarrolladores podrían programar en un lenguaje más potente, ahorrando esfuerzo a los navegadores que solo tendrían que mantener un motor de javascript mucho más ligero.

Por último comentó cómo era posible usar las APIs de WebGL (que dan a las páginas web acceso de bajo nivel a las tarjetas gráficas) para ejecutar modelos de inteligencia artificial, y cómo proyectos como DeepSeek lo estaban utilizando para reducir inmensamente los gastos de servidores en la nube.


### [10 años al mando de […] Platonic Games - Valeria Castro](https://bilbostack.com/speakers/valeria-castro/#talk)

En esta charla Valeria compartió con nosotros su historia y aprendizaje al mando de Platonic Games. Desde el punto de vista de haber montado una empresa de videojuegos, nos contó qué cosas no repetiría de su experiencia. En concreto, nos dio diez consejos que sorprendían por su honestidad.

Nos llamó la atención el tema de los salarios. Cómo empezaron queriendo ofrecer el mismo salario a todos los trabajadores, que es algo que suena muy bonito, pero luego generó problemas cuando los seniors veían que los recién contratados cobraban lo mismo que ellos.

O por ejemplo cómo el saber demasiado de la vida personal de tus empleados puede llegar a abrumarnos. Comentándolo entre nosotros, coincidíamos en que como *managers* nos era útil tener esa información para poder adaptarnos mejor a las situaciones personales de nuestro equipo. También nos sorprendíamos de nuestra ingenuidad, al no ver que cuando se trata de equipos grandes el involucrarnos tanto puede suponer una sobrecarga emocional que nos afecte considerablemente.


### [Cuando los robots aprenden a hablar - Fernando Díaz Garrido](https://bilbostack.com/speakers/fernando-diaz/#talk)

Esta charla fue una iniciación perfecta a el mundo de Tecnología Operativa (OT), que es la informática que se usa en una línea de producción industrial. Esto incluye, sensores, robots, códigos de barra, y un sinfín de equipos informáticos especializados.

Poniendo como ejemplo una fábrica de inyección de plástico, Fernando nos explicó los componentes de una planta industrial. Y nos presentó el problema que le pidieron solucionar en ella: Unas máquinas que se atascaban periódicamente, y cuyo arreglo costaba miles de euros.

Se centró en los sensores que recogen datos de la maquinaria, como temperatura, presión, etc. Y nos fue contando paso a paso el camino para correlacionar esos datos y convertirlos en conocimiento útil. En su ejemplo, consiguieron identificar que una diferencia de temperatura mayor de 10ºC entre dos zonas de la maquinaria era la causa de los atascos.

El momento “WOW, no se me habría ocurrido antes”, vino cuando explicó que restar dos cifras para obtener la diferencia de temperatura a lo largo del tiempo no era nada sencillo. Y es que las muestras de temperatura de cada sensor no se toman en el mismo instante, si no con un pequeño margen, y para complicar las cosas a veces falta alguna muestra en la línea temporal. Así que las matemáticas para hacer un cálculo aparentemente tan sencillo acaban siendo bastante complicadas.


### El resto de charlas

No pudimos atender a todas las charlas, y fue una pena porque solo escuchamos cosas buenas de todos los ponentes. Estas son esas charlas que nos perdimos:

- [Y si “hacer lo correcto” no fuera lo correcto - Jordi Martí Carrera](https://bilbostack.com/speakers/jordi-marti/#talk)
- [Fatal, gracias - Irene M Morgado](https://bilbostack.com/speakers/irene-morgado/#talk)
- [Culture Driven Development - Sebi Collell](https://bilbostack.com/speakers/sebi-collell/#talk)
