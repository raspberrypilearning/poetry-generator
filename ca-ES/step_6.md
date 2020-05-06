## Més poesia

El teu poema és bastant curt: afegim més text!

\--- task \---

Ara utilitzarem adverbis a la següent línia del teu poema. Un **adverbi** és una paraula que descriu un verb. Crea una altra llista que es digui adverbis i afegeix aquestes 3 paraules:

![list with the words loudly, silently, endlessly](images/poetry-adverbs.png)

\--- /task \---

\--- task \---

Afegeix aquesta línia al codi de l'ordinador, per dir un adverbi a l'atzar a la següent línia del teu poema:

![personatge de l'ordinador](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Here is your poem...] for (2) seconds
say (join [I ](item (pick random (1) to (length of [verbs v])) of [verbs v])) for (2) seconds
+say (item (pick random (1) to (length of [adverbs v])) of [adverbs v]) for (2) seconds
```

\--- /task \---

\--- task \---

Prova el codi diverses vegades. Hauries de veure un poema aleatori cada vegada.

![bombolles parlants amb adverbis a l'atzar](images/poetry-adverb-test.png)

\--- /task \---

\--- task \---

Afegeix una llista de substantius al teu projecte. Un **substantiu** és un lloc o una cosa.

![una llista de substantius amb les paraules mar, lluna, arbre](images/poetry-nouns.png)

\--- /task \---

\--- task \---

Afegeix codi per utilitzar els substantius al teu poema.

![personatge de l'ordinador](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Here is your poem...] for (2) seconds
say (join [I ](item (pick random (1) to (length of [verbs v])) of [verbs v])) for (2) seconds
say (item (pick random (1) to (length of [adverbs v])) of [adverbs v]) for (2) seconds
+say (join [by the ](item (pick random (1) to (length of [nouns v])) of [nouns v])) for (2) seconds
```

\--- /task \---

\--- task \---

Afegeix una llista d'adjectius al teu projecte. Un **adjectiu** és una paraula que descriu.

![una llista d'adjectius amb les paraules feliç, cansada, famolenca](images/poetry-adjectives.png)

\--- /task \---

\--- task \---

Afegeix codi per utilitzar els adjectius al teu poema:

![personatge de l'ordinador](images/computer-sprite.png)

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

Pots fer clic a les caselles que hi ha al costat de les teves llistes per ocultar-les.

![llista de variables amb les caselles de selecció seleccionades](images/poetry-lists-tick.png)

\--- /task \---

\--- task \---

Prova el teu nou poema.

\--- /task \---