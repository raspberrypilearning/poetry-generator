## 给分析引擎添加动画

让我们给计算机生成一些动画，好让它看起来像在生成诗歌。

--- task ---

单击您的计算机精灵，然后在第一个 `说`{:class="block3looks"} 模块之后添加这些代码：

您可以在 `控制`{:class="block3control"} 分类下找到 `重复执行`{:class="block3control"} 和 `等待`{:class="block3control"} 模块。

![计算机精灵](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [这是你的诗...] for (2) seconds
+ repeat (10)
    turn left (5) degrees
    wait (0.1) seconds
    turn right (5) degrees
    wait (0.1) seconds  
end
say (join [我 ](item (pick random (1) to (length of [动词 v])) of [动词 v])) for (2) seconds
say (item (pick random (1) to (length of [副词 v])) of [副词 v]) for (2) seconds
say (join [在 ](item (pick random (1) to (length of [名词 v])) of [名词 v])) for (2) seconds
say (join [我觉得 ](item (pick random (1) to (length of [形容词 v])) of [形容词 v])) for (2) seconds
```

--- /task ---

--- task ---

测试你的项目。 你应该看到计算机在产生诗歌前会摇动一会！

![计算机来回摇动](images/poetry-animate-test.png)

--- /task ---

--- task ---

单击 “声音” 选项，然后单击左下方的 “选择一个声音” 图标。

[[[generic-scratch3-sound-from-library]]]

--- /task ---

--- task ---

选择一个 “computer beeps” 声音，单击确定。

![计算机发出哔哔叭叭的蜂鸣声](images/poetry-beeps.png)

--- /task ---

--- task ---

添加一个 `播放声音`{:class="block3sound"} 模块，以便在动画开始之前播放声音。

![计算机精灵](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [这是你的诗...] for (2) seconds
+ start sound (computer beeps1 v)
repeat (10)
    turn left (5) degrees
    wait (0.1) seconds
    turn right (5) degrees
    wait (0.1) seconds  
end
say (join [我 ](item (pick random (1) to (length of [动词 v])) of [动词 v])) for (2) seconds
say (item (pick random (1) to (length of [副词 v])) of [副词 v]) for (2) seconds
say (join [在 ](item (pick random (1) to (length of [名词 v])) of [名词 v])) for (2) seconds
say (join [我觉得 ](item (pick random (1) to (length of [形容词 v])) of [形容词 v])) for (2) seconds
```

--- /task ---