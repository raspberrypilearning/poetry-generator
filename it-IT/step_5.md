## The Analytical Engine

Programmiamo il computer di Ada (chiamato 'Motore Analitico') per generare poesia.

\--- task \---

Aggiungi questo codice allo sprite 'Computer', in modo che parli quando fai clic:

![sprite computer](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Here is your poem...] for (2) seconds
```

\--- /task \---

\--- task \---

Per creare una poesia casuale, per prima cosa avrai bisogno di una **lista** di parole da usare. Per creare una nuova lista, fai clic sulla scheda `Variabili`{:class="block3variables"}.

Usiamo dei **verbi** (parole d'azione) nella prima riga della tua poesia. Crea una nuova lista chiamata `verbi`{:class="block3variables"}.

[[[generic-scratch3-make-list]]]

\--- /task \---

\--- task \---

La tua nuova lista sarà vuota. Click the `+` at the bottom of your empty list and add these verbs:

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