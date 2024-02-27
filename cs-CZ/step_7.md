## Animování analytického stroje

Pojďme tvůj počítač naanimovat tak, aby to vypadalo, že generuje poezii.

--- task ---

Klikni na postavu počítače a po prvním bloku `bublina`{:class="block3looks"} přidej tento kód:

V sekci `Ovládání`{:class="block3control"} najdeš bloky `opakuj`{:class="block3control"} a `čekej`{:class="block3control"}.

![postava počítače](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Tady je tvoje báseň,] for (2) seconds
+ repeat (10)
    turn left (5) degrees
    wait (0.1) seconds
    turn right (5) degrees
    wait (0.1) seconds  
end
say (join [Já ](item (pick random (1) to (length of [slovesa v])) of [slovesa v])) for (2) seconds
say (item (pick random (1) to (length of [příslovce v])) of [příslovce v]) for (2) seconds
say (join [u ](item (pick random (1) to (length of [podstatná jména v])) of [podstatná jména v])) for (2) seconds
say (join [cítím se ](item (pick random (1) to (length of [přídavná jména v])) of [přídavná jména v])) for (2) seconds
```

--- /task ---

--- task ---

Otestuj svůj projekt. Před vytvořením básně by se měl tvůj počítač třepat!

![postava počítače třepající se nahoru a dolů](images/poetry-animate-test.png)

--- /task ---

--- task ---

Klikni na záložku „Zvuky“ a pak vlevo dole klikni na ikonu „Vyber zvuk“.

[[[generic-scratch3-sound-from-library]]]

--- /task ---

--- task ---

Vyber zvuk „Computer Beep“ a klikni na OK.

![počítač pípá 1 a 2 zvuky z knihovny zvuků](images/poetry-beeps.png)

--- /task ---

--- task ---

Přidej blok `začni hrát zvuk`{:class="block3sound"} aby se začal přehrávat zvuk ještě předtím, než tvoje animace začne.

![postava počítače](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Tady je tvoje báseň,] for (2) seconds
+ start sound (computer beeps1 v)
repeat (10)
    turn left (5) degrees
    wait (0.1) seconds
    turn right (5) degrees
    wait (0.1) seconds  
end
say (join [Já ](item (pick random (1) to (length of [slovesa v])) of [slovesa v])) for (2) seconds
say (item (pick random (1) to (length of [příslovce v])) of [příslovce v]) for (2) seconds
say (join [u ](item (pick random (1) to (length of [podstatná jména v])) of [podstatná jména v])) for (2) seconds
say (join [I feel ](item (pick random (1) to (length of [přídavná jména v])) of [přídavná jména v])) for (2) seconds
```

--- /task ---