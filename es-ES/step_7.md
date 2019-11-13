## Animando el motor analítico

Animemos el ordenador, para que parezca que está generando poesía.

\--- task \---

Haz clic en la imagen del ordenador y añade este código despues del primer bloque `decir`{:class="block3looks"}:

Encontrarás los bloques `repetir`{:class="block3control"} y `esperar`{:class="block3control"} en la sección `Control`{:class="block3control"}.

![imagen ordenador](images/computer-sprite.png)

```blocks3
al hacer clic en este objeto
decir [Aquí está tu poema...] durante (2) segundos
+ repetir (10)
girar a la izquierda (5) grados
esperar (0.1) segundos
girar a la derecha (5) grados
 esperar (0.1) segundos
fin
decir (unir [Yo ](elemento (número aleatorio entre (1) y (longitud de [verbos v])) de [verbos v])) durante (2) segundos
decir (elemento (número aleatorio entre (1) y (longitud de [adverbios v])) de [adverbios v]) durante (2) segundos
decir (unir [por](elemento (número aleatorio entre (1) y (longitud de [nombres v])) de [nombres v])) durante (2) segundos
decir (unir [me siento ](elemento (número aleatorio entre (1) y (longitud de [adjetivos v])) de [adjetivos v])) durante (2) segundos
```

\--- /task \---

\--- task \---

Prueba tu proyecto. ¡Deberías ver que el ordenador tiembla antes de producir un poema!

![imagen ordenador temblando](images/poetry-animate-test.png)

\--- /task \---

\--- task \---

Haz clic en la pestaña de "Sonidos", y haz clic en el icono "Elige un sonido" en la esquina inferior izquierda.

[[[generic-scratch3-sound-from-library]]]

\--- /task \---

\--- task \---

Elige el sonido "computer beep" y haz clic en OK.

![pitidos de ordenador 1 y 2 en la librería de sonidos](images/poetry-beeps.png)

\--- /task \---

\--- task \---

Añadir un bloque `iniciar sonido`{:class="block3sound"} para reproducir el sonido justo antes de que la animación comience.

![imagen ordenador](images/computer-sprite.png)

```blocks3
al hacer clic en este objeto
decir [Aquí está tu poema...] durante (2) segundos
+ iniciar sonido (computer beep 1 v)
repetir (10)
girar a la izquierda (5) grados
esperar (0.1) segundos
girar a la derecha (5) grados
 esperar (0.1) segundos
fin
decir (unir [Yo ](elemento (número aleatorio entre (1) y (longitud de [verbos v])) de [verbos v])) durante (2) segundos
decir (elemento (número aleatorio entre (1) y (longitud de [adverbios v])) de [adverbios v]) durante (2) segundos
decir (unir [por](elemento (número aleatorio entre (1) y (longitud de [nombres v])) de [nombres v])) durante (2) segundos
decir (unir [me siento ](elemento (número aleatorio entre (1) y (longitud de [adjetivos v])) de [adjetivos v])) durante (2) segundos
```

\--- /task \---