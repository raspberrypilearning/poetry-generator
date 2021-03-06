## Mais poesia

O teu poema é bastante curto - vamos aumentá-lo!

--- task ---

Usemos advérbios na próxima linha do teu poema. Um **advérbio** é uma palavra que descreve um verbo. Cria outra lista chamada advérbios e adiciona-lhe estas 3 palavras:

![lista com as palavras ruidosamente, silenciosamente, interminavelmente](images/poetry-adverbs.png)

--- /task ---

--- task ---

Adiciona esta linha ao código do ator computador, para dizer um advérbio ao acaso na próxima linha do teu poema:

![ator computador](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Aqui está o teu poema…] for (2) seconds
say (join [Eu ](item (pick random (1) to (length of [verbos v])) of [verbos v])) for (2) seconds
+say (item (pick random (1) to (length of [advérbios v])) of [advérbios v]) for (2) seconds
```

--- /task ---

--- task ---

Testa o teu código algumas vezes. Deverás ver um poema diferente a cada vez.

![balões de diálogo com advérbios ao acaso](images/poetry-adverb-test.png)

--- /task ---

--- task ---

Adiciona uma lista de substantivos ao teu projeto. Um **substantivo** é um lugar ou uma coisa.

![uma lista de substantivos com as palavras mar, luar, arvoredo](images/poetry-nouns.png)

--- /task ---

--- task ---

Acrescenta código de forma a usar os substantivos no teu poema.

![ator computador](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Aqui está o teu poema…] for (2) seconds
say (join [Eu ](item (pick random (1) to (length of [verbos v])) of [verbos v])) for (2) seconds
say (item (pick random (1) to (length of [advérbios v])) of [advérbios v]) for (2) seconds
+say (join [pelo ](item (pick random (1) to (length of [nouns v])) of [nouns v])) for (2) seconds
```

--- /task ---

--- task ---

Adiciona uma lista de substantivos ao teu projeto. Um **adjetivo** é uma palavra descritiva.

![uma lista de adjetivos com as palavras feliz, cansado, esfomeado](images/poetry-adjectives.png)

--- /task ---

--- task ---

Acrescenta código de forma a usar os adjetivos no teu poema:

![ator computador](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Aqui está o teu poema…] for (2) seconds
say (join [Eu ](item (pick random (1) to (length of [verbos v])) of [verbos v])) for (2) seconds
say (item (pick random (1) to (length of [advérbios v])) of [advérbios v]) for (2) seconds
say (join [pelo ](item (pick random (1) to (length of [nouns v])) of [nouns v])) for (2) seconds
+ say (join [Sinto-me ](item (pick random (1) to (length of [adjectives v])) of [adjectives v])) for (2) seconds
```

--- /task ---

--- task ---

Podes clicar nas caixas junto às tuas listas para as ocultar.

![lista de variáveis com as caixas de seleção preenchidas](images/poetry-lists-tick.png)

--- /task ---

--- task ---

Testa o teu novo poema.

--- /task ---