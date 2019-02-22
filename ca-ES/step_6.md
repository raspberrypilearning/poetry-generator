## Més poesia

El teu poema és bastant curt: afegim més text!

+ Ara utilitzarem adverbis a la següent línia del teu poema. Un **adverbi** és una paraula que descriu un verb. Crea una altra llista anomenada adverbis i afegiu aquestes 3 paraules:

![captura de pantalla](images/poetry-adverbs.png)

+ Afegeix aquesta línia al codi de l'ordinador, per dir un adverbi a l'atzar a la següent línia del teu poema:

```blocks
digues (element (aleatori v) de [adverbis v]) durant (2) secs
```

+ Prova el codi diverses vegades. Hauries de veure un poema aleatori cada vegada.

![captura de pantalla](images/poetry-adverb-test.png)

+ Afegeix una llista de substantius al teu projecte. Un **substantiu** és un lloc o una cosa.

![captura de pantalla](images/poetry-nouns.png)

+ Afegeix codi per utilitzar els substantius al teu poema.

```blocks
digues (uneix (element (aleatori v) de [substantius v])) durant (2) secs
```

+ Afegeix una llista d'adjectius al teu projecte. Un **adjectiu** és una paraula que descriu.

![captura de pantalla](images/poetry-adjectives.png)

+ Afegeix codi per utilitzar els adjectius del teu poema:

```blocks
digues (uneix [em sento] (element (aleatori v) de [adjectius v])) durant (2) secs
```

+ Pots fer clic a les caselles que hi ha al costat de les teves llistes per ocultar-les.

![captura de pantalla](images/poetry-lists-tick.png)

+ Prova el teu nou poema. Aquí s'et mostra com haura de veure's el teu codi:

```blocks
quan es cliqui aquest personatge
digues [Aquí tens el teu poema...] durant (2) secs 
digues (uneix [Jo ] (element (aleatori v) de [verbs v])) durant (2) secs 
digues (element (aleatori v) de [adverbis v]) durant (2) secs 
digues (uneix [amb el] (element (aleatori v) de [substantius v])) durant (2) secs 
digues (uneix) [Em sento] (element (aleatori v) de [adjectius v])) durant (2) secs
```