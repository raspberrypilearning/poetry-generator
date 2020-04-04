## Mai multă poezie

Poezia ta este destul de scurtă - hai să o mărim!

\--- task \---

Să folosim adverbe în următorul vers al poeziei tale. Un ** adverb ** este un cuvânt care descrie un verb. Creează o altă listă numită adverbe și adaugă aceste 3 cuvinte:

![list with the words loudly, silently, endlessle](images/poetry-adverbs.png)

\--- /task \---

\--- task \---

Adaugă această linie la codul computerului tău pentru ca acesta să pună un adverb aleatoriu pe următorul vers al poeziei:

![computer sprite](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Here is your poem...] for (2) seconds
say (join [I ](item (pick random (1) to (length of [verbs v])) of [verbs v])) for (2) seconds
+say (item (pick random (1) to (length of [adverbs v])) of [adverbs v]) for (2) seconds
```

\--- /task \---

\--- task \---

Testează-ți codul de câteva ori. Ar trebui să vezi o poezie aleatorie de fiecare dată.

![random speech bubbles with adverbs](images/poetry-adverb-test.png)

\--- /task \---

\--- task \---

Adaugă o listă de substantive la proiectul tău. Un **substantiv** este un loc sau un lucru.

![a list of nouns with the words sea, moon, tree](images/poetry-nouns.png)

\--- /task \---

\--- task \---

Adaugă cod pentru a folosi substantivele în poezia ta.

![computer sprite](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Here is your poem...] for (2) seconds
say (join [I ](item (pick random (1) to (length of [verbs v])) of [verbs v])) for (2) seconds
say (item (pick random (1) to (length of [adverbs v])) of [adverbs v]) for (2) seconds
+say (join [by the ](item (pick random (1) to (length of [nouns v])) of [nouns v])) for (2) seconds
```

\--- /task \---

\--- task \---

Adaugă o listă de adjective la proiectul tău. An **adjective** is a describing word.

![a list of adjective words happy, tired, hungry](images/poetry-adjectives.png)

\--- /task \---

\--- task \---

Add code to use the adjectives in your poem:

![computer sprite](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Here is your poem...] for (2) seconds
say (join [I ](item (pick random (1) to (length of [verbs v])) of [verbs v])) for (2) seconds
say (item (pick random (1) to (length of [adverbs v])) of [adverbs v]) for (2) seconds
say (join [by the ](item (pick random (1) to (length of [nouns v])) of [nouns v])) for (2) seconds
+ say (join [I feel ](item (pick random (1) to (length of [adjectives v])) of [adjectives v])) for (2) seconds
```

\--- /task \---

\--- task \---

You can click the boxes next to your lists to hide them.

![list variables with the tick boxes selected](images/poetry-lists-tick.png)

\--- /task \---

\--- task \---

Test out your new poem.

\--- /task \---