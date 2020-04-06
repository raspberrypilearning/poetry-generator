## Ενεργοποιώντας την Αναλυτική Μηχανή

Ας ενεργοποιήσουμε τον Υπολογιστή σου, έτσι ώστε να φαίνεται σαν να δημιουργεί ποίηση.

--- task ---

Κάνε κλικ στο αντικείμενο Υπολογιστής σου και πρόσθεσε αυτόν τον κώδικα μετά από το πρώτο μπλοκ `πες`{:class="block3looks"}:

Θα βρεις ότι τα μπλοκ `επανέλαβε`{:class="block3control"} και `περίμενε`{:class="block3control"} βρίσκονται στην ενότητα `Έλεγχος`{:class="block3control"}.

![αντικείμενο υπολογιστή](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Εδώ είναι το ποίημα σου…] for (2) seconds
+ repeat (10)
    turn left (5) degrees
    wait (0.1) seconds
    turn right (5) degrees
    wait (0.1) seconds  
end
say (join [Εγώ ](item (pick random (1) to (length of [ρήματα v])) of [ρήματα v])) for (2) seconds
say (item (pick random (1) to (length of [επιρρήματα v])) of [επιρρήματα v]) for (2) seconds
say (join [εκ ](item (pick random (1) to (length of [ουσιαστικά v])) of [ουσιαστικά v])) for (2) seconds
say (join [Αισθάνομαι ](item (pick random (1) to (length of [επίθετα v])) of [επίθετα v])) for (2) seconds
```

--- /task ---

--- task ---

Δοκίμασε το έργο σου. Θα πρέπει να δεις τον Υπολογιστή να κουνιέται πριν παράγει ένα ποίημα!

![αντικείμενο υπολογιστή που κινείται μπρος και πίσω](images/poetry-animate-test.png)

--- /task ---

--- task ---

Κάνε κλικ στην καρτέλα 'Ήχοι' και κάνε κλικ στο εικονίδιο 'Επιλογή ήχου' στο κάτω αριστερό μέρος.

[[[generic-scratch3-sound-from-library]]]

--- /task ---

--- task ---

Επίλεξε έναν ήχο "μπιπ υπολογιστή" και πάτησε ΟΚ.

![οι ήχοι μπιπ 1 και 2 υπολογιστή στη βιβλιοθήκη ήχων](images/poetry-beeps.png)

--- /task ---

--- task ---

Πρόσθεσε ένα μπλοκ `παίξε ήχο`{:class="block3sound"}, για να παίξεις τον ήχο πριν ξεκινήσει η κίνηση.

![αντικείμενο υπολογιστή](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Εδώ είναι το ποίημα σου…] for (2) seconds
+ start sound (computer beeps1 v)
repeat (10)
    turn left (5) degrees
    wait (0.1) seconds
    turn right (5) degrees
    wait (0.1) seconds  
end
say (join [Εγώ ](item (pick random (1) to (length of [ρήματα v])) of [ρήματα v])) for (2) seconds
say (item (pick random (1) to (length of [επιρρήματα v])) of [επιρρήματα v]) for (2) seconds
say (join [εκ ](item (pick random (1) to (length of [ουσιαστικά v])) of [ουσιαστικά v])) for (2) seconds
say (join [Αισθάνομαι ](item (pick random (1) to (length of [επίθετα v])) of [επίθετα v])) for (2) seconds
```

--- /task ---