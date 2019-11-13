## Digues-li el teu nom a l'Ada

L'Ada s'ha presentat, però ella no sap el teu nom!

\--- task \---

Drag an `ask`{:class="block3sensing"} block (from the `sensing`{:class="block3sensing"} section) onto your code. Així és com s'hauria de veure el teu codi:

![ada sprite](images/ada-sprite.png)

```blocks3
when this sprite clicked
say [Hi, I'm Ada!] for (2) seconds
+ ask [What's your name?] and wait
```

\--- /task \---

\--- task \---

Feu clic a l'Ada per provar el vostre codi. L'Ada t'hauria de demanar el teu nom, que pots escriure!

![ada sprite asking whats your name](images/poetry-input.png)

\--- /task \---

\--- task \---

Podem utilitzar una **variable** per emmagatzemar el teu nom. Click `Data`{:class="block3variables"}, and then 'Make a Variable'. Com que aquesta variable s'utilitzarà per emmagatzemar el vostre nom, anomenem la variable... `name`{:class="block3variables"}!

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

Fes clic a l'Ada per provar el teu codi i introdueix el teu nom quan s'et demani. You should see that your name has been stored in the `name`{:class="block3variables"} variable.

![captura de pantalla](images/poetry-name-test.png)

\--- /task \---

\--- task \---

Ara ja pots fer ús del del teu nom en el teu codi. Afegeix aquest codi:

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

Prova el codi nou. L'Ada hauria de saludar-te amb el teu nom!

![captura de pantalla](images/poetry-name-test2.png)

Si no hi ha espai entre la paraula "Hola" i el teu nom, hauràs d'afegir-hi un espai al codi!

\--- /task \---

\--- task \---

Finalment, afegeix aquest codi per explicar què fer a continuació:

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

Prova el codi de l'Ada per última vegada, per assegurar-te que tot funciona.

\--- /task \---