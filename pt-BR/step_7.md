## Animando o Motor Analítico

Vamos animar seu computador, para que pareça estar gerando uma poesia.

\--- task \---

Clique em seu ator computador, e adicione este código logo após do primeiro bloco `diga`{:class="block3looks"}:

Você irá encontrar os blocos `repita`{:class="block3control"} e `espere`{:class="block3control"} na categoria `Controle`{:class="block3control"}.

![computer sprite](images/computer-sprite.png)

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

Test your project. You should see the computer shake before producing a poem!

![computer sprite shaking back and forth](images/poetry-animate-test.png)

\--- /task \---

\--- task \---

Click the 'Sounds' tab, and click the 'Choose a Sound' icon in the bottom left.

[[[generic-scratch3-sound-from-library]]]

\--- /task \---

\--- task \---

Choose a 'computer beeps' sound and click OK.

![computer beeps 1 and 2 sounds in sound library](images/poetry-beeps.png)

\--- /task \---

\--- task \---

Add a `start sound`{:class="block3sound"} block, to play your sound just before your animation starts.

![computer sprite](images/computer-sprite.png)

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