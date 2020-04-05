## 给分析引擎添加动画

让我们给计算机生成一些动画，好让它看起来像在生成诗歌。

\--- task \---

单击您的计算机精灵，然后在第一个 `说`{:class="block3looks"} 模块之后添加这些代码：

您可以在 `控制`{:class="block3control"} 分类下找到 `重复执行`{:class="block3control"} 和 `等待`{:class="block3control"} 模块。

![计算机精灵](images/computer-sprite.png)

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

测试你的项目。 你应该看到计算机在产生诗歌前会摇动一会！

![计算机来回摇动](images/poetry-animate-test.png)

\--- /task \---

\--- task \---

单击 “声音” 选项，然后单击左下方的 “选择一个声音” 图标。

[[[generic-scratch3-sound-from-library]]]

\--- /task \---

\--- task \---

选择一个 “computer beeps” 声音，单击确定。

![计算机发出 1 和 2 声](images/poetry-beeps.png)

\--- /task \---

\--- task \---

添加一个 `播放声音`{:class="block3sound"} 模块，以便在动画开始之前播放声音。

![计算机精灵](images/computer-sprite.png)

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