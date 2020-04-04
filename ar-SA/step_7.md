## تحريك المحرك التحليلي

دعونا نقوم بتحريك جهاز الكمبيوتر الخاص بك، بحيث يبدو أنه يولد الشعر.

--- task ---

انقر على جهاز الكمبيوتر الخاص بك، وأضف هذا الرمز بعد أول كتلة `قل`{:class="block3looks"}:

ستجد كتل `كرر`{:class= "block3control"} و `أنتظر`{:class="block3control"} الموجودة في قسم `التحكم`{:class="block3control"}.

![كائن الكمبيوتر](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [هذه هي قصيدتك…] for (2) seconds
+ repeat (10)
    turn left (5) degrees
    wait (0.1) seconds
    turn right (5) degrees
    wait (0.1) seconds  
end
say (join [أنا ](item (pick random (1) to (length of [الأفعال v])) of [الأفعال v])) for (2) seconds
say (item (pick random (1) to (length of [ظرف الحال v])) of [ظرف الحال v]) for (2) seconds
say (join [بواسطة ](item (pick random (1) to (length of [الأسماء v])) of [الأسماء v])) for (2) seconds
say (join [انا أشعر ](item (pick random (1) to (length of [الصفات v])) of [الصفات v])) for (2) seconds
```

--- /task ---

--- task ---

اختبر مشروعك. يجب أن ترى اهتزاز الكمبيوتر قبل إنتاج قصيدة!

![كائن الكمبيوتر يهتز ذهاباً وإياباً](images/poetry-animate-test.png)

--- /task ---

--- task ---

انقر فوق علامة التبويب "الأصوات" ، وانقر فوق الرمز "اختيار صوت" في أسفل اليسار.

[[[generic-scratch3-sound-from-library]]]

--- /task ---

--- task ---

اختر صوت "computer beeps" وانقر فوق "موافق".

![يصدر الكمبيوتر صوتًا 1 و 2 في مكتبة الصوت](images/poetry-beeps.png)

--- /task ---

--- task ---

إضف كتلة `شغل الصوت`{:class= "block3sound"}، للعب الصوت فقط قبل البدء بتحريك جهازك الخاص.

![كائن الكمبيوتر](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [هذه هي قصيدتك…] for (2) seconds
+ start sound (computer beeps1 v)
repeat (10)
    turn left (5) degrees
    wait (0.1) seconds
    turn right (5) degrees
    wait (0.1) seconds  
end
say (join [أنا ](item (pick random (1) to (length of [الأفعال v])) of [الأفعال v])) for (2) seconds
say (item (pick random (1) to (length of [ظرف الحال v])) of [ظرف الحال v]) for (2) seconds
say (join [بواسطة ](item (pick random (1) to (length of [الأسماء v])) of [الأسماء v])) for (2) seconds
say (join [انا أشعر ](item (pick random (1) to (length of [الصفات v])) of [الصفات v])) for (2) seconds
```

--- /task ---