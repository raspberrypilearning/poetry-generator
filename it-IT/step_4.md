## Dire ad Ada il tuo nome

Ada si è presentata, ma non conosce il tuo nome!

\--- task \---

Trascina un blocco `chiedi`{:class="block3sensing"} (dalla sezione `sensori`{:class="block3sensing"}) nel tuo codice. Il tuo codice dovrebbe essere più o meno così:

![sprite ada](images/ada-sprite.png)

```blocks3
when this sprite clicked
say [Hi, I'm Ada!] for (2) seconds
+ ask [What's your name?] and wait
```

\--- /task \---

\--- task \---

Fai clic su Ada per testare il tuo codice. Ada dovrebbe chiederti il tuo nome, che puoi digitare!

![sprite ada che chiede come ti chiami](images/poetry-input.png)

\--- /task \---

\--- task \---

Possiamo usare una **variabile** per memorizzare il tuo nome. Fai clic su `Variabili`{:class="block3variables"}, quindi su "Crea una Variabile". Poiché questa variabile verrà utilizzata per memorizzare il tuo nome, chiamiamo la variabile... `nome`{:class="block3variables"}!

[[[generic-scratch3-add-variable]]]

\--- /task \---

\--- task \---

To store your name, click the `Data`{:class="block3variables"} tab, and then drag the `set name`{:class="block3variables"} block onto the end of your code.

![ada sprite](images/ada-sprite.png)

```blocks3
when this sprite clicked
say [Hi, I'm Ada!] for (2) seconds
ask [What's your name?] and wait
+ set [name v] to [0]
```

\--- /task \---

\--- task \---

Use the `answer`{:class="block3sensing"} block to store the answer you type in.

![ada sprite](images/ada-sprite.png)

```blocks3
when this sprite clicked
say [Hi, I'm Ada!] for (2) seconds
ask [What's your name?] and wait
set [name v] to (answer :: +)
```

\--- /task \---

\--- task \---

Click on Ada to test your code, and enter your name when asked. You should see that your name has been stored in the `name`{:class="block3variables"} variable.

![screenshot](images/poetry-name-test.png)

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