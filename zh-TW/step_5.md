## 分析引擎

讓我們對Ada的計算機（稱為“分析引擎”）進行編程以生成詩歌。

\--- task \---

將此代碼添加到您的“計算機”精靈中，以便在單擊時發出聲音：

![電腦精靈](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Here is your poem...] for (2) seconds
```

\--- /task \---

\--- task \---

要創建隨機詩，首先需要一個**列表**使用的單詞。 要創建新列表，請單擊`變量` {：class =“ block3variables”}標籤。

讓我們使用**動詞** （動作詞）在詩歌的第一行。 建立一個清單，命名為 `序列`{:class="block3variables"}。

[[[generic-scratch3-make-list]]]

\--- /task \---

\--- task \---

您的新列表將為空。 點擊` + `在空列表的底部，添加以下動詞：

![列出並突出顯示+](images/poetry-verbs-annotated.png)

\--- /task \---

\--- task \---

詩歌的第一行應該是單詞“ I”，然後是一個隨機動詞。

要創建這一行詩，您需要：

1. `選擇一個隨機數` {：class =“ block3operators”}在` 1之間`和動詞列表的`長度` {：class =“ block3variables”}：
    
    ```blocks3
    (pick random (1) to (length of [verbs v]))
    ```

2. 使用此塊獲取隨機的`物品`來自`動詞的{：class =“ block3variables”} ` {：class =“ block3variables”}列表：
    
    ```blocks3
    (item (pick random (1) to (length of [verbs v]) :: +) of [verbs v])
    ```

3. `加入` {：class =“ block3operators”}“ I”與隨機動詞一起創建詩歌的第一行：
    
    ```blocks3
    (join [I ] (item (pick random (1) to (length of [verbs v])) of [verbs v] :: +))
    ```

4. 使用` ` {：class =“ block3looks”}塊以顯示詩歌行：
    
    ```blocks3
    say (join [I ](item (pick random (1) to (length of [verbs v])) of [verbs v]) :: +) for (2) seconds
    ```

你的程式應該會像這樣：

![電腦精靈](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Here is your poem...] for (2) seconds
+ say (join [I ](item (pick random (1) to (length of [verbs v])) of [verbs v])) for (2) seconds
```

\--- /task \---

\--- task \---

測試您的代碼幾次。 您的計算機應該從`動詞中選擇一個隨機詞` {：class =“ block3variables”}每次都列出。

![3泡泡說不同的話](images/poetry-random-test.png)

\--- /task \---