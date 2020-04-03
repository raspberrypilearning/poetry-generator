## 분석 엔진 애니메이션

컴퓨터가 시를 생성하는 것처럼 보이도록 컴퓨터 스프라이트에 애니메이션을 적용 해 봅시다.

\--- task \---

컴퓨터 스프라이트를 클릭하고, 아래 코드를 첫 번째 `말하기`{:class="block3looks"} 블록 이후에 추가하세요:

`반복하기`{:class="block3control"} 블록과 `기다리기`{:class="block3control"} 블록은 `제어`{:class="block3control"} 섹션에서 찾을 수 있을 것입니다.

![컴퓨터 스프라이트](images/computer-sprite.png)

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

프로젝트를 테스트하십시오. 시를 제작하기 전에 컴퓨터 스프라이트가 흔들리는 것을 볼수 있어야 합니다!

![앞 뒤로 흔들리는 컴퓨터 스프라이트](images/poetry-animate-test.png)

\--- /task \---

\--- task \---

'소리' 탭을 클릭하여 ('코드' 탭 옆에 있는 '소리' 탭) 왼쪽 하단에 있는 '소리 고르기' 를 클릭합니다.

[[[generic-scratch3-sound-from-library]]]

\--- /task \---

\--- task \---

'computer beeps' 소리를 클릭하고, OK 버튼을 누르세요.

![사운드 라이브러리 내 내장된 'computer beeps 1, 2' 사운드](images/poetry-beeps.png)

\--- /task \---

\--- task \---

`재생하기`{:class="block3sound"} 블록을 추가하여, 애니메이션이 시작하기 전에 사운드가 연주될 수 있도록 하세요.

![컴퓨터 스프라이트](images/computer-sprite.png)

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