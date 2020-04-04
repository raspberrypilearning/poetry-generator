## O Motor Analítico

Vamos programar o computador da Ada (chamado 'Motor Analítico') de forma a criar poesia.

--- task ---

Acrescenta este código ao teu ator 'Computador', para que fale quando é clicado:

![ator computador](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Aqui está o teu poema…] for (2) seconds
```

--- /task ---

--- task ---

Para criar um poema aleatório, primeiro terás que criar uma **lista** de palavras a usar. Para criar uma lista, clica na categoria `Dados`{:class="block3variables"}.

Vamos usar **verbos** (palavras de ação) na primeira linha do teu poema. Cria uma nova variável chamada `pontuação`{:class="block3variables"}.

[[[generic-scratch3-make-list]]]

--- /task ---

--- task ---

A tua nova lista vai estar vazia. Clica no `+` ao fundo da tua lista vazia e adiciona estes verbos:

![lista com o + destacado](images/poetry-verbos-annotated.png)

--- /task ---

--- task ---

A primeira linha do teu poema deve ser começar com a palavra "Eu", seguida de um verbo aleatório.

Para criar esta linha de poesia, vais necessitar de:

1. Escolhe `um valor ao acaso`{:class="block3operators"} entre `1` e o `comprimento da lista de verbos`{:class="block3variables"}:
    
    ```blocks3
    (pick random (1) to (length of [verbos v]))
    ```

2. Usa este bloco para obter um `elemento`{:class="block3variables"} ao acaso a partir da lista de `verbos`{:class="block3variables"}:
    
    ```blocks3
    (item (pick random (1) to (length of [verbos v]) :: +) of [verbos v])
    ```

3. Faz a `junção`{:class="block3operators"} de "Eu" com um verbo ao acaso para criar a primeira linha do teu poema:
    
    ```blocks3
    (join [Eu ] (item (pick random (1) to (length of [verbos v])) of [verbos v] :: +))
    ```

4. Usa o bloco `diz` {:class="block3looks"} para mostrar a linha de poesia:
    
    ```blocks3
    say (join [Eu ](item (pick random (1) to (length of [verbos v])) of [verbos v]) :: +) for (2) seconds
    ```

O teu código deverá ter este aspeto:

![ator computador](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Aqui está o teu poema…] for (2) seconds
+ say (join [Eu ](item (pick random (1) to (length of [verbos v])) of [verbos v])) for (2) seconds
```

--- /task ---

--- task ---

Testa o teu código algumas vezes. O teu computador deverá escolher uma palavra ao acaso a partir da lista de `verbos`{:class="block3variables"} a cada vez.

![3 balões de diálogo a dizer coisas diferentes](images/poetry-random-test.png)

--- /task ---