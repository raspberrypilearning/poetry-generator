## Animatie van de analytische machine

Laten we de computer animeren, zodat het lijkt alsof deze poëzie genereert.

--- task ---

Klik op de computer sprite en voeg deze code toe na het eerste `zeg`{:class="block3looks"} blok:

Je vindt de `herhaal`{:class="block3control"} en `wacht`{:class="block3control"} blokken in de sectie `Besturen`{:class="block3control"}.

![computer sprite](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Hier is je gedicht...] for (2) seconds
+ repeat (10)
	turn left (5) degrees
	wait (0.1) seconds
	turn right (5) degrees
	wait (0.1) seconds	
end
say (join [Ik ](item (pick random (1) to (length of [werkwoorden v])) of [werkwoorden v])) for (2) seconds
say (item (pick random (1) to (length of [bijwoorden v])) of [bijwoorden v]) for (2) seconds
say (join [bij de ](item (pick random (1) to (length of [zelfstandige naamwoorden v])) of [zelfstandige naamwoorden v])) for (2) seconds
say (join [Ik voel me ](item (pick random (1) to (length of [bijvoeglijke naamwoorden v])) of [bijvoeglijke naamwoorden v])) for (2) seconds
```

--- /task ---

--- task ---

Test je project. Je zou de computer moeten zien schudden voordat je een gedicht maakt!

![computer sprite schudt heen en weer](images/poetry-animate-test.png)

--- /task ---

--- task ---

Klik op het tabblad 'Geluiden' en klik linksonder op het pictogram 'Kies een geluid'.

[[[generic-scratch3-sound-from-library]]]

--- /task ---

--- task ---

Kies een 'computer beep' geluid en klik op OK.

![computer beeps 1 en 2 geluiden in geluidsbibliotheek](images/poetry-beeps.png)

--- /task ---

--- task ---

Voeg een `start geluid`{:class="block3sound"} toe om een geluid af te spelen net voordat je animatie begint.

![computer sprite](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Hier is je gedicht...] for (2) seconds
+ start sound (computer beeps1 v)
repeat (10)
	turn left (5) degrees
	wait (0.1) seconds
	turn right (5) degrees
	wait (0.1) seconds	
end
say (join [Ik ](item (pick random (1) to (length of [werkwoorden v])) of [werkwoorden v])) for (2) seconds
say (item (pick random (1) to (length of [bijwoorden v])) of [bijwoorden v]) for (2) seconds
say (join [bij de ](item (pick random (1) to (length of [zelfstandige naamwoorden v])) of [zelfstandige naamwoorden v])) for (2) seconds
say (join [Ik voel me ](item (pick random (1) to (length of [bijvoeglijke naamwoorden v])) of [bijvoeglijke naamwoorden v])) for (2) seconds
```

--- /task ---