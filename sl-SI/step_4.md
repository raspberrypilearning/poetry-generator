## Povej Ada svoje ime

Ada se je predstavila, vendar ne ve tvojega imena!

\--- task \---

Na svoj kodi povlecite blok z `vprašanji`:: class = "block3sensing"} (iz razdelka `zaznavanja`{: class = "block3sensing"}). Takole mora izgledati vaša koda:

![ada sprite](images/ada-sprite.png)

```blocks3
when this sprite clicked
say [Hi, I'm Ada!] for (2) seconds
+ ask [What's your name?] and wait
```

\--- /task \---

\--- task \---

Kliknite na Ada, da preizkusite svojo kodo. Ada naj vas vpraša svoje ime, ki ga lahko vnesete!

![ada sprite sprašuje, kako je tvoje ime](images/poetry-input.png)

\--- /task \---

\--- task \---

Mi lahko uporabite **spremenljivko** za shranjevanje svoje ime. Click `Variables`{:class="block3variables"}, and then 'Make a Variable'. Ker bo ta spremenljivka uporabljena za shranjevanje vašega imena, pokličimo spremenljivko ... `ime`{: class = "block3variables"}!

[[[generic-scratch3-add-variable]]]

\--- /task \---

\--- task \---

To store your name, click the `Variables`{:class="block3variables"} tab, and then drag the `set name`{:class="block3variables"} block onto the end of your code.

![ada sprite](images/ada-sprite.png)

```blocks3
when this sprite clicked
say [Hi, I'm Ada!] for (2) seconds
ask [What's your name?] and wait
+ set [name v] to [0]
```

\--- /task \---

\--- task \---

Uporabite blok `odgovor`{: class = "block3sensing"}, da shranite odgovor, ki ga vnesete.

![ada sprite](images/ada-sprite.png)

```blocks3
when this sprite clicked
say [Hi, I'm Ada!] for (2) seconds
ask [What's your name?] and wait
set [name v] to (answer :: +)
```

\--- /task \---

\--- task \---

Kliknite na Ada, da preizkusite kodo in na vprašanje vnesite svoje ime. Morali bi videti, da je bilo vaše ime shranjeno v spremenljivki `ime`{: class = "block3variables"}.

![posnetek zaslona](images/poetry-name-test.png)

\--- /task \---

\--- task \---

Zdaj lahko svoje ime uporabite v kodi. Dodaj to kodo:

![ada sprite](images/ada-sprite.png)

```blocks3
when this sprite clicked
say [Hi, I'm Ada!] for (2) seconds
ask [What's your name?] and wait
set [name v] to (answer)
+say (join [Hi ] (name)) for (2) seconds 
```

Če želite ustvariti to kodo:

1. Povlecite blok `pridruži se`{: class = "blockoperators"} na blok `recimo`{: class = "blocklooks"}
    
    ```blocks3
    say (join [apple] [banana] :: +) for (2) seconds
    ```

2. Dodajte blok `ime`{: class = "blockdata"} na blok `pridruži`:: class = "blokkoperators"}.
    
    ```blocks3
    say (join [Hi] (name :: variables +)) for (2) seconds
    ```

\--- /task \---

\--- task \---

Če želite na odru skriti svojo spremenljivko `name`{: class = "block3variables"}, kliknite kljuk poleg spremenljivke.

![oznaka spremenljivke imena](images/poetry-tick-annotated.png)

\--- /task \---

\--- task \---

Preizkusite svojo novo kodo. Ada naj se pozdravi s tvojim imenom!

![posnetek zaslona](images/poetry-name-test2.png)

Če med besedo "Živjo" in vašim imenom ni prostora, boste morali v kodo sami dodati presledek!

\--- /task \---

\--- task \---

Na koncu dodajte to kodo in pojasnite, kaj naj naredim naprej:

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

Zadnjič preizkusite kodo Ade in se prepričajte, ali vse deluje.

\--- /task \---