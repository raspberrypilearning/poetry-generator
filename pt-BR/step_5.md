## O Motor Analítico

Vamos programar o computador da Ada (chamado 'Motor Analítico') para gerar a poesia.

\--- task \---

Adicione este código ao seu ator 'Computador', para que fale quando for clicado:

![computer sprite](images/computer-sprite.png)

```blocks3
quando este ator for clicado
diga [Aqui está o seu poema] por (2) segundos
```

\--- /task \---

\--- task \---

Para criar um poema aleatório, primeiro precisará criar uma **lista** de palavras que serão usadas. Para criar uma lista, clica na categoria `Variáveis` {:class="block3variables"}.

Vamos usar **verbos** (palavras que indicam ações) na primeira linha do seu poema. Create a new list called `verbs`{:class="block3variables"}.

[[[generic-scratch3-make-list]]]

\--- /task \---

\--- task \---

Your new list will be empty. Click the `+` at the bottom of your empty list and add these verbs:

![list with the + highlighted](images/poetry-verbs-annotated.png)

\--- /task \---

\--- task \---

The first line of your poem should be the word "I", followed by a random verb.

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