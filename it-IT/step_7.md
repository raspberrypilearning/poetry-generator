## Animare il Motore Analitico

Proviamo ad animare il tuo computer, in modo che sembri generare poesia.

--- task ---

Fai clic sullo sprite del tuo computer e aggiungi questo codice dopo il primo blocco `dire`{:class="block3looks"}:

Troverai i blocchi `ripeti`{:class="block3control"} e `attendi`{:class="block3control"} nella sezione `Controllo`{:class="block3control"}.

![sprite computer](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Ecco la tua poesia…] for (2) seconds
+ repeat (10)
    turn left (5) degrees
    wait (0.1) seconds
    turn right (5) degrees
    wait (0.1) seconds  
end
say (join [Io ](item (pick random (1) to (length of [verbi v])) of [verbi v])) for (2) seconds
say (item (pick random (1) to (length of [avverbi v])) of [avverbi v]) for (2) seconds
say (join [dal ](item (pick random (1) to (length of [nomi v])) of [nomi v])) for (2) seconds
say (join [Mi sento ](item (pick random (1) to (length of [aggettivi v])) of [aggettivi v])) for (2) seconds
```

--- /task ---

--- task ---

Prova il tuo progetto. Dovresti vedere il computer scuotersi prima di produrre una poesia!

![sprite del computer che si scuote avanti e indietro](images/poetry-animate-test.png)

--- /task ---

--- task ---

Fai clic sulla scheda 'Suoni' e fai clic sull'icona 'Scegli un Suono' in basso a sinistra.

[[[generic-scratch3-sound-from-library]]]

--- /task ---

--- task ---

Scegli un suono 'Computer Beep' e fai clic su OK.

![suoni computer beep 1 e 2 nella libreria suoni](images/poetry-beeps.png)

--- /task ---

--- task ---

Aggiungi un blocco `avvia riproduzione suono`{:class="block3sound"}, per riprodurre il suono appena prima dell'inizio dell'animazione.

![sprite computer](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Ecco la tua poesia…] for (2) seconds
+ start sound (computer beeps1 v)
repeat (10)
    turn left (5) degrees
    wait (0.1) seconds
    turn right (5) degrees
    wait (0.1) seconds  
end
say (join [Io ](item (pick random (1) to (length of [verbi v])) of [verbi v])) for (2) seconds
say (item (pick random (1) to (length of [avverbi v])) of [avverbi v]) for (2) seconds
say (join [dal ](item (pick random (1) to (length of [nomi v])) of [nomi v])) for (2) seconds
say (join [Mi sento ](item (pick random (1) to (length of [aggettivi v])) of [aggettivi v])) for (2) seconds
```

--- /task ---