## エイダにあなたの名前を伝える

エイダは自己紹介しましたが、彼女はあなたの名前を知りません！

\--- task \---

`と聞いて待つ`{:class="block3sensing"}ブロックを(`調べる`{:class="block3sensing"}セクションから)作成中のコードにドラッグします。 コードは次のようになります。

![ada スプライト](images/ada-sprite.png)

```blocks3
when this sprite clicked
say [Hi, I'm Ada!] for (2) seconds
+ ask [What's your name?] and wait
```

\--- /task \---

\--- task \---

エイダをクリックしてコードをテストします。 エイダはあなたの名前を聞いてきます。そしてあなたは名前をキーボードから入力できます！

![あなたの名前を尋ねるadaスプライト](images/poetry-input.png)

\--- /task \---

\--- task \---

**変数** を使用すればあなたの名前を保存できます。 `変数`{:class="block3variables"}をクリックし、次に「変数を作る」をクリックします。 この変数はあなたの名前を保存するために使用されるので、変数名は... `名前`{:class="block3variables"}にしましょう！

[[[generic-scratch3-add-variable]]]

\--- /task \---

\--- task \---

名前を保存するには、`変数`{:class="block3variables"}タブをクリックし、 `名前を(0)にする`{:class="block3variables"}ブロックをコードの最後にドラッグします。

![ada スプライト](images/ada-sprite.png)

```blocks3
when this sprite clicked
say [Hi, I'm Ada!] for (2) seconds
ask [What's your name?] and wait
+ set [name v] to [0]
```

\--- /task \---

\--- task \---

入力した内容を保存するには、`答え`{:class="block3sensing"}ブロックを使います。

![ada スプライト](images/ada-sprite.png)

```blocks3
when this sprite clicked
say [Hi, I'm Ada!] for (2) seconds
ask [What's your name?] and wait
set [name v] to (answer :: +)
```

\--- /task \---

\--- task \---

エイダをクリックして、問いかけられたらあなたの名前を入力し、コードをテストします。 あなたの名前が`名前`{:class="block3variables"}変数に保存されたことがわかります。

![スクリーンショット](images/poetry-name-test.png)

\--- /task \---

\--- task \---

You can now make use of your name in your code. Add this code:

![ada sprite](images/ada-sprite.png)

```blocks3
when this sprite clicked
say [Hi, I'm Ada!] for (2) seconds
ask [What's your name?] and wait
set [name v] to (answer)
+say (join [Hi ] (name)) for (2) seconds 
```

To create this code:

1. Drag a `join`{:class="blockoperators"} block onto the `say`{:class="blocklooks"} block
    
    ```blocks3
    say (join [apple] [banana] :: +) for (2) seconds
    ```

2. Add your `name`{:class="blockdata"} block onto the `join`{:class="blockoperators"} block.
    
    ```blocks3
    say (join [Hi] (name :: variables +)) for (2) seconds
    ```

\--- /task \---

\--- task \---

To hide your `name`{:class="block3variables"} variable on the stage, click the tick next to the variable.

![tick name variable](images/poetry-tick-annotated.png)

\--- /task \---

\--- task \---

Test your new code. Ada should say hello to you, using your name!

![screenshot](images/poetry-name-test2.png)

If there's no space between the word 'Hi' and your name, you'll need to add a space into the code yourself!

\--- /task \---

\--- task \---

Finally, add this code to explain what to do next:

![ada sprite](images/ada-sprite.png)

```blocks3
when this sprite clicked
say [Hi, I'm Ada!] for (2) seconds
ask [What's your name?] and wait
set [name v] to (answer)
say (join [Hi ] (name)) for (2) seconds 
+ say [Click the computer to generate a poem.] for (2) seconds 
```

\--- /task \---

\--- task \---

Test Ada's code one last time, to make sure that everything works.

\--- /task \---