---
title: "☕️ #88 - Crónica de Codemotion Mulesoft + Hackeo de AEAT + Investigando los visitantes a la isla Epstein"
slug: cafe-88-codemotion-mulesoft-aeat-epstein
date: "2024-12-03T08:00:00+00:00"

programas: "Café OnTheNubs"
etiquetas:

colaboradores:
 - capitangolo
 - melocopon

cover:
  image: 'images/featured.webp'
  relative: true

youtube: RI9TH5Z70lM
---


## Codemotion + MuleSoft Barcelona

[Miriam](https://hachyderm.io/@melocopon) estuvo la semana pasada por el evento “[#CodeMeet Barcelona: Qui no té tecnologia, el gat pentina](https://community.codemotion.com/codemotion-espana/meetups/codemeet-barcelona-qui-no-t-tecnologia-el-gat-pentina)” y nos cuenta su experiencia.

{{< figure src="images/01-evento.webp" >}}


### ¿De qué va el evento?

Codemotion es una comunidad y plataforma para dar charlas de innovación en la informática.

En este caso el título era “Qui no té tecnologia, el gat pentina”, que viene a decir algo como “Quien no tiene tecnología, el gato peina (se está perdiendo algo)”. Y el evento estuvo formado for cinco charlas.

Un agradecimiento enorme a [Natalia de Pablo](https://www.linkedin.com/in/nataliadepablo/), CM de Codemotion, por animarnos a acudir al evento.


### ¿Qué es MuleSoft?

[MuleSoft](https://www.mulesoft.com), un producto de Salesforce, es un puente, un puente, una plataforma que unifica varias tecnologías a nivel de Business Intelligence y utiliza IA para facilitar la gestión de APIs.

{{< figure src="images/02-mulesoft.webp" >}}


### ¿De qué se habló?

Las dos primeras fueron más técnicas y hablaban de desarrollo de APIs:

En **Prácticas para User-First API Designa**, ****Angel Paredes hablaba de cómo hacer la vida más fácil al desarrollador creando APIs que fueran fáciles de usar, y que luego retornara en una aplicación que funcionara mejor y los usuarios estén más contentos con ella. Comentaban, por ejemplo, que usar *streaming* en el API hace que las aplicaciones se sientan más fluidas.

En **Gobernanza de APIs**, Mark Boyd profundizó en cómo hacer que varias APIs sigan las mismas guías y mejores prácticas de tal forma que los desarrolladores lo tengan más fácil para usarlas. Se incidió en la necesidad de documentar, y en hacer un desarrollo continuo que no se centre solo en funcionalidades nuevas, si no también en mantener el código legacy.

Poco a poco las charlas se fueron centrando más en el negocio.

En **¿Por qué la Liga de la Justicia no necesita MuleSoft?**, Jorge Lebrato hablaba de qué es MuleSoft, y qué no es, y cómo se aplica a nivel de negocio y en cada departamento. Llamó la atención cómo se hizo amena con multiples referencias a cómics.

{{< figure src="images/03-ligadelajusticia.webp" >}}

Las dos siguientes charlas, **Construye tu producto digital y mantenlo a salvo de ataques** (Sergio Acebes) y **Impulsando la estrategia de datos en B2B** (Laura Marqués) hablaban de cómo construir un producto, y cómo recoger datos de tu producto para utilizarlos en mejorarlo.

En la última charla, **Rompiendo Códigos: Inclusión y Talento Femenino en el sector Tech**, Noelia Torres nos presentó la ONG Factoria F5 que ayuda a personas en situaciones de potencial exclusión social, y explicó formas de poder colaborar con ellos.


### ¿Qué te llamó la atención?

Miriam nos comenta que se quedó mas con las dos primeras charlas. En un momento en el que está “comenzando” con la programación, los conceptos de pensar a largo plazo y seguir buenas prácticas marcan un camino muy interesante para mejorar sus habilidades.

Para alguien que viene del mundo de sistemas, fue muy interesante ver otros tipos de enfoques que se le da a la tecnología.

También fue una experiencia muy positiva participar en una comunidad con gente tan maja. Fue muy bonito ver gente con una mentalidad abierta a aprender y mejorar.


## Noticias


### [Bruselas expedienta a España y una veintena de países por no reforzar la ciberseguridad en sectores críticos](https://www.elmundo.es/economia/2024/11/28/674898fefdddff27088b457a.html)

En Octubre tendría que haber salido la ley Española que adaptaba la [directiva Europea de seguridad NIS2](https://safetybits.io/es/blog/nis2-afectara-industria-europea-european-industries/). Una directiva que quiere hacer a Europa más resistente frente a ciberataques, y que obliga a aquellas empresas claves a implementar ciertas medidas de ciberseguridad.

Al haber incumplido el plazo, a España y a otros veinte paises el plazo se les ha abierto un expediente que puede acabar en sanciones.

Lo que sí sabemos es que en España las medidas que van a tener que tomar las empresas van a estar basadas en el [Esquema Nacional de Seguridad](https://ens.ccn.cni.es/es/que-es-el-ens), por lo que no tienes que esperar a que se publique la ley para empezar a implementar la NIS2.


### [Hemos seguido a todos los visitantes de la isla Epstein](https://www.youtube.com/watch?si=1vug-gDZmL4AJAW3&v=PjPHq-Ez0nc&feature=youtu.be)

Wired ha lanzado un reportaje de investigación en el que han seguido a todas las personas que han visitado la isla de Jeffrey Epstein, en la que se celebraban bacanales con menores de edad.

Near Intelligence, ahora conocida como [Azira](https://azira.com), recogió información de unos 200 teléfonos que visitaron la isla. Lo interesante es cómo se han obtenido esos datos, a través de una filtración de un *data-broker**.*** 

Muchas aplicaciones y plataformas de publicidad recogen nuestra información para ofrecernos publicidad personalizada. Mucha de esta información está geolocalizada, por lo que es posible seguir los movimientos de una persona. Los *data-brokers* se dedican a recopilar y vender información desde varias fuentes, y a veces esta información es vendida a servicios de inteligencia.

También es posible que parte de esta información se haya obtenido a través de la red de gestión de los teléfonos móviles. En un vídeo reciente de veritasium, demonstraban lo fácil que es clonar un teléfono móvil para hacerse pasar por otra persona:

{{< youtube wVyu7NB7W6Y >}}


### [Stop Using Predictable Bucket Names: A Failed Attempt at Hacking Satellites](https://www.securityrunners.io/post/stop-using-predictable-bucket-names-a-failed-attempt-at-hacking-satellites)

En este artículo se explica cómo los servicios en la nube utilizan nombres predecibles en muchos lugares, y cómo los hackers pueden aprovecharlo.

Por ejemplo, un hacker que consiga acceso a un sistema puede crear un Bucket S3 con la estructura de nombre de una región de AWS que todavía no exista. Cuando se cree esa región cabe la posibilidad de que el código de ese bucket se ejecute. (Lo hemos resumido mucho, mejor leed el artículo)


## Tozolón de la semana - El hackeo de la Agencia Tributaria

Nos levantamos esta semana con la noticia de que habían robado 560GB de datos a la Agencia tributaria:

- [El Confidencial](https://www.elconfidencial.com/tecnologia/2024-12-01/agencia-tributaria-aeat-trinity-ransomware_4014867/)
- [La Vanguardia](https://www.lavanguardia.com/andro4all/tecnologia/un-grupo-de-hackers-exige-38-millones-de-euros-por-el-rescate-de-560-gb-de-informacion-de-hacienda)
- [Newtral](https://www.newtral.es/hackeo-agencia-tributaria/20241201/)

El historial del grupo de *hackers* Trinity hace creer de que se trata de un hackeo real, aunque la Agencia Tributaria insiste en que no han hallado indicios de que su seguridad se haya visto comprometida.

Se sospecha que los hackers han podido acceder a través de alguna administración (como un ayuntamiento) con acceso a la red de la Agencia Tributaria. Algo parecido a lo que pasó con [el hackeo a través del poder judicial](https://facua.org/noticias/un-hackeo-a-traves-del-poder-judicial-roba-a-hacienda-datos-de-medio-millon-de-contribuyentes/) hace un par de años.

**Actualización:** El hecho de que Trinity no haya contactado con AEAT (entre otros motivos) señala a que los datos pertenezcan a una gestoría privada. Más información en esta publicación de Ramón Carlos Rico, ingeniero de ciberseguridad: [Caso AEAT… ¿O quizá no?](https://www.linkedin.com/feed/update/urn:li:activity:7270193874331959298/).
