## Animarea motorului analitic

Hai să animăm computer-ul astfel încât acesta să arate că generează poezie.

--- task ---

Dă click pe personajul computer-ului tău și adaugă acest cod după primul bloc `spune`{:class="block3looks"}:

Vei găsi blocurile `repetă`{:class="block3control"} și `așteaptă`{:class="block3control"} în secțiunea `Control`{:class="block3control"}.

![personaj computer](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Aici este poezia ta…] for (2) seconds
+ repeat (10)
    turn left (5) degrees
    wait (0.1) seconds
    turn right (5) degrees
    wait (0.1) seconds  
end
say (join [Eu ](item (pick random (1) to (length of [verbe v])) of [verbe v])) for (2) seconds
say (item (pick random (1) to (length of [adverbe v])) of [adverbe v]) for (2) seconds
say (join [lângă ](item (pick random (1) to (length of [substantive v])) of [substantive v])) for (2) seconds
say (join [Mă simt ](item (pick random (1) to (length of [adjective v])) of [adjective v])) for (2) seconds
```

--- /task ---

--- task ---

Testează-ți proiectul. Ar trebui să vezi cum se mișcă computer-ul tău înainte de a produce un poem!

![personajul calculatorului zguduindu-se înainte și înapoi](images/poetry-animate-test.png)

--- /task ---

--- task ---

Dă click pe secțiunea „Sunet” și apoi pe pictograma „Alege un sunet” din partea stângă jos.

[[[generic-scratch3-sound-from-library]]]

--- /task ---

--- task ---

Alege un sunet de tip „Computer Beeps” și apasă OK.

![computerul emite sunete de 1 și 2 sunete din sunetoteca](images/poetry-beeps.png)

--- /task ---

--- task ---

Adaugă un bloc `pornește sunetul`{:class="block3sound"}, pentru a reda sunetul chiar înainte ca animația să înceapă.

![personaj computer](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Aici este poezia ta…] for (2) seconds
+ start sound (computer beeps1 v)
repeat (10)
    turn left (5) degrees
    wait (0.1) seconds
    turn right (5) degrees
    wait (0.1) seconds  
end
say (join [Eu ](item (pick random (1) to (length of [verbe v])) of [verbe v])) for (2) seconds
say (item (pick random (1) to (length of [adverbe v])) of [adverbe v]) for (2) seconds
say (join [lângă ](item (pick random (1) to (length of [substantive v])) of [substantive v])) for (2) seconds
say (join [Mă simt ](item (pick random (1) to (length of [adjective v])) of [adjective v])) for (2) seconds
```

--- /task ---