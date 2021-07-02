## Animació del motor analític

Ara animarem el teu ordinador, de manera que sembli que està generant poesia.

\--- task \---

Fes clic al personatge de l'ordinador, i afegeix aquest codi després del primer bloc `digues`{:class="blocklooks"}:

Trobareu el `repeteix`{:class="blockcontrol"} i `espera`{:class="blockcontrol"} blocs estan a la secció `Control`{:class="blockcontrol"}.

![captura de pantalla](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Here is your poem...] for (2) seconds
+ repeat (10)
    turn left (5) degrees
    wait (0.1) seconds
    turn right (5) degrees
    wait (0.1) seconds  
end
say (join [I ](item (pick random (1) to (length of [verbs v])) of [verbs v])) for (2) seconds
say (item (pick random (1) to (length of [adverbs v])) of [adverbs v]) for (2) seconds
say (join [by the ](item (pick random (1) to (length of [nouns v])) of [nouns v])) for (2) seconds
say (join [I feel ](item (pick random (1) to (length of [adjectives v])) of [adjectives v])) for (2) seconds
```

\--- /task \---

\--- task \---

Prova el teu projecte. Hauries de veure tremolar l'ordinador abans de crear un poema!

![personatge de l’ordinador tremolant](images/poetry-animate-test.png)

\--- /task \---

\--- task \---

Fes clic a la pestanya "Sons", i a continuació clic a la icona "Tria un so" de la part inferior esquerra.

[[[generic-scratch3-sound-from-library]]]

\--- /task \---

\--- task \---

Tria un so de "sonorització de l'ordinador"(ho trobaràs en anglès amb el nom de "computer beep") i fes clic per confirmar.

![sons "computer beeps 1 i 2" de la biblioteca de sons](images/poetry-beeps.png)

\--- /task \---

\--- task \---

Afegeix un bloc `inicia el so`{:class="blocksound"}, per reproduir el so abans que comenci l'animació.

![personatge de l'ordinador](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Here is your poem...] for (2) seconds
+ start sound (computer beeps1 v)
repeat (10)
    turn left (5) degrees
    wait (0.1) seconds
    turn right (5) degrees
    wait (0.1) seconds  
end
say (join [I ](item (pick random (1) to (length of [verbs v])) of [verbs v])) for (2) seconds
say (item (pick random (1) to (length of [adverbs v])) of [adverbs v]) for (2) seconds
say (join [by the ](item (pick random (1) to (length of [nouns v])) of [nouns v])) for (2) seconds
say (join [I feel ](item (pick random (1) to (length of [adjectives v])) of [adjectives v])) for (2) seconds
```

\--- /task \---