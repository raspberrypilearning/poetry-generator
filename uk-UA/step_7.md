## Анімація аналітичної машини

Давай анімуємо твій комп’ютер, щоб здавалося, що він генерує вірші.

\--- task \---

Клацни на спрайт комп’ютера та додай цей код після першого блоку `говорити`{:class="block3looks"}:

В розділі `Керування`{:class="block3control"} ти знайдеш блоки `повторити`{:class="block3control"} та `чекати`{:class="block3control"}.

![спрайт комп’ютера](images/computer-sprite.png)

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

Перевір свій проєкт. Ти маєш побачити, як комп’ютер хитається перед тим, як видати вірш!

![спрайт комп’ютера, що хитається](images/poetry-animate-test.png)

\--- /task \---

\--- task \---

Перейди у вкладку "Звуки" і клацни "Обрати звук" в нижньому лівому куті.

[[[generic-scratch3-sound-from-library]]]

\--- /task \---

\--- task \---

Вибери звук "Computer Beep".

![звуки computer beeps 1 та 2 в бібліотеці звуків](images/poetry-beeps.png)

\--- /task \---

\--- task \---

Додай блок `відтворити звук`{:class="block3sound"}, щоб відтворити його перед початком анімації.

![спрайт комп’ютера](images/computer-sprite.png)

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