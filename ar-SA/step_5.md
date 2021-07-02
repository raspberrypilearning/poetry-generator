## المحرك التحليلي

دعنا نبرمج كمبيوتر ادا (يسمى "المحرك التحليلي") لتوليد الشعر.

\--- task \---

أضف هذا الكود البرمجي إلى "الكمبيوتر" الخاص بك، ليتحدث عند النقر عليه:

![الكمبيوتر](images/computer-sprite.png)

```blocks3
when this sprite clicked
say [Here is your poem...] for (2) seconds
```

\--- /task \---

\--- task \---

لإنشاء قصيدة عشوائية، أولاً يجب عليك ان تحصل على **لائحة** من الكلمات لأستخدامها. لإنشاء قائمة جديدة، انقر فوق علامة التبويب `المتغيرات`{:class="block3variables"}.

دعونا نستخدم **أفعال** (افعال الحركة) في السطر الأول من قصيدتك. أنشئ قائمة جديدة تسمى `أفعال`{: class = "block3variables"}.

[[[generic-scratch3-make-list]]]

\--- /task \---

\--- task \---

ستكون قائمتك الجديدة فارغة. انقر فوق `+` أسفل القائمة الفارغة وأضف هذه الأفعال:

![قائمة مع تحديد +](images/poetry-verbs-annotated.png)

\--- /task \---

\--- task \---

يجب أن يكون السطر الأول من قصيدتك الكلمة "أنا" ، متبع بفعل عشوائي.

لإنشاء هذا السطر من الشعر، سوف تحتاج إلى:

1. `اختر رقمًا عشوائيًا`{: class = "block3operators"} بين `1` و `طول قائمة الأفعال`{: class = "block3variables"}:
    
    ```blocks3
    (pick random (1) to (length of [verbs v]))
    ```

2. استخدام هذه الكتلة للحصول على عنصر `عشوائي`{: فئة = "block3variables"} من `الأفعال`{: فئة = "block3variables"} القائمة:
    
    ```blocks3
    (item (pick random (1) to (length of [verbs v]) :: +) of [verbs v])
    ```

3. `اربط`{: class = "block3operators"} "أنا" مع فعل عشوائي لإنشاء السطر الأول من قصيدتك:
    
    ```blocks3
    (join [I ] (item (pick random (1) to (length of [verbs v])) of [verbs v] :: +))
    ```

4. استخدم كتلة { `قل`{: class = "block3looks"} لعرض سطر الشعر:
    
    ```blocks3
    say (join [I ](item (pick random (1) to (length of [verbs v])) of [verbs v]) :: +) for (2) seconds
    ```

يجب أن تبدو التعليمات البرمجية الخاصة بك بالشكل التالي:

![الكمبيوتر](images/computer-sprite.png)

```blocks3
عندما نقر هذا العفريت
قل [إليكم قصيدتك ...] لمدة (2) ثانية
+ قل (انضم [أنا] (البند (اختر عشوائيًا (1) إلى (طول [الأفعال v])) من [الأفعال v ])) لمدة (2) ثانية
```

\--- /task \---

\--- task \---

اختبر الكود البرمجي الخاص بك عدة مرات. يجب أن يختار جهاز الكمبيوتر كلمة عشوائية من قائمة الأفعال `{`: class = "block3variables"} في كل مرة.

![3 فقاعات للكلمات تقول أشياء مختلفة](images/poetry-random-test.png)

\--- /task \---