## The Analytical Engine

Let's program Ada's computer (called the 'Analytical Engine') to generate poetry.

--- task ---

Add this code to your 'Computer' sprite, so that it speaks when clicked:

![computer sprite](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Here is your poem...] for (2) seconds
```

--- /task ---

--- task ---

To create a random poem, first you'll need a __list__ of words to use. To create a new list, click the `Data`{:class="block3variables"} tab.

Let's use __verbs__ (action words) in the first line of your poem. Create a new list called `verbs`{:class="block3variables"}.

[[[generic-scratch3-make-list]]]

--- /task ---

--- task ---

Your new list will be empty. Click the `+` at the bottom of your empty list and add these verbs:

![list with the + highlighted](images/poetry-verbs-annotated.png)

--- /task ---

--- task ---

The first line in your poem will be the word "I", followed by a random verb. 

To do this you should:

1. `Pick a random number`{:class="block3operators"} between `1` and the `length of the verbs list`{:class="block3variables"}.

    ```blocks3
    (pick random (1) to (length of [verbs v]))
    ```

2. Use this block to get a random `item`{:class="block3variables"} from verb the `verbs`{:class="block3variables"} list.

    ```blocks3
    (item (pick random (1) to (length of [verbs v]) :: +) of [verbs v])
    ```

3. `join`{:class="block3operators"} "I " with the random verb to create the first line of your poem.

    ```blocks3
    (join [I ] (item (pick random (1) to (length of [verbs v])) of [verbs v] :: +))
    ```

4. Use a `say`{:class="block3operators"} block to display it.

    ```blocks3
    say (join [I ](item (pick random (1) to (length of [verbs v])) of [verbs v]) :: +) for (2) seconds
    ```

Your code should look like this:

![computer sprite](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Here is your poem...] for (2) seconds
+ say (join [I ](item (pick random (1) to (length of [verbs v])) of [verbs v])) for (2) seconds
```

--- /task ---

--- task ---

Test your code a few times. Your computer should say a random word from your verb list each time.

![3 speech bubbles saying different things](images/poetry-random-test.png)

--- /task ---
