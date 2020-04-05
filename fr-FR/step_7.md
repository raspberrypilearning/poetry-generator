## Animons la Machine Analytique

Animons l'ordinateur, afin qu'il ait l'air de générer de la poésie.

\--- task \---

Clique sur ton sprite ordinateur, et ajoute ce code après le premier bloc `dire`{:class="block3looks"} :

Tu trouveras les blocs `répéter`{:class="block3control"} et `attendre`{:class="block3control"} dans la section `Contrôle`{:class="block3control"}.

![sprite ordinateur](images/computer-sprite.png)

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

Teste ton projet. Tu devrais voir l'ordinateur trembler avant de produire un poème !

![sprite ordinateur secouant d'avant en arrière](images/poetry-animate-test.png)

\--- /task \---

\--- task \---

Clique sur l’onglet « Sons » et clique sur l’icône « Choisir un son » en bas à gauche.

[[[generic-scratch3-sound-from-library]]]

\--- /task \---

\--- task \---

Choisis le son « computer beep » et clique sur OK.

![les deux bips sons dans la bibliothèque de sons](images/poetry-beeps.png)

\--- /task \---

\--- task \---

Ajoute un bloc `commencer le son`{:class="block3sound"}, pour jouer ton son juste avant le début de ton animation.

![sprite ordinateur](images/computer-sprite.png)

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