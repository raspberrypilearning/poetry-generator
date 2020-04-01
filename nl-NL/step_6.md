## Meer poëzie

Je gedicht is vrij kort - laten we er wat aan toevoegen!

--- task ---

Laten we bijwoorden in de volgende regel van je gedicht gebruiken. Een **bijwoord** is een woord dat een werkwoord beschrijft. Maak nog een lijst met als naam bijwoorden en voeg deze 3 woorden toe:

![lijst met de woorden luidruchtig, stilletjes, oneindig](images/poetry-adverbs.png)

--- /task ---

--- task ---

Voeg deze regel toe aan de code van de computer, om een willekeurig bijwoord op de volgende regel van je gedicht te zeggen:

![computer sprite](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Hier is je gedicht...] for (2) seconds
say (join [Ik ](item (pick random (1) to (length of [werkwoorden v])) of [werkwoorden v])) for (2) seconds
+say (item (pick random (1) to (length of [bijwoorden v])) of [bijwoorden v]) for (2) seconds
```

--- /task ---

--- task ---

Test je code een paar keer. Je zou elke keer een willekeurig gedicht moeten zien.

![willekeurige tekstballonnen met bijwoorden](images/poetry-adverb-test.png)

--- /task ---

--- task ---

Voeg een lijst met zelfstandige naamwoorden toe aan je project. Een **zelfstandig naamwoord** is een plaats of een ding.

![een lijst met zelfstandige naamwoorden met de woorden zee, maan, boom](images/poetry-nouns.png)

--- /task ---

--- task ---

Voeg code toe om de zelfstandige naamwoorden in je gedicht te gebruiken.

![computer sprite](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Hier is je gedicht...] for (2) seconds
say (join [Ik ](item (pick random (1) to (length of [werkwoorden v])) of [werkwoorden v])) for (2) seconds
say (item (pick random (1) to (length of [bijwoorden v])) of [bijwoorden v]) for (2) seconds
+say (join [bij de ](item (pick random (1) to (length of [zelfstandige naamwoorden v])) of [zelfstandige naamwoorden v])) for (2) seconds
```

--- /task ---

--- task ---

Voeg een lijst met bijvoeglijke naamwoorden toe aan je project. Een **bijvoeglijk naamwoord** is een beschrijvend woord.

![een lijst met bijvoeglijke naamwoorden blij, moe, hongerig](images/poetry-adjectives.png)

--- /task ---

--- task ---

Voeg code toe om de bijvoeglijke naamwoorden in je gedicht te gebruiken:

![computer sprite](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Hier is je gedicht...] for (2) seconds
say (join [Ik ](item (pick random (1) to (length of [werkwoorden v])) of [werkwoorden v])) for (2) seconds
say (item (pick random (1) to (length of [bijwoorden v])) of [bijwoorden v]) for (2) seconds
say (join [bij de ](item (pick random (1) to (length of [zelfstandige naamwoorden v])) of [zelfstandige naamwoorden v])) for (2) seconds
+ say (join [Ik voel me ](item (pick random (1) to (length of [bijvoeglijke naamwoorden v])) of [bijvoeglijke naamwoorden v])) for (2) seconds
```

--- /task ---

--- task ---

Je kunt op de vakjes naast je lijsten klikken om ze te verbergen.

![lijst variabelen met de geselecteerde selectievakjes](images/poetry-lists-tick.png)

--- /task ---

--- task ---

Test je nieuwe gedicht.

--- /task ---