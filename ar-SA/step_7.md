## تحريك المحرك التحليلي

دعونا نقوم بتحريك جهاز الكمبيوتر الخاص بك، بحيث يبدو أنه يولد الشعر.

\--- task \---

Click on your computer sprite, and add this code after the first `say`{:class="block3looks"} block:

ستجد كتل `كرر`{: فئة = "block3control"} و `أنتظر`{: فئة = "block3control"} الموجودة في قسم `التحكم`{: فئة = "block3control"}.

![الكمبيوتر](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Here is your poem...] for (2) seconds
+ repeat (10)
    turn left (5) degrees
    wait (0.1) seconds
    turn right (5) degrees
    wait (0.1) seconds  
end
say (join [I ](item (pick random (1) to (length of [verbs v])) of [verbs v])) for (2) seconds
say (item (pick random (1) to (length of [adverbs v])) of [adverbs v]) for (2) seconds
say (join [by the ](item (pick random (1) to (length of [nouns v])) of [nouns v])) for (2) seconds
say (join [I feel ](item (pick random (1) to (length of [adjectives v])) of [adjectives v])) for (2) seconds
```

\--- /task \---

\--- task \---

اختبر مشروعك. يجب أن ترى اهتزاز الكمبيوتر قبل إنتاج قصيدة!

![الكمبيوتر يهتز ذهاباً وإياباً](images/poetry-animate-test.png)

\--- /task \---

\--- task \---

انقر فوق علامة التبويب "الأصوات" ، وانقر فوق الرمز "اختيار صوت" في أسفل اليسار.

[[[generic-scratch3-sound-from-library]]]

\--- /task \---

\--- task \---

اختر صوت "computer beeps" وانقر فوق "موافق".

![يصدر الكمبيوتر صوتًا 1 و 2 في مكتبة الصوت](images/poetry-beeps.png)

\--- /task \---

\--- task \---

إضف كتلة `شغل الصوت`{: فئة = "block3sound"}، للعب الصوت فقط قبل البدء بتحريك جهازك الخاص.

![الكمبيوتر](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Here is your poem...] for (2) seconds
+ start sound (computer beeps1 v)
repeat (10)
    turn left (5) degrees
    wait (0.1) seconds
    turn right (5) degrees
    wait (0.1) seconds  
end
say (join [I ](item (pick random (1) to (length of [verbs v])) of [verbs v])) for (2) seconds
say (item (pick random (1) to (length of [adverbs v])) of [adverbs v]) for (2) seconds
say (join [by the ](item (pick random (1) to (length of [nouns v])) of [nouns v])) for (2) seconds
say (join [I feel ](item (pick random (1) to (length of [adjectives v])) of [adjectives v])) for (2) seconds
```

\--- /task \---