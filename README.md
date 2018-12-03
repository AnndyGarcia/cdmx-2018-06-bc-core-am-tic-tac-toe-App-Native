# ROBOTS vs APPLES - App Native
_Un proyecto hecho por Andrea García_

## Introducción

Como desarrolladores web, sabemos que podemos contruir PWAs (_Progressive Web
Apps_) dirigidas a todo tipo de dispositivos, incluyendo celulares y tabletas,
pero hay ciertas situaciones donde podemos preferir una app nativa, como cuando
necesitamos acceso al hardware del dispositivo, UI nativa, código nativo (Java,
Objective C, ...) o que se pueda instalar a través de un
[App Store](https://www.apple.com/lae/ios/app-store/)
o [Google Play](https://play.google.com/).

Exisen muchas herramientas y plataformas para construir aplicaciones para
dispositivos móviles, con soluciones que van desde
[PWA](https://developers.google.com/web/progressive-web-apps/), hasta 100%
nativo, pasando por soluciones híbridas (como [Phonegap](https://phonegap.com/)).
A diferencia de las soluciones híbridas, que han sido populares con
desarrolladores web en el pasado, React Native nos permite construir
aplicaciones realmente _nativas_, pero usando JavaScript y la herramienta elegida. Esto significa
mejor _performance_ y acceso directo al sistema en vez de estar confinado a una
vista _web_.

## Objetivos

En este proyecto, el reto era construir un juego de _tres en raya_ (también llamado _gato_ o _tic tac toe_), utilizando herramientas que nos permitan crear una app *nativa*, es decir, instalable en nuestros dispositivos móviles.

Para este reto, decidí usar _NativeScript_, para poder desarrollar mi juego usando _Angular 6_.

## Desarrollo

Sin embargo, al leer la documentación de NativeScript, me di cuenta de que esta no es suficientemente clara, y al buscar ejemplos o tutoriales, no encontré alguno suficientemente claro o actualizado.
Durante casi todo el tiempo del proyecto estuve experimentando la herramienta, al grado de poder dibujar la grilla,  pero al darle funcionalidad tuve muchos problemas al adaptar TypeScript, pues no todos los métodos son iguales. Adapte varios ejercicios, sin embargo, siempre llegue al punto de que no podía darle funcionalidad.

Por esta razón, decidí cambiar de herramienta a _React Native_, ya que su documentación es bastante mas clara, y tiene mucha mas comunidad que ha aportado ejemplos y tutoriales para poder guiarnos paso a paso.

Con React Native pude desarrollar rápidamente mi aplicación, así como personalizarla un poco, cambiando el tema a Android vs iOS, para darle un poco más de personalidad.

Usando React Native, pude ver en primera persona las diferencias entre React y Angular, y entendí que al aprender primero un framework tan grande y completo como lo es Angular, podía entender mas fácil la forma de trabajo con React, y aunque me falta más experimentación con la librería, creo que podría manejarla rápidamente.

## Producto final

Finalmente, mi aplicación se ve de la siguiente manera:

![robots-vs-apples](https://user-images.githubusercontent.com/8524564/49349729-9e28a000-f671-11e8-8dc6-858389d1f7b9.png)

Sin embargo, en un futuro se le harán modificaciones visuales y mejores, que se estarán documentando aquí.


## Checklist

### UI

- [x] Muestra grilla (grid) de 3x3
- [x] Muestra jugador al que le toca su turno
- [x] Permite marcar cajita vacía
- [x] Cambia el turno después de marcar cajita
- [x] No permite marcar cajita ya marcada
- [x] Permite reiniciar la partida
- [x] Detecta jugadas ganadoras en eje x
- [x] Detecta jugadas ganadoras en eje y
- [x] Detecta jugadas ganadoras en diagonales
- [x] Muestra jugador ganador cuando gana
- [ ] Muestra jugada ganadora cuando hay ganador
- [ ] Muestra empate cuando nadie gana y no quedan cajitas que marcar
- [x] Permite volver a empezar cuando termina una partida (alguien ganó o empate)
