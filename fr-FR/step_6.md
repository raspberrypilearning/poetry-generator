## Plus de poésie

Ton poème est plutôt court, étoffons-le !

\--- task \---

Utilisons des adverbes dans la ligne suivante de ton poème. Un ** adverbe ** est un mot qui décrit un verbe. Crée une autre liste appelée adverbes et ajoute ces 3 mots :

![liste avec les mots bruyamment, silencieusement, sans fin](images/poetry-adverbs.png)

\--- /task \---

\--- task \---

Ajoute cette ligne au code de ton ordinateur, pour dire un adverbe aléatoire sur la ligne suivante de ton poème :

![sprite ordinateur](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Here is your poem...] for (2) seconds
say (join [I ](item (pick random (1) to (length of [verbs v])) of [verbs v])) for (2) seconds
+say (item (pick random (1) to (length of [adverbs v])) of [adverbs v]) for (2) seconds
```

\--- /task \---

\--- task \---

Maintenant, teste ton code plusieurs fois. Tu devrais voir un poème aléatoire à chaque fois.

![bulles aléatoires avec des adverbes](images/poetry-adverb-test.png)

\--- /task \---

\--- task \---

Ajoute une liste de noms à ton projet. Un **nom** est un lieu ou une chose.

![une liste de noms avec les mots de la mer, de la lune, de l'arbre](images/poetry-nouns.png)

\--- /task \---

\--- task \---

Ajoute du code pour utiliser les noms dans ton poème.

![sprite ordinateur](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Here is your poem...] for (2) seconds
say (join [I ](item (pick random (1) to (length of [verbs v])) of [verbs v])) for (2) seconds
say (item (pick random (1) to (length of [adverbs v])) of [adverbs v]) for (2) seconds
+say (join [by the ](item (pick random (1) to (length of [nouns v])) of [nouns v])) for (2) seconds
```

\--- /task \---

\--- task \---

Ajoute une liste d'adjectifs à ton projet. Un **adjectif** précise le sens d'un mot.

![une liste d'adjectifs heureux, fatigué, affamé](images/poetry-adjectives.png)

\--- /task \---

\--- task \---

Ajoute du code pour utiliser les adjectifs dans ton poème :

![sprite ordinateur](images/computer-sprite.png)

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

Tu peux cliquer sur les cases à côté de tes listes pour les cacher.

![les variables liste avec les cases à cocher sélectionnées](images/poetry-lists-tick.png)

\--- /task \---

\--- task \---

Teste ton nouveau poème.

\--- /task \---