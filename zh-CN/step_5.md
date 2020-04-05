## 分析引擎

让我们对艾达的计算机（又称为“分析引擎”）编程，生成诗歌。

\--- task \---

将此代码添加到您的“计算机”精灵中，使它在单击时发出声音：

![计算机精灵](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Here is your poem...] for (2) seconds
```

\--- /task \---

\--- task \---

要随机生成诗歌，首先需要一个**列表** 来存储可使用的词。 要创建新的列表，请单击 `变量`{:class="block3variables"} 标签。

让我们在诗歌的第三行使用 **动词**(动作词)。 创建一个名为 `动词`{:class =“block3variables”} 的新列表。

[[[generic-scratch3-make-list]]]

\--- /task \---

\--- task \---

您的新列表将是空的。 点击空列表底部的 `+` 并添加这些动词：

![高亮显示 + 的列表](images/poetry-verbs-annotated.png)

\--- /task \---

\--- task \---

诗歌的第一行应该是单词“ 我”，第三行是一个随机动词。

To create this line of poetry, you need to:

1. `Pick a random number`{:class="block3operators"} between `1` and the `length of the verbs list`{:class="block3variables"}:
    
    ```blocks3
    (pick random (1) to (length of [verbs v]))
    ```

2. Use this block to get a random `item`{:class="block3variables"} from the `verbs`{:class="block3variables"} list:
    
    ```blocks3
    (item (pick random (1) to (length of [verbs v]) :: +) of [verbs v])
    ```

3. `Join`{:class="block3operators"} "I " with the random verb to create the first line of your poem:
    
    ```blocks3
    (join [I ] (item (pick random (1) to (length of [verbs v])) of [verbs v] :: +))
    ```

4. Use a `say`{:class="block3looks"} block to display the line of poetry:
    
    ```blocks3
    say (join [I ](item (pick random (1) to (length of [verbs v])) of [verbs v]) :: +) for (2) seconds
    ```

Your code should look like this:

![computer sprite](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Here is your poem...] for (2) seconds
+ say (join [I ](item (pick random (1) to (length of [verbs v])) of [verbs v])) for (2) seconds
```

\--- /task \---

\--- task \---

Test your code a few times. Your computer should choose a random word from the `verbs`{:class="block3variables"} list each time.

![3 speech bubbles saying different things](images/poetry-random-test.png)

\--- /task \---