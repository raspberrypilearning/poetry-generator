## Mais poesia

Seu poema está muito curto - vamos aumentá-lo!

--- task ---

Vamos usar advérbios na próxima linha do seu poema. Um **advérbio** é uma palavra que descreve um verbo. Crie outra lista chamada advérbios e adicione estas 3 palavras:

![lista com as palavras ruidosamente, silenciosamente e infinitamente](images/poetry-adverbs.png)

--- /task ---

--- task ---

Adicione esta linha ao código do seu computador, para dizer um advérbio aleatório na próxima linha do seu poema:

![ator Computador](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Aqui está o seu poema...] for (2) seconds
say (join [Eu ](item (pick random (1) to (length of [verbos v])) of [verbos v])) for (2) seconds
+say (item (pick random (1) to (length of [advérbios v])) of [advérbios v]) for (2) seconds
```

--- /task ---

--- task ---

Teste seu código algumas vezes. Você deve ver um poema aleatório a cada vez.

![balões de fala aleatórias com advérbios](images/poetry-adverb-test.png)

--- /task ---

--- task ---

Adicione uma lista de substantivos ao seu projeto. Um **substantivo** é um lugar ou uma coisa.

![uma lista de substantivos com as palavras mar, lua, árvore](images/poetry-nouns.png)

--- /task ---

--- task ---

Adicione o código para usar os substantivos no seu poema.

![ator Computador](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Aqui está o seu poema...] for (2) seconds
say (join [Eu ](item (pick random (1) to (length of [verbos v])) of [verbos v])) for (2) seconds
say (item (pick random (1) to (length of [advérbios v])) of [advérbios v]) for (2) seconds
+say (join [junte ](item (pick random (1) to (length of [substantivos v])) of [substantivos v])) for (2) seconds
```

--- /task ---

--- task ---

Adicione uma lista de adjetivos ao seu projeto. Um **adjetivo** indica um atributo a um substantivo.

![uma lista de adjetivos: feliz, cansado, com fome](images/poetry-adjectives.png)

--- /task ---

--- task ---

Adicione código para usar os adjetivos em seu poema:

![ator Computador](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Aqui está o seu poema...] for (2) seconds
say (join [Eu ](item (pick random (1) to (length of [verbos v])) of [verbos v])) for (2) seconds
say (item (pick random (1) to (length of [advérbios v])) of [advérbios v]) for (2) seconds
+say (join [junte ](item (pick random (1) to (length of [substantivos v])) of [substantivos v])) for (2) seconds
+ say (join [Eu me sinto ](item (pick random (1) to (length of [adjetivos v])) of [adjetivos v])) for (2) seconds
```

--- /task ---

--- task ---

Para ocultar suas listas você pode clicar nas caixas de seleção ao lado delas.

![lista de variáveis com as caixas de seleção selecionadas](images/poetry-lists-tick.png)

--- /task ---

--- task ---

Teste seu novo poema.

--- /task ---