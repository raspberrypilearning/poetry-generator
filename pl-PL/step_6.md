## Więcej poezji

Twój wiersz jest dość krótki - dodajmy coś do niego!

--- task ---

Użyjmy przysłówków w następnej linijce twojego wiersza. **Przysłówek** to słowo, które opisuje czasownik. Utwórz kolejną listę o nazwie przysłówki i dodaj te 3 słowa:

![lista ze słowami głośno, cicho, nieskończenie](images/poetry-adverbs.png)

--- /task ---

--- task ---

Dodaj ten wiersz do kodu komputera, aby powiedzieć losowy przysłówek w następnym wersie wiersza:

![duszek komputera](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Oto twój wiersz…] for (2) seconds
say (join [Ja ](item (pick random (1) to (length of [czasowniki v])) of [czasowniki v])) for (2) seconds
+say (item (pick random (1) to (length of [przysłówki v])) of [przysłówki v]) for (2) seconds
```

--- /task ---

--- task ---

Teraz przetestuj swój kod kilka razy. Za każdym razem powinieneś zobaczyć losowy wiersz.

![losowe dymki z przysłówkami](images/poetry-adverb-test.png)

--- /task ---

--- task ---

Dodaj listę rzeczowników do swojego projektu. **Rzeczownik** to miejsce lub rzecz.

![lista rzeczowników ze słowami morze, księżyc, drzewo](images/poetry-nouns.png)

--- /task ---

--- task ---

Dodaj kod, aby użyć rzeczowników w wierszu.

![duszek komputera](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Oto twój wiersz…] for (2) seconds
say (join [Ja ](item (pick random (1) to (length of [czasowniki v])) of [czasowniki v])) for (2) seconds
say (item (pick random (1) to (length of [przysłówki v])) of [przysłówki v]) for (2) seconds
+say (join [przy ](item (pick random (1) to (length of [rzeczowniki v])) of [rzeczowniki v])) for (2) seconds
```

--- /task ---

--- task ---

Dodaj listę przymiotników do swojego projektu. **Przymiotnik** jest słowem opisującym.

![lista przymiotników radosny, zmęczony, głodny](images/poetry-adjectives.png)

--- /task ---

--- task ---

Dodaj kod, aby użyć przymiotników w swoim wierszu:

![duszek komputera](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Oto twój wiersz…] for (2) seconds
say (join [Ja ](item (pick random (1) to (length of [czasowniki v])) of [czasowniki v])) for (2) seconds
say (item (pick random (1) to (length of [przysłówki v])) of [przysłówki v]) for (2) seconds
say (join [przy ](item (pick random (1) to (length of [rzeczowniki v])) of [rzeczowniki v])) for (2) seconds
+ say (join [Czuję się ](item (pick random (1) to (length of [przymiotniki v])) of [przymiotniki v])) for (2) seconds
```

--- /task ---

--- task ---

Możesz kliknąć pola obok listy, aby je ukryć.

![wyświetlić zmienne z zaznaczonymi polami wyboru](images/poetry-lists-tick.png)

--- /task ---

--- task ---

Przetestuj swój nowy wiersz.

--- /task ---