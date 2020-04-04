## Więcej poezji

Twój wiersz jest dość krótki - dodajmy coś do niego!

\--- task \---

Użyjmy przysłówków w następnej linijce twojego wiersza. **Przysłówek** to słowo, które opisuje czasownik. Utwórz kolejną listę o nazwie przysłówki i dodaj te 3 słowa:

![lista ze słowami głośno, cicho, nieskończenie](images/poetry-adverbs.png)

\--- /task \---

\--- task \---

Dodaj ten wiersz do kodu komputera, aby powiedzieć losowy przysłówek w następnym wersie wiersza:

![duszek komputera](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Here is your poem...] for (2) seconds
say (join [I ](item (pick random (1) to (length of [verbs v])) of [verbs v])) for (2) seconds
+say (item (pick random (1) to (length of [adverbs v])) of [adverbs v]) for (2) seconds
```

\--- /task \---

\--- task \---

Teraz przetestuj swój kod kilka razy. Za każdym razem powinieneś zobaczyć losowy wiersz.

![losowe dymki z przysłówkami](images/poetry-adverb-test.png)

\--- /task \---

\--- task \---

Dodaj listę rzeczowników do swojego projektu. **Rzeczownik** to miejsce lub rzecz.

![lista rzeczowników ze słowami morze, księżyc, drzewo](images/poetry-nouns.png)

\--- /task \---

\--- task \---

Dodaj kod, aby użyć rzeczowników w wierszu.

![duszek komputera](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Here is your poem...] for (2) seconds
say (join [I ](item (pick random (1) to (length of [verbs v])) of [verbs v])) for (2) seconds
say (item (pick random (1) to (length of [adverbs v])) of [adverbs v]) for (2) seconds
+say (join [by the ](item (pick random (1) to (length of [nouns v])) of [nouns v])) for (2) seconds
```

\--- /task \---

\--- task \---

Dodaj listę przymiotników do swojego projektu. **Przymiotnik** jest słowem opisującym.

![lista przymiotników radosny, zmęczony, głodny](images/poetry-adjectives.png)

\--- /task \---

\--- task \---

Dodaj kod, aby użyć przymiotników w swoim wierszu:

![duszek komputera](images/computer-sprite.png)

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

Możesz kliknąć pola obok listy, aby je ukryć.

![wyświetlić zmienne z zaznaczonymi polami wyboru](images/poetry-lists-tick.png)

\--- /task \---

\--- task \---

Przetestuj swój nowy wiersz.

\--- /task \---