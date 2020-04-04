## Animiere die Analytische Maschine

Lass uns deinen Computer animieren, so dass es aussieht, als ob es Gedichte erstellen würde.

\--- task \---

Klicke auf deine Computer Figur und füge diesen Code nach dem ersten `sage`{:class="block3looks"} Block hinzu:

Du wirst die `wiederhole`{:class="block3control"} und `warte`{:class="block3control"} Blöcke im `Steuerung`{:class="block3control"} Bereich finden.

![Computer Sprite](images/computer-sprite.png)

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

Teste dein Projekt. Du solltest nun sehen, dass dein Computer sich schüttelt bevor er ein Gedicht produziert!

![Computer Sprite zittert hin und her](images/poetry-animate-test.png)

\--- /task \---

\--- task \---

Klicke auf die 'Klänge' Tabelle und klicke auf das 'Wähle einen Klang' Piktogramm links unten.

[[[generic-scratch3-sound-from-library]]]

\--- /task \---

\--- task \---

Wähle einen 'computer beeps' Klang und klicke auf OK.

![Computer piept 1 und 2 Sounds in der Soundbibliothek](images/poetry-beeps.png)

\--- /task \---

\--- task \---

Füge einen `starte Klang`{:class="block3sound"} Block hinzu, um deinen Klang, bevor die Animation startet, abzuspielen.

![Computer Sprite](images/computer-sprite.png)

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