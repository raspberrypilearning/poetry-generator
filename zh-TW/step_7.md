## 動畫分析引擎

讓我們對計算機進行動畫處理，以使其看起來像在生成詩歌。

\--- task \---

單擊您的計算機精靈，然後在第一個`語句之後添加此代碼` {：class =“ block3looks”}塊：

您會發現`重複` {：class =“ block3control”}和`等待` {：class =“ block3control”}塊位於` Control中` {：class =“ block3control”}部分。

![電腦精靈](images/computer-sprite.png)

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

測試你的專案。 在寫詩之前，您應該看到計算機震動！

![電腦精靈來回搖動](images/poetry-animate-test.png)

\--- /task \---

\--- task \---

單擊“聲音”選項卡，然後單擊左下方的“選擇聲音”圖標。

[[[generic-scratch3-sound-from-library]]]

\--- /task \---

\--- task \---

選擇“計算機發出嗶聲”的聲音，然後單擊“確定”。

![聲音庫中計算機發出嗶嗶聲1和2](images/poetry-beeps.png)

\--- /task \---

\--- task \---

添加`開始聲音` {：class =“ block3sound”}塊，以在動畫開始之前播放聲音。

![電腦精靈](images/computer-sprite.png)

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