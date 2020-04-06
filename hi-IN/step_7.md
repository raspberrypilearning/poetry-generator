## एनालिटिकल यन्त्र को एनिमेट करना

चलिए आपके कंप्यूटर को एनिमेट करते है, ताकि ऐसा लगे की वो कवितायेँ जेनेरेट कर रहा हैं |

\--- task \---

अपने कंप्यूटर के स्प्राइट पर क्लिक करें, और इस कोड को पहले `say`{:class="block3looks"} ब्लॉक के बाद जोड़ें:

आपको `repeat`{:class="block3control"} और `wait`{:class="block3control"} ब्लॉक्स ये `Control`{:class="block3control"} खाने में मिलेगा |

![computer sprite](images/computer-sprite.png)

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

अपने प्रोजेक्ट का परीक्षण करें। कविता निर्माण करने से पहले आपका कंप्यूटर थोड़ा हिलना चाहिए!

![computer sprite shaking back and forth](images/poetry-animate-test.png)

\--- /task \---

\--- task \---

'Sounds' बटन पर क्लिक करें, और नीचे बाईं ओर की तरफ 'Choose a Sound' वाले विकल्प पे क्लिक करें।

[[[generic-scratch3-sound-from-library]]]

\--- /task \---

\--- task \---

'computer beeps' वाली ध्वनि को चुनें और OK पर क्लिक करें।

![computer beeps 1 and 2 sounds in sound library](images/poetry-beeps.png)

\--- /task \---

\--- task \---

अपने एनीमेशन के तुरंत पहले आवाज़ सुनने के लिए, `start sound`{:class="block3sound"} वाला ब्लॉक जोड़ें |

![computer sprite](images/computer-sprite.png)

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