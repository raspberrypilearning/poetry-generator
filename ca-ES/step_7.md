## Animating the Analytical Engine

Let's animate your computer, so that it looks like it's generating poetry.

+ Click on your computer sprite, and add this code after the first `say`{:class="blocklooks"} block:

```blocks
repeat (10)
    turn left (5) degrees
    wait (0.1) secs
    turn right (5) degrees
    wait (0.1) secs 
end
```

Here's how your code should look:

![screenshot](images/poetry-animate.png)

You'll find the `repeat`{:class="blockcontrol"} and `wait`{:class="blockcontrol"} blocks are in the `Control`{:class="blockcontrol"} section.

+ Test your project. You should see the computer shake before producing a poem!

![screenshot](images/poetry-animate-test.png)

+ Click the 'Sounds' tab, and click 'Choose sound from library'.

![screenshot](images/poetry-sound.png)

+ Choose a 'computer beeps' sound and click OK.

![screenshot](images/poetry-beeps.png)

+ Add a `play sound`{:class="blocksound"} block, to play your sound just before your animation starts.

![screenshot](images/poetry-play.png)