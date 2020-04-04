## Animar o Motor Analítico

Vamos animar o teu computador, para que pareça que está a gerar poesia.

--- task ---

Clica no teu ator computador e adiciona-lhe este código a seguir ao primeiro bloco `diz`{:class="block3looks"}:

Vais encontrar os blocos `repete`{:class="block3control"} e `espera`{:class="block3control"} na categoria `Controlo`{:class="block3control"}.

![ator computador](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Aqui está o teu poema…] for (2) seconds
+ repeat (10)
    turn left (5) degrees
    wait (0.1) seconds
    turn right (5) degrees
    wait (0.1) seconds  
end
say (join [Eu ](item (pick random (1) to (length of [verbos v])) of [verbos v])) for (2) seconds
say (item (pick random (1) to (length of [advérbios v])) of [advérbios v]) for (2) seconds
say (join [pelo ](item (pick random (1) to (length of [substantivos v])) of [substantivos v])) for (2) seconds
say (join [Sinto-me ](item (pick random (1) to (length of [adjetivos v])) of [adjetivos v])) for (2) seconds
```

--- /task ---

--- task ---

Testa o teu projeto. Deverás ver o computador a tremer antes de produzir um poema!

![ator computador a tremer para frente e para trás](images/poetry-animate-test.png)

--- /task ---

--- task ---

Vai ao separador 'Sons' e clica no ícone 'Escolher um Som' que está no canto inferior esquerdo.

[[[generic-scratch3-sound-from-library]]]

--- /task ---

--- task ---

Escolhe o som 'computer beeps' e clica em OK.

![sons 'Computer Beep' 1 e 2 da biblioteca de sons](images/poetry-beeps.png)

--- /task ---

--- task ---

Acrescenta um bloco `toca o som`{:class="block3sound"}, para que o som seja reproduzido imediatamente antes do início da animação.

![ator computador](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Aqui está o teu poema…] for (2) seconds
+ start sound (computer beeps1 v)
repeat (10)
    turn left (5) degrees
    wait (0.1) seconds
    turn right (5) degrees
    wait (0.1) seconds  
end
say (join [Eu ](item (pick random (1) to (length of [verbos v])) of [verbos v])) for (2) seconds
say (item (pick random (1) to (length of [advérbios v])) of [advérbios v]) for (2) seconds
say (join [pelo ](item (pick random (1) to (length of [substantivos v])) of [substantivos v])) for (2) seconds
say (join [Sinto-me ](item (pick random (1) to (length of [adjetivos v])) of [adjetivos v])) for (2) seconds
```

--- /task ---