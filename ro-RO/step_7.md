## Animarea motorului analitic

Hai să animăm computer-ul astfel încât acesta să arate că generează poezie.

\--- task \---

Dă click pe personajul computer-ului tău și adaugă acest cod după primul bloc `spune`{:class="block3looks"}:

Vei găsi blocurile `repetă`{:class="block3control"} și `așteaptă`{:class="block3control"} în secțiunea `Control`{:class="block3control"}.

![personaj computer](images/computer-sprite.png)

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

Testează-ți proiectul. Ar trebui să vezi cum se mișcă computer-ul tău înainte de a produce un poem!

![personajul calculatorului zguduindu-se înainte și înapoi](images/poetry-animate-test.png)

\--- /task \---

\--- task \---

Dă click pe secțiunea „Sunet” și apoi pe pictograma „Alege un sunet” din partea stângă jos.

[[[generic-scratch3-sound-from-library]]]

\--- /task \---

\--- task \---

Alege un sunet de tip „Computer Beeps” și apasă OK.

![computerul emite sunete de 1 și 2 sunete din sunetoteca](images/poetry-beeps.png)

\--- /task \---

\--- task \---

Adaugă un bloc `pornește sunetul`{:class="block3sound"}, pentru a reda sunetul chiar înainte ca animația să înceapă.

![personaj computer](images/computer-sprite.png)

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