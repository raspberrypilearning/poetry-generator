## 詩をもっとたくさん

いまのままでは詩はとても短いです ー 追加しましょう！

--- task ---

詩の次の行で副詞を使ってみましょう。 **副詞**は動詞を説明する言葉です。 副詞という名前のリストを作成し、次の3つの単語を追加します。

![うるさく、静かに、終わりなくの言葉が入ったリスト](images/poetry-adverbs.png)

--- /task ---

--- task ---

次の行をcomputerのコードに追加して、詩の次の行でランダムな副詞を言うようにしましょう：

![computer スプライト](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [あなたのための詩です。] for (2) seconds
say (join [動詞 ](item (pick random (1) to (length of [動詞 v])) of [動詞 v])) for (2) seconds
+say (item (pick random (1) to (length of [副詞 v])) of [副詞 v]) for (2) seconds
```

--- /task ---

--- task ---

コードを何回かテストしてください。 毎回ランダムな詩が表示されるはずです。

![副詞のランダムな吹き出し](images/poetry-adverb-test.png)

--- /task ---

--- task ---

名詞のリストをプロジェクトに追加します。 **名詞**は場所や物を表す言葉です。

![海、月、木が入った名詞のリスト](images/poetry-nouns.png)

--- /task ---

--- task ---

名詞を詩で使用するコードを追加します。

![computer スプライト](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [あなたのための詩です。] for (2) seconds
say (join [動詞 ](item (pick random (1) to (length of [動詞 v])) of [動詞 v])) for (2) seconds
say (item (pick random (1) to (length of [副詞 v])) of [副詞 v]) for (2) seconds
+say (join [のそばで ](item (pick random (1) to (length of [名詞 v])) of [名詞 v])) for (2) seconds
```

--- /task ---

--- task ---

形容詞のリストをプロジェクトに追加します。 **形容詞**は名詞を説明する言葉です。

![幸せだ、疲れた、お腹が減ったの形容詞のリスト](images/poetry-adjectives.png)

--- /task ---

--- task ---

形容詞を詩で使用するコードを追加します。

![computer スプライト](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [あなたのための詩です。] for (2) seconds
say (join [動詞 ](item (pick random (1) to (length of [動詞 v])) of [動詞 v])) for (2) seconds
say (item (pick random (1) to (length of [副詞 v])) of [副詞 v]) for (2) seconds
say (join [のそばで ](item (pick random (1) to (length of [名詞 v])) of [名詞 v])) for (2) seconds
+ say (join [と感じる ](item (pick random (1) to (length of [形容詞 v])) of [形容詞 v])) for (2) seconds
```

--- /task ---

--- task ---

リストの横にあるボックスをクリックしてリストを表示しないようにすることができます。

![チェックボックスが選ばれたリスト変数](images/poetry-lists-tick.png)

--- /task ---

--- task ---

新しい詩を試してみてください。

--- /task ---