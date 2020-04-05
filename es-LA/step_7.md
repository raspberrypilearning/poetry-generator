## Animando el motor analítico

Vamos a animar tu computadora, para que parezca que está generando poesía.

--- task ---

Haz clic en el objeto computadora y añade este código después del primer bloque `decir`{:class="block3looks"}:

Encontrarás los bloques `repetir`{:class="block3control"} y `esperar`{:class="block3control"} en la sección `Control`{:class="block3control"}.

![objeto computadora](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Aquí está tu poema…] for (2) seconds
+ repeat (10)
    turn left (5) degrees
    wait (0.1) seconds
    turn right (5) degrees
    wait (0.1) seconds  
end
say (join [Yo ](item (pick random (1) to (length of [verbos v])) of [verbos v])) for (2) seconds
say (item (pick random (1) to (length of [adverbios v])) of [adverbios v]) for (2) seconds
say (join [por el ](item (pick random (1) to (length of [nombres v])) of [nombres v])) for (2) seconds
say (join [Me siento ](item (pick random (1) to (length of [adjetivos v])) of [adjetivos v])) for (2) seconds
```

--- /task ---

--- task ---

Prueba tu proyecto. ¡Deberías ver la computadora temblar antes de producir un poema!

![objeto computadora temblando](images/poetry-animate-test.png)

--- /task ---

--- task ---

Haz clic en la pestaña de "Sonidos", y haz clic en el icono "Elige un sonido" en la esquina inferior izquierda.

[[[generic-scratch3-sound-from-library]]]

--- /task ---

--- task ---

Elige el sonido "computer beep" y haz clic en OK.

![sonidos 1 y 2 de la computadora en la biblioteca de sonido](images/poetry-beeps.png)

--- /task ---

--- task ---

Añadir un bloque `iniciar sonido`{:class="block3sound"} para reproducir el sonido justo antes de que la animación comience.

![objeto computadora](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Aquí está tu poema…] for (2) seconds
+ start sound (computer beeps1 v)
repeat (10)
    turn left (5) degrees
    wait (0.1) seconds
    turn right (5) degrees
    wait (0.1) seconds  
end
say (join [Yo ](item (pick random (1) to (length of [verbos v])) of [verbos v])) for (2) seconds
say (item (pick random (1) to (length of [adverbios v])) of [adverbios v]) for (2) seconds
say (join [por el ](item (pick random (1) to (length of [nombres v])) of [nombres v])) for (2) seconds
say (join [Me siento ](item (pick random (1) to (length of [adjetivos v])) of [adjetivos v])) for (2) seconds
```

--- /task ---