## 解析機関を動かす

コンピュータを動かして、詩を生み出しているように見せます。

\--- task \---

computerスプライトをクリックし、最初の`と(2)秒言う`{:class="block3looks"}ブロックの後にこのコードを追加します：

You'll find the `(10)回繰り返す`{:class="block3control"} and `(1)秒待つwait`{:class="block3control"}ブロックは`制御`{:class="block3control"}セクションにあります。

![computer スプライト](images/computer-sprite.png)

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

プロジェクトをテストします。 詩を作る前にコンピュータが揺れ動きます！

![前後に揺れているcomputerスプライト](images/poetry-animate-test.png)

\--- /task \---

\--- task \---

「音」タブをクリックし、左下にある「音を選ぶ」アイコンをクリックします。

[[[generic-scratch3-sound-from-library]]]

\--- /task \---

\--- task \---

「computer beeps」を選択し、[OK]をクリックします。

![音のライブラリの中のcomputer beeps 1と2](images/poetry-beeps.png)

\--- /task \---

\--- task \---

Add a `start sound`{:class="block3sound"} block, to play your sound just before your animation starts.

![computer sprite](images/computer-sprite.png)

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