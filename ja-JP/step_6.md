## More poetry

Your poem is quite short - let's add to it!

\--- task \---

Let's use adverbs in the next line of your poem. An **adverb** is a word that describes a verb. 副詞という名前のリストを作成し、次の3つの単語を追加します。

![うるさく、静かに、終わりなくの言葉が入ったリスト](images/poetry-adverbs.png)

\--- /task \---

\--- task \---

次の行をcomputerのコードに追加して、詩の次の行でランダムな副詞を言うようにしましょう：

![computer スプライト](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Here is your poem...] for (2) seconds
say (join [I ](item (pick random (1) to (length of [verbs v])) of [verbs v])) for (2) seconds
+say (item (pick random (1) to (length of [adverbs v])) of [adverbs v]) for (2) seconds
```

\--- /task \---

\--- task \---

Test your code a few times. You should see a random poem each time.

![random speech bubbles with adverbs](images/poetry-adverb-test.png)

\--- /task \---

\--- task \---

Add a list of nouns to your project. A **noun** is a place or a thing.

![a list of nouns with the words sea, moon, tree](images/poetry-nouns.png)

\--- /task \---

\--- task \---

Add code to use the nouns in your poem.

![computer sprite](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Here is your poem...] for (2) seconds
say (join [I ](item (pick random (1) to (length of [verbs v])) of [verbs v])) for (2) seconds
say (item (pick random (1) to (length of [adverbs v])) of [adverbs v]) for (2) seconds
+say (join [by the ](item (pick random (1) to (length of [nouns v])) of [nouns v])) for (2) seconds
```

\--- /task \---

\--- task \---

Add a list of adjectives to your project. An **adjective** is a describing word.

![a list of adjective words happy, tired, hungry](images/poetry-adjectives.png)

\--- /task \---

\--- task \---

Add code to use the adjectives in your poem:

![computer sprite](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Here is your poem...] for (2) seconds
say (join [I ](item (pick random (1) to (length of [verbs v])) of [verbs v])) for (2) seconds
say (item (pick random (1) to (length of [adverbs v])) of [adverbs v]) for (2) seconds
say (join [by the ](item (pick random (1) to (length of [nouns v])) of [nouns v])) for (2) seconds
+ say (join [I feel ](item (pick random (1) to (length of [adjectives v])) of [adjectives v])) for (2) seconds
```

\--- /task \---

\--- task \---

You can click the boxes next to your lists to hide them.

![list variables with the tick boxes selected](images/poetry-lists-tick.png)

\--- /task \---

\--- task \---

Test out your new poem.

\--- /task \---