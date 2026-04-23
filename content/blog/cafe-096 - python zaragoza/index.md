---
title: '☕️ #96 Entrevista a Python Zaragoza'
slug: cafe-96-python-zaragoza
date: '2026-04-23T08:00:00+00:00'

programas: 'Café OnTheNubs'
etiquetas:

cover:
  image: 'images/featured.webp'
  relative: true

colaboradores:
  - lasdelpulpo
  - capitangolo
  - laura-alcober

# youtube:
---

Esta semana nos acompaña Laura Alcober de Python Zaragoza.

## Entrevista a Laura Alcober

Hemos estado de charleta con Laura, que además de trabajar en backend, es organizadora en la comunidad Python Zaragoza.

Nos ha contado cómo surgió la comunidad, qué eventos suelen organizar y cuál es su relación con Python España.

También hemos aprovechado para hablar del estado de Python, ahora que vuelve a estar en boga.

## Noticias de la semana

### El tozolón de la semana

La semana pasada Bluesky estuvo inaccesible a ratos.

Los primeros informes apuntaban a un ataque de denegación de servicio:

[Bluesky confirms DDoS attack is cause of continued app outages](https://techcrunch.com/2026/04/17/its-not-just-you-bluesky-is-sorta-down/)

Aunque la realidad parece ser diferente. Fue un problema en como gestionan memcache con Scylla, su base de datos. Cada vez que un dato no se encuentra en memcached, y se consulta en la base de datos, se abre un puerto nuevo. Una nueva funcionalidad lanzaba rachas de 10-20 consultas por segundo, agotando los puertos disponibles.

Fue un error difícil de depurar, ya que este error destapó otro problema en el sistema de logging. Cada vez que tienen un error de memcached, lo logean asíncronamente abriendo un nuevo hilo. Las rachas de miles de errores pusieron presión extra sobre el recolector de basura de go.

Por tanto, tenían dos errores juntos: Se quedaban sin puertos y sin memoria.

Por eso el sistema funcinaba a ratos. Poco a poco se quedaban sin memoria y Bluesky empezaba a ir lento. Llegado un momento límite, el sistema mataba los procesos y lo reiniciaba. Y vuelta a empezar.

[April 2026 Outage Post-Mortem](https://pckt.blog/b/jcalabro/april-2026-outage-post-mortem-219ebg2)

### IA IA OH!

La semana pasada hablábamos de un robot policía, lo que no comentamos es que… ¡Persigue jabalíes!

[El robot que persigue a los jabalíes en Polonia tiene nombre, es 'influencer' y toda una celebridad en el país](https://www.20minutos.es/gonzoo/robot-que-persigue-los-jabalies-polonia-tiene-nombre-es-influencer-toda-una-celebridad-pais_6958603_0.html)

Los datos son oro para las empresas de IA:

[Failed Companies Are Selling Old Slack Chats and Email Archives to Train AI](https://gizmodo.com/failed-companies-are-selling-old-slack-chats-and-email-archives-to-train-ai-2000747916)

Antrhopic no para de lanzar cosas nuevas:

[Introducing Claude Design by Anthropic Labs](https://www.youtube.com/watch?v=t_LBECIQQqs)

También han sacado una movida que te busca bugs en el código:

[New in Claude Code: /ultrareview](https://x.com/ClaudeDevs/status/2046999435239133246?s=20)

La hipocresía se huele a distancia:

{{< figure src="./images/doraemon-chatgpt.webp" >}}

Esto del token maxxing se va de las manos:

[CEO obsessed with token maxxing](https://x.com/mytechceoo/status/2046664705176187180?s=20)

Han hecho una movida que le pone voz a Claude Code. En concreto, la del peón de Warcraft.

[PeonPing en GitHub](https://github.com/PeonPing/peon-ping)

Aquí puedes verlo en acción:

[PeonPing.com](https://www.peonping.com)

ChatGPT al verme llegar de nuevo porque se me acabaron los tokens con Claude:

[Vídeo](https://scontent-muc2-1.cdninstagram.com/o1/v/t2/f2/m86/AQOJFjpWHhbtWxvNeK290QHWm5OGJpodUENfig1N4S2nC6o_Q00u2H-rj5tUfDu8rsWVogcisS6L2EJSUQ7SFF0AYiiBZWqCMOciCms.mp4?_nc_cat=108&_nc_sid=5e9851&_nc_ht=scontent-muc2-1.cdninstagram.com&_nc_ohc=qwTLBEIlCv4Q7kNvwHaTWAL&efg=eyJ2ZW5jb2RlX3RhZyI6Inhwdl9wcm9ncmVzc2l2ZS5JTlNUQUdSQU0uQ0xJUFMuQzMuNzIwLmRhc2hfYmFzZWxpbmVfMV92MSIsInhwdl9hc3NldF9pZCI6MTc4NjQ2MTk5OTk2NzMzOTQsImFzc2V0X2FnZV9kYXlzIjo3LCJ2aV91c2VjYXNlX2lkIjoxMDA5OSwiZHVyYXRpb25fcyI6NywidXJsZ2VuX3NvdXJjZSI6Ind3dyJ9&ccb=17-1&vs=b6d2bcd190ca4d27&_nc_vs=HBksFQIYUmlnX3hwdl9yZWVsc19wZXJtYW5lbnRfc3JfcHJvZC8yQzQ4QkYwNjdGRTdENjVBMTE4N0VGNjJBMTQxQzA5MF92aWRlb19kYXNoaW5pdC5tcDQVAALIARIAFQIYUWlnX3hwdl9wbGFjZW1lbnRfcGVybWFuZW50X3YyLzc1NEQwRkQ4NEMxRDU5NEE0QTQ2QkVBMTkwQTJCMkI0X2F1ZGlvX2Rhc2hpbml0Lm1wNBUCAsgBEgAoABgAGwKIB3VzZV9vaWwBMRJwcm9ncmVzc2l2ZV9yZWNpcGUBMRUAACbk8IWS3_G7PxUCKAJDMywXQB12yLQ5WBAYEmRhc2hfYmFzZWxpbmVfMV92MREAdf4HZeadAQA&_nc_gid=xKqH4BM1CjUJ5-ly7VAJ4g&_nc_zt=28&_nc_ss=7a22e&oh=00_Af1-yzTP_dwaFx0ozEbrYdmtTkw30b7hfoDezgmp4HLfug&oe=69EB7CFD)

### Ciberseguridad

La verificación de edad es un peligro para la ciberseguridad:

[Pillan a la app de verificación de edad de la UE proporcionando a la Policía todos los datos personales que almacena](https://www.adslzone.net/noticias/internet/app-verificacion-edad-ue-datos-sensibles/)

Timos de criptomonedas en el estrecho de Hormuz

[Fraud in the strait?: How crypto scamsters are targeting ships stuck in Hormuz](https://www.businesstoday.in/technology/story/fraud-in-the-strait-how-crypto-scamsters-are-targeting-ships-stuck-in-hormuz-526705-2026-04-21?utm_source=rssfeed)
