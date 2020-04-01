## Animatie van de analytische machine

Laten we de computer animeren, zodat het lijkt alsof deze poëzie genereert.

--- task ---

Klik op de computer sprite en voeg deze code toe na het eerste `zeg`{:class="block3looks"} blok:

Je vindt de `herhaal`{:class="block3control"} en `wacht`{:class="block3control"} blokken in de sectie `Besturen`{:class="block3control"}.

![computer sprite](images/computer-sprite.png)

```blocks3
wanneer op deze sprite wordt geklikt
zeg [Hier is je gedicht...] (2) sec.
+ herhaal (10)
    draai links (5) graden
    wacht (0.1) seconden
    draai rechts (5) graden
    wacht (0.1 ) seconden  
einde
zeg (voeg [Ik ] en (item (willekeurig getal tussen (1) en (lengte van [werkwoorden v])) van [werkwoorden v]) samen) (2) sec.
zeg (item (willekeurig getal tussen (1) en (lengte van [bijwoorden v])) van [bijwoorden v]) (2) sec.
zeg (voeg [bij de] (item (willekeurig getal tussen (1) en (lengte van [zelfstandige naamwoorden v])) van [ zelfstandige naamwoorden v] samen)) (2) sec.
zeg (voeg [Ik voel me ] (item (willekeurig getal tussen (1) en (lengte van [bijvoeglijke naamwoorden v])) van [bijvoeglijke naamwoorden v] samen)) (2) sec.
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
wanneer op deze sprite wordt geklikt
zeg [Hier is je gedicht ...] (2) sec.
+ start geluid (computer beeps1 v)
herhaal (10)
    draai links (5) graden
    wacht (0.1) seconden
    draai rechts (5) graden
    wachten (0.1) seconden  
einde
zeg (voeg [Ik ] en (item (willekeurig getal tussen (1) en (lengte van [werkwoorden v])) van [werkwoorden v] samen)) (2) sec.
zeg (item (willekeurig getal tussen (1) en (lengte van [bijwoorden v])) van [bijwoorden v]) (2) sec.
zeg (voeg [bij de ] (item (willekeurig getal tussen (1) en (lengte van [zelfstandige naamwoorden v])) van [zelfstandige naamwoorden v] samen)) (2) sec.
zeg (voeg [Ik voel me ] (item (willekeurig getal tussen (1) en (lengte van [bijvoeglijke naamwoorden v])) van [bijvoeglijke naamwoorden v] samen)) (2) sec.
```

--- /task ---