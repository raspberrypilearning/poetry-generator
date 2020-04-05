## Animiere die Analytische Maschine

Lass uns deinen Computer animieren, so dass es aussieht, als ob es Gedichte erstellen würde.

--- task ---

Klicke auf deine Computer Figur und füge diesen Code nach dem ersten `sage`{:class="block3looks"} Block hinzu:

Du wirst die `wiederhole`{:class="block3control"} und `warte`{:class="block3control"} Blöcke im `Steuerung`{:class="block3control"} Bereich finden.

![Computer Sprite](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Hier ist dein Gedicht…] for (2) seconds
+ repeat (10)
    turn left (5) degrees
    wait (0.1) seconds
    turn right (5) degrees
    wait (0.1) seconds  
end
say (join [Ich ](item (pick random (1) to (length of [Verben v])) of [Verben v])) for (2) seconds
say (item (pick random (1) to (length of [Adverbien v])) of [Adverbien v]) for (2) seconds
say (join [am ](item (pick random (1) to (length of [Nomen v])) of [Nomen v])) for (2) seconds
say (join [Ich fühle ](item (pick random (1) to (length of [Adjektive v])) of [Adjektive v])) for (2) seconds
```

--- /task ---

--- task ---

Teste dein Projekt. Du solltest nun sehen, dass dein Computer sich schüttelt bevor er ein Gedicht produziert!

![Computer Sprite zittert hin und her](images/poetry-animate-test.png)

--- /task ---

--- task ---

Klicke auf die 'Klänge' Tabelle und klicke auf das 'Wähle einen Klang' Piktogramm links unten.

[[[generic-scratch3-sound-from-library]]]

--- /task ---

--- task ---

Wähle einen 'computer beeps' Klang und klicke auf OK.

![Computer piept 1 und 2 Sounds in der Soundbibliothek](images/poetry-beeps.png)

--- /task ---

--- task ---

Füge einen `starte Klang`{:class="block3sound"} Block hinzu, um deinen Klang, bevor die Animation startet, abzuspielen.

![Computer Sprite](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Hier ist dein Gedicht…] for (2) seconds
+ start sound (computer beeps1 v)
repeat (10)
    turn left (5) degrees
    wait (0.1) seconds
    turn right (5) degrees
    wait (0.1) seconds  
end
say (join [Ich ](item (pick random (1) to (length of [Verben v])) of [Verben v])) for (2) seconds
say (item (pick random (1) to (length of [Adverbien v])) of [Adverbien v]) for (2) seconds
say (join [am ](item (pick random (1) to (length of [Nomen v])) of [Nomen v])) for (2) seconds
say (join [Ich fühle ](item (pick random (1) to (length of [Adjektive v])) of [Adjektive v])) for (2) seconds
```

--- /task ---