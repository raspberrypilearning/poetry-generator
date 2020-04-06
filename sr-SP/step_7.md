## Анимирање аналитичког мотора

Анимирајмо ваш рачунар тако да изгледа као да ствара поезију.

\--- task \---

Кликните на рачунарски сприте и додајте овај код после првог блока `рецимо`{: цласс = "блоцк3лоокс"}:

Пронаћи ћете `понављања`{: цласс = "блоцк3цонтрол"} и `причекајте`{: цласс = "блоцк3цонтрол"} блокови су у одељку `Цонтрол`{: цласс = "блоцк3цонтрол"}.

![рачунарски сприте](images/computer-sprite.png)

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

Испробај свој пројекат. Требали бисте видети како се рачунар тресе пре стварања песме!

![компјутерски сприте који се тресе напред-назад](images/poetry-animate-test.png)

\--- /task \---

\--- task \---

Кликните картицу „Звукови“ и у доњем левом углу иконе „Изабери звук“.

[[[generic-scratch3-sound-from-library]]]

\--- /task \---

\--- task \---

Изаберите звук „звучни сигнал рачунара“ и кликните на дугме У реду.

![рачунар звучи 1 и 2 звука у библиотеци звука](images/poetry-beeps.png)

\--- /task \---

\--- task \---

Додајте `почетни звук`{: цласс = "блоцк3соунд"} блок да бисте репродуковали свој звук пре него што анимација почне.

![рачунарски сприте](images/computer-sprite.png)

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