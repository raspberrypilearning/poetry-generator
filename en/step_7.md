## Animating the Analytical Engine

Let's animate your computer, so that it looks like it's generating poetry.

--- task ---

Click on your computer sprite, and add this code after the first `say`{:class="blocklooks"} block:

You'll find the `repeat`{:class="blockcontrol"} and `wait`{:class="blockcontrol"} blocks are in the `Control`{:class="blockcontrol"} section.

![computer sprite](images/computer-sprite.png)

```blocks
when this sprite clicked
say [Here is your poem...] for (2) secs
+ repeat (10)
	turn left (5) degrees
	wait (0.1) secs
	turn right (5) degrees
	wait (0.1) secs	
end
say (join [I ] (item (random v) of [verbs v])) for (2) secs
say (item (random v) of [adverbs v]) for (2) secs
say (join [by the ] (item (random v) of [nouns v])) for (2) secs
say (join [I feel ] (item (random v) of [adjectives v])) for (2) secs
```

--- /task ---

--- task ---

Test your project. You should see the computer shake before producing a poem!

![computer sprite shaking back and forth](images/poetry-animate-test.png)

--- /task ---

--- task ---

Click the 'Sounds' tab, and click 'Choose sound from library'.

![choose sound from library icon highlighted](images/poetry-sound.png)

--- /task ---

--- task ---

Choose a 'computer beeps' sound and click OK.

![computer beeps 1 and 2 sounds in sound library](images/poetry-beeps.png)

--- /task ---

--- task ---

Add a `play sound`{:class="blocksound"} block, to play your sound just before your animation starts.

![computer sprite](images/computer-sprite.png)

```blocks
when this sprite clicked
say [Here is your poem...] for (2) secs
+ play sound [computer beeps1 v]
repeat (10)
	turn left (5) degrees
	wait (0.1) secs
	turn right (5) degrees
	wait (0.1) secs	
end
say (join [I ] (item (random v) of [verbs v])) for (2) secs
say (item (random v) of [adverbs v]) for (2) secs
say (join [by the ] (item (random v) of [nouns v])) for (2) secs
say (join [I feel ] (item (random v) of [adjectives v])) for (2) secs
```

--- /task ---
