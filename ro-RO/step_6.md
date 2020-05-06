## Mai multă poezie

Poezia ta este destul de scurtă - hai să o mărim!

\--- task \---

Să folosim adverbe în următorul vers al poeziei tale. Un ** adverb ** este un cuvânt care descrie un verb. Creează o altă listă numită adverbe și adaugă aceste 3 cuvinte:

![list with the words loudly, silently, endlessly](images/poetry-adverbs.png)

\--- /task \---

\--- task \---

Adaugă această linie la codul computerului tău pentru ca acesta să pună un adverb aleatoriu pe următorul vers al poeziei:

![personaj computer](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Here is your poem...] for (2) seconds
say (join [I ](item (pick random (1) to (length of [verbs v])) of [verbs v])) for (2) seconds
+say (item (pick random (1) to (length of [adverbs v])) of [adverbs v]) for (2) seconds
```

\--- /task \---

\--- task \---

Testează-ți codul de câteva ori. Ar trebui să vezi o poezie aleatorie de fiecare dată.

![bule de vorbire aleatorii cu adverbe](images/poetry-adverb-test.png)

\--- /task \---

\--- task \---

Adaugă o listă de substantive la proiectul tău. Un **substantiv** este un loc sau un lucru.

![o listă de substantive cu cuvintele mare, lună, copac](images/poetry-nouns.png)

\--- /task \---

\--- task \---

Adaugă cod pentru a folosi substantivele în poezia ta.

![personaj computer](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Here is your poem...] for (2) seconds
say (join [I ](item (pick random (1) to (length of [verbs v])) of [verbs v])) for (2) seconds
say (item (pick random (1) to (length of [adverbs v])) of [adverbs v]) for (2) seconds
+say (join [by the ](item (pick random (1) to (length of [nouns v])) of [nouns v])) for (2) seconds
```

\--- /task \---

\--- task \---

Adaugă o listă de adjective la proiectul tău. Un **adjectiv** este un cuvânt descriptiv.

![o listă de adjective fericit, obosit, flămând](images/poetry-adjectives.png)

\--- /task \---

\--- task \---

Adaugă cod pentru a folosi substantivele în poezia ta:

![personaj computer](images/computer-sprite.png)

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

Poți da click pe casetele de lângă listele tale pentru a le ascunde.

![lista variabilelor cu casetele de bifare selectate](images/poetry-lists-tick.png)

\--- /task \---

\--- task \---

Testează-ți noua poezie.

\--- /task \---