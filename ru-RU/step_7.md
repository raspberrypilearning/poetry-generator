## Анимируем аналитический двигатель

Давай оживим твой компьютер, чтобы он выглядел так, как будто он генерирует стихи.

\--- task \---

Нажми на спрайт компьютера и добавь этот код после первого блока `говорить`{:class="block3looks"}:

Ты найдешь блоки `повторить`{:class="block3control"} и `ждать`{:class="block3control"} в секции `Управление`{:class="block3control"}.

![спрайт компьютер](images/computer-sprite.png)

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

Протестируй свой проект. Ты должен увидеть как компьютер трясется, перед ткм, как создать стихотворение!

![спрайт компьютера трясется](images/poetry-animate-test.png)

\--- /task \---

\--- task \---

Перейди на вкладку «Звуки» и нажмите значок «Выбрать звук» в левом нижнем углу.

[[[generic-scratch3-sound-from-library]]]

\--- /task \---

\--- task \---

Выбери звук «компьютерный сигнал» и нажми «ОК».

![компьютер издает звуки 1 и 2 из звуковой библиотеки](images/poetry-beeps.png)

\--- /task \---

\--- task \---

Добавь блок `включить звук`{:class="block3sound"}, чтобы воспроизвести звук непосредственно перед началом анимации.

![спрайт компьютер](images/computer-sprite.png)

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