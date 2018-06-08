## Més poesia

El teu poema és bastant curt: afegim més text!

+ Anem a utilitzar adverbis a la següent línia del vostre poema. Un **adverbi** és una paraula que descriu un verb. Creeu una altra llista anomenada adverbis i afegiu aquestes 3 paraules:

![captura de pantalla](images/poetry-adverbs.png)

+ Afegiu aquesta línia al codi de l'ordinador, per dir un adverbi a l'atzar a la següent línia del vostre poema:

```blocks
digues (element (aleatori v) de [adverbis v]) durant (2) secs
```

+ Proveu el codi diverses vegades. Hauríeu de veure un poema aleatori cada vegada.

![captura de pantalla](images/poetry-adverb-test.png)

+ Afegiu una llista de substantius al vostre projecte. Un **substantius** és un lloc o una cosa.

![captura de pantalla](images/poetry-nouns.png)

+ Afegiu codi per utilitzar els substantius del vostre poema.

```blocks
digus (uneix (element (aleatori v) de [substantius v])) durant (2) secs
```

+ Afegiu una llista d'adjectius al vostre projecte. Un **adjectiu** és una paraula que descriu.

![captura de pantalla](images/poetry-adjectives.png)

+ Afegiu codi per utilitzar els adjectius del vostre poema:

```blocks
digues (uneix [em sento] (element (aleatori v) de [adjectius v])) durant (2) secs
```

+ Podeu fer clic a les caselles que hi ha al costat de les vostres llistes per ocultar-les.

![captura de pantalla](images/poetry-lists-tick.png)

+ Proveu el vostre nou poema. Aquí teniu el codi que hauria de tenir:

```blocks
quan es cliqui aquest personatge
digues [Aquí està el vostre poema ...] durant (2) secs 
digues (uneix [Jo ] (element (aleatori v) de [verbs v])) durant (2) secs 
digues (element (aleatori v) de [adverbis v]) durant (2) secs 
digues (uneix [amb el] (element (aleatori v) de [substantius v])) durant (2) secs 
digues (uneix) [Em sento] (element (aleatori v) de [adjectius v])) durant (2) secs
```