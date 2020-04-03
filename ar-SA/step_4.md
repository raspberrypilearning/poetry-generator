## إخبار آدا بأسمك

قدمت ادا نفسها، لكنها لا تعرف اسمك!

\--- task \---

اسحب كتلة `اسأل`{: class = "block3sensing"} (من قسم التحسس ``{: class = "block3sensing"}) إلى الكود الخاص بك. هذا ما ينبغي ان تبدو عليه تعليماتك البرمجية:

![كائن ادا](images/ada-sprite.png)

```blocks3
when this sprite clicked
say [Hi, I'm Ada!] for (2) seconds
+ ask [What's your name?] and wait
```

\--- /task \---

\--- task \---

انقر على ادا لأختبار الكود البرمجي الخاص بك. يجب أن تسألك ادا عن اسمك، والذي يمكنك كتابته!

![كائن ادا يسأل ما هو اسمك](images/poetry-input.png)

\--- /task \---

\--- task \---

يمكننا استخدام **متغير** لتخزين اسمك. انقر فوق `المتغيرات`{: class = "block3variables"} ، ثم "إنشاء متغير". نظرًا لأنه سوف يتم استخدام هذا المتغير لتخزين اسمك، فلندعو المتغير... `الاسم`{: class = "block3variables"}!

[[[generic-scratch3-add-variable]]]

\--- /task \---

\--- task \---

لتخزين اسمك، انقر فوق علامة التبويب `المتغيرات`{: class = "block3variables"} ، ثم اسحب كتلة `إجعل الاسم مساوياً`: {= class = "block3variables"} إلى نهاية الكود البرمجي الخاص بك.

![كائن ادا](images/ada-sprite.png)

```blocks3
when this sprite clicked
say [Hi, I'm Ada!] for (2) seconds
ask [What's your name?] and wait
+ set [name v] to [0]
```

\--- /task \---

\--- task \---

استخدم كتلة `الإجابة`{: class = "block3sensing"} لتخزين الإجابة التي تكتبها.

![كائن ادا](images/ada-sprite.png)

```blocks3
when this sprite clicked
say [Hi, I'm Ada!] for (2) seconds
ask [What's your name?] and wait
set [name v] to (answer :: +)
```

\--- /task \---

\--- task \---

أنقر على ادا لأختبار الكود البرمجي الخاص بك، وأدخل اسمك عندما يُطلب منك ذلك. يجب أن ترى أن اسمك قد تم تخزينه في متغير الاسم `{`: class = "block3variables"}.

![لقطة الشاشة](images/poetry-name-test.png)

\--- /task \---

\--- task \---

يمكنك الآن الاستفادة من اسمك في التعليمات البرمجية الخاصة بك. أضف هذا الكود البرمجي:

![كائن ادا](images/ada-sprite.png)

```blocks3
when this sprite clicked
say [Hi, I'm Ada!] for (2) seconds
ask [What's your name?] and wait
set [name v] to (answer)
+say (join [Hi ] (name)) for (2) seconds 
```

لإنشاء هذا الكود البرمجي:

1. اسحب كتلة `اربط`{: class = "blockoperators"} إلى الكتلة `قل`{: class = "blocklooks"}
    
    ```blocks3
    say (join [apple] [banana] :: +) for (2) seconds
    ```

2. اضف كتلة `الاسم`{: فئة = "blockdata"} الى كتلة `اربط`{: فئة = "blockoperators"}.
    
    ```blocks3
    say (join [Hi] (name :: variables +)) for (2) seconds
    ```

\--- /task \---

\--- task \---

لإخفاء متغير `الأسم`{: فئة = "block3variables"} الخاص بك من المنصة، انقر فوق العلامة بجانب المتغير.

![متغير الاسم](images/poetry-tick-annotated.png)

\--- /task \---

\--- task \---

اختبر الكود البرمجي الجديد. يجب أن تقول لك ادا مرحباً، باستخدام اسمك!

![لقطة الشاشة](images/poetry-name-test2.png)

إذا لم تكن هناك مسافة بين كلمة "مرحبا" واسمك، فستحتاج إلى إضافة مسافة إلى الكود البرمجي بنفسك!

\--- /task \---

\--- task \---

أخيرًا، أضف هذا الكود البرمجي لشرح ما يجب فعله بعد ذلك:

![كائن ادا](images/ada-sprite.png)

```blocks3
when this sprite clicked
say [Hi, I'm Ada!] for (2) seconds
ask [What's your name?] and wait
set [name v] to (answer)
say (join [Hi ] (name)) for (2) seconds 
+ say [Click the computer to generate a poem.] for (2) seconds 
```

\--- /task \---

\--- task \---

اختبر الكود البرمجي الخاص ب ادا للمرة الأخيرة، للتأكد من أن كل شيء يعمل.

\--- /task \---