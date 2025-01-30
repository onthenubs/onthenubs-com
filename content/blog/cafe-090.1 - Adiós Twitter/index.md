---
title: "☕️ #90.1 - ¿Cómo migrar de Twitter a Bluesky? Y borrar tus datos de Twitter por el camino"
slug: cafe-90-adios-twitter-migracion-bluesky
date: "2025-01-30T06:00:00+00:00"

programas: "Café OnTheNubs"
etiquetas:

cover:
  image: 'images/featured.webp'
  relative: true

youtube: 9H--W1zq8OM
---

Desde que Melon Ask compró Twitter (nos negamos a llamarle por su nombre de crisis de los 40) se ha visto una clara degradación del servicio. Tanto es así que los usuarios están abandonando en masa la red social.

En el episodio de hoy vemos cómo hemos llegado hasta aquí, y cómo migrar tu cuenta a Bluesky.

## Cómo la plaza del pueblo se convirtió en la cafetería del psiquiátrico

Nada más entrar por la puerta, Melon Ask [despidió a los moderadores](https://www.eleconomista.es/tecnologia/noticias/12101126/01/23/Twitter-continua-con-los-despidos-adios-a-los-moderadores-de-contenido-de-las-oficinas-internacionales-.html#), reemplazando su trabajo por unas notas de la comunidad que han sido inútiles para frenar tanto noticias falsas y como comportamientos tóxicos.

También [han priorizado a los suscriptores de Twitter Blue](https://owlead.com/is-twitter-blue-worth-it/) muy por encima del resto de usuarios, lo que se ha traducido en que o eres un usuario de pago, o el algoritmo te entierra y te hace invisible.

La nueva gestión de Twitter ha sido un goteo constante de decisiones en contra de sus usuarios y su comunidad. Como cuando [decidieron emplear los datos de todas sus cuentas para entrenar su nueva inteligencia artificial](https://es.wired.com/articulos/como-evitar-que-elon-musk-use-tus-tuits-de-x-para-entrenar-a-su-modelo-de-ia-grok).

Sin embargo, la gota que ha colmado el vaso ha sido [el apoyo de Melon Ask a la campaña presidencial republicana](https://elpais.com/internacional/elecciones-usa/2024-12-06/elon-musk-acabo-donando-mas-de-260-millones-de-dolares-a-la-campana-de-trump.html). Y es que se ha demostrado que [el algoritmo de Twitter fue modificado para potenciar las cuentas afines a Trump](https://www.publico.es/internacional/estudio-sugiere-musk-favorecio-cuentas-pro-trump-x-meses-elecciones-eeuu.html).

Twitter ha dejado de ser una red social, lo han convertido en una herramienta de manipulación en la que además hay un ambiente un poco turbio. Como resultado, tanto usuarios particulares como organizaciones están abandonando la red social en masa.

- [‘La Vanguardia’ sigue la estela de ‘The Guardian’ y abandona la red social X](https://elpais.com/comunicacion/2024-11-14/la-vanguardia-sigue-la-estela-de-the-guardian-y-abandona-la-red-social-x.html)
- [La Universidad de Sevilla y ahora el Ayuntamiento de Barcelona abandonan Twitter](https://computerhoy.20minutos.es/apps/adios-x-universidad-sevilla-ahora-ayuntamiento-barcelona-abandonan-twitter-pero-estampida-1438443)
- [Estos son los políticos que han abandonado la red social tras el 'saludo nazi' de Elon Musk.](https://www.20minutos.es/noticia/5674583/0/adios-x-estos-son-los-politicos-que-han-abandonado-red-social-tras-saludo-nazi-elon-musk/)
- [Medios, entidades y empresas abandonan X avivando el debate sobre la red social de Musk](https://www.eitb.eus/es/noticias/sociedad/detalle/9627804/varios-medios-entidades-y-empresas-abandonan-x-avivando-debate-sobre-red-social-de-musk/)


## Las alternativas

Por suerte contamos con dos redes sociales maduras que no solo sirven como alternativa a Twitter, si no que están diseñadas de tal forma que un asalto así nunca pueda ocurrir.

Estas redes son [Mastodon](http://que.pasa.co/@onthenubs) y [Bluesky](http://bsky.app/profile/onthenubs.com/), y ambas son redes sociales distribuídas que usan sus propios protocolos (ActivityPub y ATProto). Como vimos recientemente en el [Episodio 87]( {{< ref "../cafe-087 - SANS Hack Challenge + Es Bluesky descentralizado/index.md" >}} ), ATProto no es del todo distribuido. Pero sí es cierto que si un indeseable comprase Bluesky (la empresa), la comunidad lo tendría relativamente fácil para migrar fuera del servidor oficial y continuar sin él.

Entre estas dos alternativas, parece que los usuarios lo han tenido claro y han optado por Bluesky, que acaba de superar los 30 millones de usuarios registrados. (Estadísticas de [bsky.jazco.dev](https://bsky.jazco.dev/stats))

{{< figure src="images/bluesky-stats.webp" >}}


## 1. Migrando tus seguidores a Bluesky

Para encontrar en Bluesky a la gente que seguías en Twitter, puedes usar la extensión de chrome [Sky Follower Bridge](https://chromewebstore.google.com/detail/sky-follower-bridge/behhbpbpmailcnfbjagknjngnfdojpko).

Los pasos son:

1. Instala la extensión en tu navegador.
2. Genera un “App Password” en Bluesky (la extensión te guía en este proceso).
3. Configura la extensión con tu nombre de usuario en Bluesky y el “App Password”.
4. Navega hasta tu perfil de Twitter.
5. Ejecuta la extensión.

Sky Follower Bridge hará un procesado de fuerza bruta, analizando el código HTML de la página de Twitter para recuperar las cuentas que sigues. Luego utilizará varias estrategias para intentar encontrar a cada una de esas cuentas en Bluesky. Por ejemplo, buscando el mismo nombre de usuario, o buscando por nombre y apellidos.

Cuando Sky Follower Bridge termine de procesar, te ofrecerá una lista de cuentas que seguir. Revísala, porque suele encontrar varios falsos positivos.

Aunque esta herramienta no es perfecta, ya que siempre hay alguna cuenta que se le escapa, te elimina casi por completo la cansina tarea de volver a seguir a todas las cuentas que te interesan.


## 2. Borrando tu rastro de Twitter

Tus datos y publicaciones son oro para Twitter, seguramente los usen frecuentemente para entrenar a su inteligencia artificial. Por eso recomendamos eliminarlos.

¡Pero no vamos a eliminar nuestra cuenta! Y es que si eliminas una cuenta por completo, el nombre de usuario queda disponible a los pocos días. Cualquiera podría registrarse de nuevo con tu nombre de usuario y hacerse pasar por tí.

Vamos a usar [TweetXer](https://github.com/lucahammer/tweetXer), que es un script que es capaz de borrar una a una todas nuestras publicaciones, like, o seguidor.

El proceso es:

1. [Solicitar y descargar tu archivo de twitter](https://help.x.com/es/managing-your-account/how-to-download-your-x-archive). Pueden pasar hasta 24 horas entre que solicitas tu archivo y este está listo para descargar.
2. Copia el código del script de TweetXer.
3. Navega hasta tu perfil de twitter.
4. Abre el inspector.
5. Pega y ejecuta el código en la consola del inspector. Verás que aparece un panel nuevo en la interfaz de twitter.
6. Proporciona el archivo `tweet-headers.js` a esta nueva interfaz.
7. Déjale trabajar, se tomará su tiempo.
8. Cuando acabe, también puedes proporcionarle el archivo `like.js` para eliminar tus likes.
9. Por último, en opciones avanzadas puedes dejar de seguir a todas las cuentas a las que sigues.


## 3. ¿Re-subir tus publicaciones viejas a Bluesky?

Es posible recuperar tus viejos tweets en Bluesky. Por ejemplo, utilizando [twitter-to-bsky](https://github.com/ianklatzco/twitter-to-bsky), una herramienta escrita en python que lee las publicaciones en tu archivo de twitter, y las recrea en Bluesky.

¿Deberías hacerlo?

Hay opiniones en ambos sentidos, así que guíate por lo que te diga el corazón.

Por un lado esta herramienta ayuda a que tus publicaciones sigan estando disponibles al público.

Por otro lado, no va a ser una recreación perfecta. Por ejemplo las conversaciones solo van a contener tu parte, por lo que muchas publicaciones dejarán de tener sentido.

Nosotros hemos utilizado el cambio de red social para hacer borrón y cuenta nueva, dejando el pasado atrás. En nuestro caso, usamos las publicaciones para anunciar los directos o la publicación de un nuevo vídeo, por lo que esas viejas publicaciones tienen escaso valor. Es posible que en un futuro hagamos público nuestro archivo de twitter, en una web específica para ello, y que así podamos mantener viva la historia de nuestros comienzos.
