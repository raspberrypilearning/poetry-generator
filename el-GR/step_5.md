## Η Αναλυτική Μηχανή

Ας προγραμματίσουμε τον υπολογιστή της Ada (που ονομάζεται 'Αναλυτική Μηχανή') για να δημιουργήσουμε ποίηση.

\--- task \---

Πρόσθεσε αυτόν τον κώδικα στο αντικείμενο 'Υπολογιστής', έτσι ώστε να μιλάει όταν κάνεις κλικ:

![computer sprite](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Here is your poem...] for (2) seconds
```

\--- /task \---

\--- task \---

Για να δημιουργήσεις ένα τυχαίο ποίημα, πρώτα θα χρειαστείς μια **λίστα** των λέξεων που πρέπει να χρησιμοποιηθούν. Για να δημιουργήσεις μια νέα λίστα, κάνε κλικ στην καρτέλα `Μεταβλητές`{:class="block3variables"}.

Ας χρησιμοποιήσουμε τα **ρήματα** (λέξεις δράσης) στην πρώτη γραμμή του ποιήματός σου. Δημιούργησε μια λίστα που ονομάζεται `ρήματα`{:class="block3variables"}.

[[[generic-scratch3-make-list]]]

\--- /task \---

\--- task \---

Η νέα σου λίστα θα είναι κενή. Click the `+` at the bottom of your empty list and add these verbs:

![list with the + highlighted](images/poetry-verbs-annotated.png)

\--- /task \---

\--- task \---

The first line of your poem should be the word "I", followed by a random verb.

To create this line of poetry, you need to:

1. `Pick a random number`{:class="block3operators"} between `1` and the `length of the verbs list`{:class="block3variables"}:
    
    ```blocks3
    (pick random (1) to (length of [verbs v]))
    ```

2. Use this block to get a random `item`{:class="block3variables"} from the `verbs`{:class="block3variables"} list:
    
    ```blocks3
    (item (pick random (1) to (length of [verbs v]) :: +) of [verbs v])
    ```

3. `Join`{:class="block3operators"} "I " with the random verb to create the first line of your poem:
    
    ```blocks3
    (join [I ] (item (pick random (1) to (length of [verbs v])) of [verbs v] :: +))
    ```

4. Use a `say`{:class="block3looks"} block to display the line of poetry:
    
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

\--- /task \---

\--- task \---

Test your code a few times. Your computer should choose a random word from the `verbs`{:class="block3variables"} list each time.

![3 speech bubbles saying different things](images/poetry-random-test.png)

\--- /task \---