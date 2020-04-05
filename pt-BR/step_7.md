## Animando o Motor Analítico

Vamos animar seu computador, para que pareça estar gerando uma poesia.

--- task ---

Clique em seu ator computador, e adicione este código logo após do primeiro bloco `diga`{:class="block3looks"}:

Você irá encontrar os blocos `repita`{:class="block3control"} e `espere`{:class="block3control"} na categoria `Controle`{:class="block3control"}.

![ator Computador](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Aqui está o seu poema...] for (2) seconds
+ repeat (10)
	turn left (5) degrees
	wait (0.1) seconds
	turn right (5) degrees
	wait (0.1) seconds	
end
say (join [Eu ](item (pick random (1) to (length of [verbos v])) of [verbos v])) for (2) seconds
say (item (pick random (1) to (length of [advérbios v])) of [advérbios v]) for (2) seconds
say (join [pelo ](item (pick random (1) to (length of [substantivos v])) of [substantivos v])) for (2) seconds
say (join [Eu me sinto ](item (pick random (1) to (length of [adjetivos v])) of [adjetivos v])) for (2) seconds
```

--- /task ---

--- task ---

Teste seu projeto. Você vai ver o computador tremendo antes de produzir um poema!

![ator computador tremendo para frente e para trás](images/poetry-animate-test.png)

--- /task ---

--- task ---

Clique na categoria 'Sons', e clique no ícone 'Selecionar um som' no canto inferior esquerdo.

[[[generic-scratch3-sound-from-library]]]

--- /task ---

--- task ---

Escolha o som 'sons de computador' e clique em OK.

![beeps de computador 1 e 2 sons na biblioteca de sons](images/poetry-beeps.png)

--- /task ---

--- task ---

Adicione o bloco `toque o som`{:class="block3sound"}, para que o som seja reproduzido imediatamente antes do início da animação.

![ator Computador](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Aqui está o seu poema...] for (2) seconds
+ start sound (computer beeps1 v)
+ repeat (10)
	turn left (5) degrees
	wait (0.1) seconds
	turn right (5) degrees
	wait (0.1) seconds	
end
say (join [Eu ](item (pick random (1) to (length of [verbos v])) of [verbos v])) for (2) seconds
say (item (pick random (1) to (length of [advérbios v])) of [advérbios v]) for (2) seconds
say (join [pelo ](item (pick random (1) to (length of [substantivos v])) of [substantivos v])) for (2) seconds
say (join [Eu me sinto ](item (pick random (1) to (length of [adjetivos v])) of [adjetivos v])) for (2) seconds
```

--- /task ---