## The Analytical Engine

Let's program Ada's computer (called the 'Analytical Engine') to generate poetry.

--- task ---

Add this code to your 'Computer' sprite, so that it speaks when clicked:

![computer sprite](images/computer-sprite.png)

```blocks
when this sprite clicked
say [Here is your poem...] for (2) secs
```

--- /task ---

--- task ---

To create a random poem, first you'll need a __list__ of words to use. To create a new list, click the `Data`{:class="blockdata"} tab.

Let's use __verbs__ (action words) in the first line of your poem. Create a new list called 'verbs'.

![new list dialog box](images/poetry-list.png)

--- /task ---

--- task ---

Your new list will be empty. Click the `+` at the bottom of your empty list and add these verbs:

![list with the + highlighted](images/poetry-verbs.png)

--- /task ---

--- task ---

The first line in your poem will be the word "I", followed by a random verb. This is the code that you'll need to add:

![computer sprite](images/computer-sprite.png)

```blocks
when this sprite clicked
say [Here is your poem...] for (2) secs
+ say (join [I ] (item (random v) of [verbs v])) for (2) secs
```

--- /task ---

--- task ---

Test your code a few times. Your computer should say a random word from your verb list each time.

![3 speech bubbles saying different things](images/poetry-random-test.png)

--- /task ---
