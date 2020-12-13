---
title: Reproductor de música ligero
date: "2020-12-05T22:12:03.284Z"
spoiler: "Si estas usando una distribución de Linux sabrás que no hay tantos reproductores de música disponibles como nos gustaría."
cta: "react"
discussionId: "2020-12-05-page-slug"
---

Si estas usando una distribución de Linux sabrás que no hay tantos reproductores de música disponibles como nos gustaría. Yo quería encontrar un reproductor que cumpla con las siguientes características:

- Que tenga soporte de _bit-perfect_
- Que tenga soporte a una gran cantidad de _códecs_ de audio.
- Que sea personalizable.
- Que sea rápido

### ¿Para qué soporte a [_bit-perfect_](https://it.wikipedia.org/wiki/BitPerfect)?
El _bit-perfect_ es muy importante para mí que soy un entusiasta de la calidad del sonido, normalmente uso [DACs](https://es.wikipedia.org/wiki/Conversor_de_se%C3%B1al_digital_a_anal%C3%B3gica) externos que deben recibir una señal limpia para sacar su máximo provecho.

Un sistema operativo como Linux tiende a montar internamente un mezclador que se encarga de tomar todas las señales de audio, mezclarlas para luego pasarlas a los altavoces o audífonos. Por esta razón, puedes ver vides en YouTube, escuchar música en Spotify, escuchar la notificación de Telegram, todo al mismo tiempo.

Esto es muy útil, pero cuando se trata de sacar el máximo provecho a cada bit de información que contiene [archivos sin pérdida](https://es.wikipedia.org/wiki/Formato_de_archivo_de_audio#:~:text=Hay%20tres%20grupos%20principales%20de,Lossless%20y%20ape%20Monkey%27s%20Audio), este proceso interno suele ser muy molesto, ya que, el audio final se ve afectado por los algoritmos de comprensión de audio que tenga el propio sistema operativo.

Es aquí, donde llega al rescate los sistemas _bit-perfect_, estos toman control exclusivo de la tarjeta de sonido o del DAC y se saltan todos los procesos del mixer internos, para así, darle una señal bit a bit exacto de cómo debería ser la onda de sonido, que luego se escuchara por los altavoces o audífonos.

### Soporte para muchos códecs
Realmente la mayoría de reproductores de música dan soporte a los códecs más usados, tales como mp3, ogg, aac, m4a, flac, wav, etc. Me atrevería a decir que si un reproductor de audio soporta _bit-perfect_ este tendría de por si una gran cantidad de códecs a su disposición.

### Personalizable
Puede no parecer importante, pero no me gusta que el reproductor sea muy rígido en cuanto su estructura, me gusta decidir que quiero ver, me gusta crear columnas personalizables, etiquetas, listas de reproducción, me gusta cambiar los colores de como se ve todo, incluso me encanta cuando el reproductor permite crear _skins_ que luego las personas comparten en internet.

### Rapidez
A nadie le gusta esperar, y no todos tenemos un muy buen computador para que todo sea muy veloz, por eso busco un reproductor liviano, que demande muy pocos recursos del sistema pero que a la vez sea muy poderoso por dentro.

## Conclusión
Luego de estar varios días navegando, y de probar muchas opciones, he tomado al fin una decisión, usar el reproductor llamado [cmus](https://cmus.github.io/), cumple con todas las características que he mencionado.

<p><img src="https://i.imgur.com/B0wAau4.png"></p>

Muy pronto estaré publicando un pequeño tutorial de como fui configurando cmus para que se adapte a mis necesidades, y como fui resolviendo algunos problemas habituales que se me presentaron en el camino.