## 解析機関(アナリティカルエンジン)

エイダのコンピュータ(「アナリティカルエンジン」と呼ばれています)が詩を生成するようにプログラムしてみましょう。

--- task ---

このコードを 'Computer'スプライトに追加して、クリックしたときに読み上げられるようにします。

![computer スプライト](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [あなたのための詩です。] for (2) seconds
```

--- /task ---

--- task ---

ランダムな詩を作成するには、使用する言葉の**リスト**が最初に必要です。 新しいリストを作成するには、`変数`{:class="block3variables"}タブをクリックします。

詩の最初の行に**動詞**(動きを表す言葉)を使いましょう。 `動詞`{:class="block3variables"}という新しいリストを作成します。

[[[generic-scratch3-make-list]]]

--- /task ---

--- task ---

新しいリストには何も入っていません。 空のリストの一番下にある`+`をクリックして次の動詞を追加します。

![+が強調表示されたリスト](images/poetry-verbs-annotated.png)

--- /task ---

--- task ---

詩の最初の行は「私は」という単語で始まり、ランダムに選ばれた動詞が続きます。

この一行の詩を作成するには、次のことを行う必要があります。

1. `1`から`動詞リストの長さ`{:class="block3variables"}`までの乱数`{:class="block3operators"}の間の：
    
    ```blocks3
    (pick random (1) to (length of [動詞 v]))
    ```

2. このブロックを使用して`動詞`{:class="block3variables"}リストからランダム`番目`{:class="block3variables"}を取得します：
    
    ```blocks3
    (item (pick random (1) to (length of [動詞 v]) :: +) of [動詞 v])
    ```

3. 「私は」`と`{:class="block3operators"}ランダムな動詞で詩の最初の行を作成します：
    
    ```blocks3
    (join [私は ] (item (pick random (1) to (length of [動詞 v])) of [動詞 v] :: +))
    ```

4. `と(2)秒言う`{:class="block3looks"}ブロックを使って詩の行を表示します：
    
    ```blocks3
    say (join [私は ](item (pick random (1) to (length of [動詞 v])) of [動詞 v]) :: +) for (2) seconds
    ```

コードは次のようになります:

![computer スプライト](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [あなたのための詩です。] for (2) seconds
+ say (join [私は ](item (pick random (1) to (length of [動詞 v])) of [動詞 v])) for (2) seconds
```

--- /task ---

--- task ---

コードを何回かテストしてください。 コンピュータは`動詞`{:class="block3variables"}リストから、毎回ランダムに単語を選んで表示します。

![異なることを言っている3つの吹き出し](images/poetry-random-test.png)

--- /task ---