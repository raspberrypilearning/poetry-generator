## Кажем Ади своје име

Ада се представила, али не зна ваше име!

\--- task \---

Превуците блок `аск`{: цласс = "блоцк3сенсинг"} (из одељка `сенсинг`{: цласс = "блоцк3сенсинг"}) на свој код. Ево како би ваш код требао изгледати:

![ада сприте](images/ada-sprite.png)

```blocks3
when this sprite clicked
say [Hi, I'm Ada!] for (2) seconds
+ ask [What's your name?] and wait
```

\--- /task \---

\--- task \---

Кликните на Аду да бисте тестирали свој код. Ада би те требала питати своје име, које можеш уписати!

![ада сприте питајући како се зовеш](images/poetry-input.png)

\--- /task \---

\--- task \---

Можемо користити **променљиву** за чување своје име. Click `Variables`{:class="block3variables"}, and then 'Make a Variable'. Како ће се ова променљива користити за чување вашег имена, назовимо променљиву ... `име`{: цласс = "блоцк3вариаблес"}!

[[[generic-scratch3-add-variable]]]

\--- /task \---

\--- task \---

To store your name, click the `Variables`{:class="block3variables"} tab, and then drag the `set name`{:class="block3variables"} block onto the end of your code.

![ада сприте](images/ada-sprite.png)

```blocks3
when this sprite clicked
say [Hi, I'm Ada!] for (2) seconds
ask [What's your name?] and wait
+ set [name v] to [0]
```

\--- /task \---

\--- task \---

Користите блок `одговор`{: цласс = "блоцк3сенсинг"} да бисте спремили одговор у који сте уписали.

![ада сприте](images/ada-sprite.png)

```blocks3
when this sprite clicked
say [Hi, I'm Ada!] for (2) seconds
ask [What's your name?] and wait
set [name v] to (answer :: +)
```

\--- /task \---

\--- task \---

Кликните на Аду да бисте тестирали свој код и на упит унесите своје име. Требали бисте видети да је ваше име сачувано у променљивој `име`{: цласс = "блоцк3вариаблес"}.

![слика екрана](images/poetry-name-test.png)

\--- /task \---

\--- task \---

Сада можете да користите своје име у свом коду. Додајте овај код:

![ада сприте](images/ada-sprite.png)

```blocks3
when this sprite clicked
say [Hi, I'm Ada!] for (2) seconds
ask [What's your name?] and wait
set [name v] to (answer)
+say (join [Hi ] (name)) for (2) seconds 
```

Да бисте креирали овај код:

1. Превуците блок `придруживања`{: цласс = "блоцкоператорс"} на блок `рецимо`{: цласс = "блоцклоокс"}
    
    ```blocks3
    say (join [apple] [banana] :: +) for (2) seconds
    ```

2. Додајте свој блок `наме`{: цласс = "блоцкдата"} у блок `јоин`{: цласс = "блоккоператорс"}.
    
    ```blocks3
    say (join [Hi] (name :: variables +)) for (2) seconds
    ```

\--- /task \---

\--- task \---

Да бисте сакрили променљиву `наме`{: цласс = "блоцк3вариаблес"} на позорници, кликните на дугме поред променљиве.

![Промените назив променљиве](images/poetry-tick-annotated.png)

\--- /task \---

\--- task \---

Тестирајте свој нови код. Ада би требало да те поздрави, користећи своје име!

![слика екрана](images/poetry-name-test2.png)

Ако између речи „Здраво“ и вашег имена нема размака, мораћете сами да додате размак у код!

\--- /task \---

\--- task \---

На крају додајте овај код да објасните шта даље:

![ада сприте](images/ada-sprite.png)

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

Испитајте Ади код последњи пут како бисте били сигурни да све функционише.

\--- /task \---