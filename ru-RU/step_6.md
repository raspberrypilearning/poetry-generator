## Больше поэзии

Твое стихотворение довольно короткое - давай дополним его!

--- task ---

Давай использовать наречия в следующей строке твоего стихотворения. **Наречие** - это слово, которое описывает глагол. Создай еще один список под названием наречия и добавь эти 3 слова:

![список со словами громко, тихо, бесконечно](images/poetry-adverbs.png)

--- /task ---

--- task ---

Добавь эту строку в код твоего компьютера, чтобы сказать случайное наречие в следующей строке твоего стихотворения:

![спрайт компьютер](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Вот твое стихотворение…] for (2) seconds
say (join [Я ](item (pick random (1) to (length of [глаголы v])) of [глаголы v])) for (2) seconds
+say (item (pick random (1) to (length of [наречия v])) of [наречия v]) for (2) seconds
```

--- /task ---

--- task ---

Протестируй свой код несколько раз. Ты должен видеть каждый раз случайное стихотворение.

![случайные облачка текста с наречиями](images/poetry-adverb-test.png)

--- /task ---

--- task ---

Добавь список существительных в твой проект. **Существительное** - это место или вещь.

![список существительных со словами море, луна, дерево](images/poetry-nouns.png)

--- /task ---

--- task ---

Добавь код, чтобы использовать существительные в твоем стихотворении.

![спрайт компьютер](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Вот твое стихотворение…] for (2) seconds
say (join [Я ](item (pick random (1) to (length of [глаголы v])) of [глаголы v])) for (2) seconds
say (item (pick random (1) to (length of [наречия v])) of [наречия v]) for (2) seconds
+say (join [около ](item (pick random (1) to (length of [существительные v])) of [существительные v])) for (2) seconds
```

--- /task ---

--- task ---

Добавь список прилагательных в твой проект. **Прилагательное** - это описательное слово.

![список прилагательных - счастливый, усталый, голодный](images/poetry-adjectives.png)

--- /task ---

--- task ---

Добавь код, чтобы использовать прилагательные в твоем стихотворении:

![спрайт компьютер](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Вот твое стихотворение…] for (2) seconds
say (join [Я ](item (pick random (1) to (length of [глаголы v])) of [глаголы v])) for (2) seconds
say (item (pick random (1) to (length of [наречия v])) of [наречия v]) for (2) seconds
say (join [около ](item (pick random (1) to (length of [существительные v])) of [существительные v])) for (2) seconds
+ say (join [Я чувствую ](item (pick random (1) to (length of [прилагательные v])) of [прилагательные v])) for (2) seconds
```

--- /task ---

--- task ---

Ты можешь нажать на галочку рядом со списками, чтобы скрыть их.

![список переменных с поставленными галочками](images/poetry-lists-tick.png)

--- /task ---

--- task ---

Проверь свое новое стихотворение.

--- /task ---