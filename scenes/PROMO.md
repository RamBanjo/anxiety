# intro

`SceneSetup.intro();`

# intro-play-button

(...51)

[เล่น!](#intro-start) `publish("intro-to-game-1"); Game.OVERRIDE_CHOICE_LINE=true;`

# intro-start

(...500)

`clearText()`

n3: ก่อนเราจะเรี่มกัน *คุณ* อยากอ่านเร็วแค่ไหน?

`publish("show_options_bottom")`

# intro-start-2

n3: เรามาเรี่มเรี่องของเรากันเลย...

```
publish("hide_tabs");
clearText();
```

(...1000)

`publish("intro-to-game-2")`

n2: นี่คือมนุษย์

(...600)

`clearText()`

(...300)

`publish("intro-to-game-3")`

# act1

```
SceneSetup.act1();
publish("hide_tabs");
music('battle', {volume:0.5});
```

(...300)

n: และนี่คือความวิตกของมนุษย์

n: _คุณ_ คือความวิตก

(#act1_normal)


# act1_normal

```
hong({body:"putaway"});
sfx("rustle");
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: ม่าย ไม ไม่ ชั้นจะไม่ฟัง ดูมือถือดีกว่า

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: หน้าที่ของคุณคือปกป้องมนุษย์ของคุณจาก *อันตราย*

`bb({eyes:"look", mouth:"small_lock", body:"fear"})`

b: เฮือก! นายเอาเวลาชีวิตไปไถทวิต! อีกแล้ว!

```
bb({eyes:"normal", mouth:"normal", body:"normal"});
hong({eyes:"annoyed"});
```

h: เออสงสัยจังว่าทำไมถึงไม่อยากนั่งฟังเสียงในหัวให้บ่อยกว่านี้

`hong({eyes:"neutral"});`

n: เร็วเข้า เตือนเขาถึง *อันตราย!*

```
bb({eyes:"look"});
```

[แย่ละ ดูข่าวไม่ดีนั่นสิ!](#act1d_news)

[แย่ละ มีคนทวิต *เรา* ลับหลังเปล่า?](#act1d_subtweet)

[ดูนั่นสิ รูปแมวกินนม](#act1d_milk)

# act1d_milk

`hong({mouth:"smile", eyes:"surprise"});`

h: เออ น่ารักดี ชั--

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: แมวย่อยนมไม่ได้โว้ย พวกเราชอบการทรมานสัตว์!! พวกเรามันถ่อย!!

(...200)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
attack("20p", "bad");
publish("hp_show");
```



