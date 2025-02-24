---
title: "☕️ #91 - Robando credenciales cloud para hablar con IAs calientes"
slug: cafe-91-robando-credenciales-nsfw
date: "2025-02-13T08:00:00+00:00"

programas: "Café OnTheNubs"
etiquetas:

cover:
  image: 'images/featured.webp'
  relative: true

colaboradores:
  - capitangolo
  - miguel

youtube: WgXt39dx09Q
---
En el episodio de hoy, [Miguel Hernández]({{< ref "miguel">}}), nos descubre una nueva tendencia que consiste en robar credenciales de servicios *cloud* y sobre los que ejecutar inteligencias artificiales. En concreto, *chat bots* de temáticas sexuales o bizarras.


## Robo de credenciales

En el pasado hemos comentado lo lucrativo que es el robo de credenciales de servicios en la nube. Lo vimos, por ejemplo, con el caso de [EmeraldWhale](https://sysdig.com/blog/emeraldwhale/), una operación que había robado 15.000 credenciales.

{{< figure src="images/01-emeraldwhale-attack-chain.webp" alt="Attack chain of emeraldwhale">}}

Hasta ahora habíamos visto que los objetivos más comunes de estos ataques eran:

- Usar los recursos de las cuentas comprometidas para minar criptomonedas. ([Labrat](https://sysdig.com/blog/labrat-cryptojacking-proxyjacking-campaign/))
- Robar información sensible o sabotear la infraestructura.

Lo que estamos viendo ahora es el uso de estos credenciales para ejecutar modelos de inteligencia artificial:

- [LLMjacking: Stolen Cloud Credentials Used in New AI Attack](https://sysdig.com/blog/llmjacking-stolen-cloud-credentials-used-in-new-ai-attack/)
- [The Growing Dangers of LLMjacking: Evolving Tactics and Evading Sanctions](https://sysdig.com/blog/growing-dangers-of-llmjacking/)

LLMjacking ha sido registrado en MITRE ATT&CK como parte de “[Resource Hijacking: Cloud Service Hijacking](https://attack.mitre.org/techniques/T1496/004/)”. 


## Explotación a través de proxies

Lo interesante es que estos sistemas comprometidos no siempre son explotados directamente. Los atacantes a menudo mantienen proxies que son utilizados por terceros. Estos proxies pueden ser totalmente abiertos, o necesitar registro, y pueden ser gratis o de pago.

**Nota:** no todos los proxies OpenAI son maliciosos.

{{< figure src="images/02-llmjacking-attack.webp" alt="Attack chain of emeraldwhale">}}


## El bizarro mundo de los chatbots

Lo que nos lleva a lo que Miguel y su equipo han estado investigando últimamente ([LLMjacking targets DeepSeek](https://sysdig.com/blog/llmjacking-targets-deepseek/)). Comunidades que utilizan estos credenciales robados y estos proxies para hablar con chatbots.

Los objetivos de los miembros en estas comunidades pueden ser varios:

- Están adictos a hablar con inteligencias artificiales y no pueden pagar el coste.
- Quieren usar las inteligencias artificiales de modos no soportados (sexo, por ejemplo), y les echan de los servicios oficiales.
- Les gusta poner a prueba a las inteligencias artificiales, ver cómo las pueden romper, y compartir sus éxitos con otros.

En el episodio de hoy, Miguel nos enseña cómo se coordinan estas comunidades a través de 4chan y Discord. Cómo comparten las credenciales de los proxies, y los sitios en los que se pueden compartir modelos de los chatbots.
