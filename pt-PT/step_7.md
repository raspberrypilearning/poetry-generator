## Animar o Motor Analítico

Vamos animar o teu computador, para que pareça que está a gerar poesia.

\--- task \---

Clica no teu ator computador e adiciona-lhe este código a seguir ao primeiro bloco `diz`{:class="block3looks"}:

Vais encontrar os blocos `repete`{:class="block3control"} e `espera`{:class="block3control"} na categoria `Controlo`{:class="block3control"}.

![ator computador](images/computer-sprite.png)

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

Testa o teu projeto. Deverás ver o computador a tremer antes de produzir um poema!

![ator computador a tremer para frente e para trás](images/poetry-animate-test.png)

\--- /task \---

\--- task \---

Vai ao separador 'Sons' e clica no ícone 'Escolher um Som' que está no canto inferior esquerdo.

[[[generic-scratch3-sound-from-library]]]

\--- /task \---

\--- task \---

Escolhe o som 'computer beeps' e clica em OK.

![sons 'Computer Beep' 1 e 2 da biblioteca de sons](images/poetry-beeps.png)

\--- /task \---

\--- task \---

Acrescenta um bloco `toca o som`{:class="block3sound"}, para que o som seja reproduzido imediatamente antes do início da animação.

![ator computador](images/computer-sprite.png)

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