## 解析機関を動かす

コンピュータを動かして、詩を生み出しているように見せます。

--- task ---

computerスプライトをクリックし、最初の`と(2)秒言う`{:class="block3looks"}ブロックの後にこのコードを追加します：

You'll find the `(10)回繰り返す`{:class="block3control"} and `(1)秒待つwait`{:class="block3control"}ブロックは`制御`{:class="block3control"}セクションにあります。

![computer スプライト](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [あなたのための詩です。] for (2) seconds
+ repeat (10)
    turn left (5) degrees
    wait (0.1) seconds
    turn right (5) degrees
    wait (0.1) seconds  
end
say (join [私は ](item (pick random (1) to (length of [動詞 v])) of [動詞 v])) for (2) seconds
say (item (pick random (1) to (length of [副詞 v])) of [副詞 v]) for (2) seconds
say (join [のそばで ](item (pick random (1) to (length of [動詞 v])) of [動詞 v])) for (2) seconds
say (join [と感じる ](item (pick random (1) to (length of [名詞 v])) of [名詞 v])) for (2) seconds
```

--- /task ---

--- task ---

プロジェクトをテストします。 詩を作る前にコンピュータが揺れ動きます！

![前後に揺れているcomputerスプライト](images/poetry-animate-test.png)

--- /task ---

--- task ---

「音」タブをクリックし、左下にある「音を選ぶ」アイコンをクリックします。

[[[generic-scratch3-sound-from-library]]]

--- /task ---

--- task ---

「computer beeps」を選択し、[OK]をクリックします。

![音のライブラリの中のcomputer beeps 1と2](images/poetry-beeps.png)

--- /task ---

--- task ---

コンピュータが揺れ動く直前に音が再生されるよう、`の音を鳴らす`{:class="block3sound"}ブロックを追加します。

![computer スプライト](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [あなたのための詩です。] for (2) seconds
+ start sound (computer beeps1 v)
repeat (10)
    turn left (5) degrees
    wait (0.1) seconds
    turn right (5) degrees
    wait (0.1) seconds  
end
say (join [私は ](item (pick random (1) to (length of [動詞 v])) of [動詞 v])) for (2) seconds
say (item (pick random (1) to (length of [副詞 v])) of [副詞 v]) for (2) seconds
say (join [のそばで ](item (pick random (1) to (length of [動詞 v])) of [動詞 v])) for (2) seconds
say (join [と感じる ](item (pick random (1) to (length of [名詞 v])) of [名詞 v])) for (2) seconds
```

--- /task ---