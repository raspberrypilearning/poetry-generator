## Dire à Ada ton nom

Ada s'est présentée, mais elle ne connaît pas ton nom!

\--- task \---

Fais glisser un bloc `demander`{: class = "block3sensing"} (de la section `capteurs`{: class = "block3sensing"}) sur ton code. Voici à quoi ton code devrait ressembler :

![ada sprite](images/ada-sprite.png)

```blocks3
when this sprite clicked
say [Hi, I'm Ada!] for (2) seconds
+ ask [What's your name?] and wait
```

\--- /task \---

\--- task \---

Clique sur Ada pour tester votre code. Ada devrait te demander ton nom, que tu peux taper!

![ada sprite asking whats your name](images/poetry-input.png)

\--- /task \---

\--- task \---

Nous pouvons utiliser une variable **** pour stocker ton nom. Clique sur `Variables`{: class = "block3variables"}, puis sur "Créer une variable". Comme cette variable sera utilisée pour stocker ton nom, appelons la variable ... `nom`{: class = "block3variables"}!

[[[generic-scratch3-add-variable]]]

\--- /task \---

\--- task \---

Pour stocker ton nom, clique sur l'onglet `variables`{: class = "block3variables"}, puis fais glisser le bloc `mettre nom`{: class = "block3variables"} à la fin de votre code.

![ada sprite](images/ada-sprite.png)

```blocks3
when this sprite clicked
say [Hi, I'm Ada!] for (2) seconds
ask [What's your name?] and wait
+ set [name v] to [0]
```

\--- /task \---

\--- task \---

Utilise le bloc `réponse`{: class = "block3sensing"} pour stocker la réponse que tu saisis.

![ada sprite](images/ada-sprite.png)

```blocks3
when this sprite clicked
say [Hi, I'm Ada!] for (2) seconds
ask [What's your name?] and wait
set [name v] to (answer :: +)
```

\--- /task \---

\--- task \---

Clique sur Ada pour tester ton code et entre ton nom lorsque tu y es invité. You should see that your name has been stored in the `name`{:class="block3variables"} variable.

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