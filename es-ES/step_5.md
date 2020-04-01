## El motor analítico

Vamos a programar el ordenador de Ada (llamado el 'Motor Analítico') para generar poesía.

--- task ---

Añade este código a tu objeto "ordenador", para que hable cuando le hagas clic:

![imagen de ordenador](images/computer-sprite.png)

```blocks3
al hacer clic en este objeto
decir [Aquí está tu poema...] durante (2) segundos
```

--- /task ---

--- task ---

Para crear un poema aleatorio, primero necesitarás una **lista** de palabras que usar. Para crear una lista nueva, haz clic en la pestaña `Variables`{:class="block3variables"}.

Vamos a usar **verbos** (palabras de acción) en la primera línea de tu poema. Crea una nueva lista llamada `verbos`{:class="block3variables"}.

[[[generic-scratch3-make-list]]]

--- /task ---

--- task ---

Tu nueva lista estará vacía. Haz clic en `+` al final de tu lista vacía y añade estos verbos conjugados en primera persona:

![lista con el + marcado](images/poetry-verbs-annotated.png)

--- /task ---

--- task ---

La primera línea de tu poema debe ser la palabra "Yo", seguida de un verbo al azar.

Para crear una línea de poesía, necesitas:

1. `número aleatorio`{:class="block3operators"} entre `1` y `longitud de verbos`{:class="block3variables"}:
    
    ```blocks3
    (número aleatorio entre (1) y (longitud de [verbos v]))
    ```

2. Usa este bloque para escoger un `elemento`{:class="block3variables"} al azar de la lista de `verbos`{:class="block3variables"}:
    
    ```blocks3
    (elemento (número aleatorio entre (1) y (longitud de [verbos v]) :: +) de [verbos v])
    ```

3. `Unir`{:class="block3operators"} "Yo " con el verbo al azar para crear la primera línea de tu poema:
    
    ```blocks3
    (unir[Yo ] (elemento(número aleatorio entre (1) y (longitud de [verbos v])) de [verbos v] :: +))
    ```

4. Usa un bloque `decir`{:class="block3looks"} para mostrar una línea de poesía:
    
    ```blocks3
    decir (unir[Yo ](elemento(número aleatorio entre (1) y (longitud de [verbos v])) de [verbos v]) :: +) durante (2) segundos
    ```

Tu código debería verse así:

![imagen de ordenador](images/computer-sprite.png)

```blocks3
al hacer clic en este objeto
decir [Aquí está tu poema...] durante (2) segundos
+ decir (unir[Yo ](elemento(número aleatorio entre (1) y (longitud de [verbos v])) de [verbos v])) durante (2) segundos
```

--- /task ---

--- task ---

Prueba tu código unas cuantas veces. Tu ordenador debería elegir una palabra al azar de la lista de `verbos`{:class="block3variables"} cada vez.

![3 burbujas de voz que dicen cosas diferentes](images/poetry-random-test.png)

--- /task ---