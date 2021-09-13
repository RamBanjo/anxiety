# act1

```
SceneSetup.act1();
```

(...300)

n: และนี่คือความวิตกของมนุษย์

n: _คุณ_ คือความวิตก

{{if window.localStorage.continueChapter=="replay"}}
(#act1_replay)
{{/if}}

{{if window.localStorage.continueChapter!="replay"}}
(#act1_normal)
{{/if}}



# act1_replay

`hong({mouth:"0_neutral", eyes:"0_neutral"})`

h: ว่าไง! กลับมานี่อีกแล้วเหรอ?

`hong({eyes:"0_neutral"})`

n: หน้าที่ของคุณคือปกป้องมนุษย์ของคุณจาก *อันตราย*

`bb({eyes:"look", mouth:"small_lock"})`

n: เอาเข้าจริงๆแล้ว การเล่นเกมนี้ใหม่เป็น *อันตราย* ต่อเขา

n: เร็วเข้า เตือนเขาสิ!

```
sfx("squeak");
bb({body:"squeeze_talk"});
hong({body:"0_squeeze"});
```

b: มนุษย์! ฟังนะ เรากำลังอยู่ในอันตราย คนเล่นน่ะ...

[...จะทรมานพวกเราอีกรอบ!](#act1_replay_torture)

[...จะหาตอนจบอีกแบบไม่เจอ!](#act1_replay_alternate)

[...จะรู้สึกว่าเนื้อเรี่องกับการเล่นมันไม่เข้ากัน!](#act1_replay_dissonance)

# act1_replay_torture

```
window.HACK_REPLAY = JSON.parse(localStorage.act4);
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

{{if window.HACK_REPLAY.act1_ending=="fight"}}
b: เขาจะทำให้เราม้วนเป็นลูกบอลแล้วร้องไห้!
{{/if}}

{{if window.HACK_REPLAY.act1_ending=="flight"}}
b: เขาจะทำให้เราทุ่มมือถือเพราะมันทำให้เราแพนิค!
{{/if}}

{{if window.HACK_REPLAY.a2_ending=="fight"}}
b: เขาจะ *ไม่ยอม* ให้เราชกคนจัดปาร์ตี้!
{{/if}}

{{if window.HACK_REPLAY.a2_ending=="flight"}}
b: เขาจะบังคับให้เราชกคนจัดปาร์ตี้ที่ร้ายแต่ก็น่าเห็นใจ!
{{/if}}

{{if window.HACK_REPLAY.a3_ending=="jump"}}
h: อย่างน้อยรอบนี้อาจไม่ต้องโดดหลัง--
{{/if}}

{{if window.HACK_REPLAY.a3_ending=="walkaway"}}
b: เขาจะให้เราโดดหลังคา!!!
{{/if}}

`bb({body:"fear"});`

b: เรี่องใหม่ๆ แย่ๆ หลายๆอย่างจะเกิดกับพวกเรา แล้วเราก็จะ--

(#act1_replay_end)


#act1_replay_alternate

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

h: จริงอยู่ที่เนื้อเรี่อง *ทั้งหมด* อาจเหมือนเดิม แต่ทุกตอนมีตอนจบสองแบบ แล้วก็มีแตกกิ่งบทพู--

`bb({body:"fear"});`

b: คนเล่นจะเซ็ง ปิดแท็บ ลบเกม แล้วพวกเราก็จะ--

(#act1_replay_end)


# act1_replay_dissonance

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

h: อ-อะไรเข้าอะไรนะ

`bb({eyes:"normal"});`

b: เรี่องนี้เป็นเรี่องเกี่ยวกับการ *เลือก* ที่จะสร้างปฏิสัมพันธ์ที่ดีกับความกลัวไม่ใช่เหรอ

`bb({eyes:"normal_right"});`

b: แล้วไอ้การมาเล่นใหม่นี่มันก็ได้เรี่องแบบเดิม มันส่อว่า *เลือก* อะไรมันก็ไม่ต่างกัน

`bb({eyes:"narrow_eyebrow"});`

b: ทำให้เห็นว่าข้อคิดของเกมกับการเล่นมันไม่เหมือนกัน

`bb({eyes:"fear"});`

b: แล้วมันจะทำให้โลกของเรี่องนี้พัง

`bb({body:"fear"});`

b: แล้วพวกเราก็จะ--

(#act1_replay_end)


# act1_replay_end

`bb({body:"panic"})`

b: ตายยยยยยยยยยยยยยยยยย

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.clearText();
```

(...1001)

```
bb({body:"laugh"});
hong({body:"laugh"});
Game.clearText();
sfx("laugh");
```

(...5001)

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({body:"0_sammich"});
```

h: โอเค เลิกเล่นแล้วเข้าบทเถอะ

```
Game.clearText();
```

n4: (ให้ความวิตก _ของคุณ_ บลา บลา บลา เลือกสิ่งที่เหมือนกับความกลัว _ของคุณ_ บลา บลา เคยเล่นแล้วไม่พูดซ้ำนะ)

```
sfx("squeak");
hong({body:"0_squeeze"});
bb({body:"squeeze"});
```

(#act1_normal_choice)



# act1_normal

`hong({mouth:"0_neutral", eyes:"0_annoyed"})`

h: โอ้ เยี่ยมม หมาป่า^กู^กลับมาอีกละ สสสสสสสสสุดยอด

`hong({eyes:"0_neutral"})`

n: หน้าที่ของคุณคือปกป้องมนุษย์ของคุณจาก *อันตราย*

`bb({eyes:"look", mouth:"small_lock"})`

n: เอาเข้าจริงๆแล้ว แซนด์วิชชิ้นนั้นเป็น *อันตราย* ต่อเขา

n: เร็วเข้า เตือนเขาสิ!

```
sfx("squeak");
bb({body:"squeeze_talk"});
hong({body:"0_squeeze"});
```

b: มนุษย์! ฟังนะ เรากำลังอยู่ในอันตราย! อันตรายนั้นคือ...

`bb({body:"squeeze"})`

n4: (ให้ความวิตก _ของคุณ_ ออกมาเล่น! เลือกสิ่งที่เหมือนกับความกลัว _ของคุณ_ ที่สุด)

(#act1_normal_choice)

# act1_normal_choice

[พวกเรากำลังกินข้าวเที่ยงคนเดียว! อีกแล้ว!](#act1a_alone) `bb({body:"squeeze_talk"})`

[พวกเราไม่ทำงานระหว่างกินข้าว!](#act1a_productive) `bb({body:"squeeze_talk"})`

[ขนมปังขาวมันสุขภาพเสีย!](#act1a_bread) `bb({body:"squeeze_talk"})`

# act1a_alone

```
bb({body:"normal", mouth:"small", eyes:"narrow"});
hong({body:"0_sammich"});
```

b: ไม่รู้หรือไงว่าความเหงามันทำให้เราตายได้ ไม่ต่างจากสูบบุหรี่วันละ 15 มวน?-

`Game.OVERRIDE_TEXT_SPEED = 2;`

`bb({mouth:"normal", eyes:"normal_right"})`

b: (Holt-Lunstad 2010, PLoS Medicine)

`hong({eyes:"0_annoyed"})`

h: เอ่อ ขอบใจที่อ้างอิงที่มานะ แต่--

`Game.OVERRIDE_TEXT_SPEED = 2;`

`bb({body:"fear", mouth:"normal", eyes:"fear"})`

b: หมายความว่าถ้าเราไม่คุยกับใคร *เดี๋ยวนี้* พวกเราก็จะ-

`bb({body:"panic"})`

b: ตายยยยยยยยยยยยยยยยยย

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "alone");
publish("hp_show");
```

(...2500)

`_.fifteencigs = true`

n: คุณได้ใช้ *ความกลัวคนไม่รัก*

(#act1b)

# act1a_productive

```
bb({body:"normal", mouth:"small", eyes:"normal"});
hong({body:"0_sammich"});
```

b: เอาคอมออกมาทำงานเดี๋ยวนี้!

`hong({eyes:"0_annoyed"})`

h: เอ่อ อย่าเลย เดี๋ยวเศษขนมปังติดคีย์บอ--

```
bb({mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: ถ้าเราไม่ทำอะไรให้สังคมพวกเราก็ไม่ต่างจากปรสิตสังคม!!

b: ร่างกายสังคมก็จะไปหาหมอสังคม ไปหายามาฆ่าปรสิตสังคม แล้วพวกเราก็จะ--

```
bb({body:"panic", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: ตายยยยยยยยยยยยยยยยยย

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "bad");
publish("hp_show");
```

(...2500)

`_.parasite = true`

n: คุณได้ใช้ *ความกลัวเป็นคนไม่ดี*

(#act1b)

# act1a_bread

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich", eyes:"0_annoyed"});
```

h: การศึกษามีการทำซ้ำเปล--

```
bb({body:"fear", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: แป้งฟอกสีจะทำน้ำตาลในเลือดเราสูงปรี้ดจนเราต้องถูกตัดแขนขา แล้วเราก็จะ--

`bb({body:"panic"})`

b: ตายยยยยยยยยยยยยยยยยย

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "harm");
publish("hp_show");
```

(...2500)

`_.whitebread = true`

n: คุณได้ใช้ *ความกลัวถูกทำร้าย*

(#act1b)

# act1b

n: ได้ผลดีจัด

`bb({mouth:"smile", eyes:"smile"});`

b: เห็นไหมมนุษย์ ฉันคือหมาป่าเฝ้าบ้านผู้ซื่อตรง

`bb({body:"pride_talk"});`

b: เชื่อสัญชาติญาณสิ! ความรู้สึกของนายถูกต้องเสมอ!

`bb({body:"pride"});`

n: ลดพลังของมนุษย์คุณ ให้เหลือศูนย์

n: เพี่อปกป้องความต้องการทาง ร่างกาย + สังคม + ศีลธรรม คุณสามารถใช้:

n: ความกลัว *ถูกทำร้าย* #harm#

n: ความกลัว *คนไม่รัก* #alone#

n: ความกลัว *เป็นคนไม่ดี* #bad#

`Game.OVERRIDE_TEXT_SPEED = 1.25;`

n4: (ข้อแนะนำ: เลือกตัวเลือกที่แทงใจดำคุณ จี้ใจดำแบบลึกสุดๆไปเลย!~)

h: ...

```
hong({body:"putaway"});
sfx("rustle");
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

(...1000)

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

h: เออ น่าจะได้เวลาเช็คมือถือละมั้ง

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: ปกป้องมนุษย์ของคุณ

n: จากโลกอันโหดร้าย จากคนอื่นๆ จากตัวเขาเอง

n: ขอให้โชคดี

(...500)

`Game.clearText()`

(...500)

(#act1c)

# act1c

`music('battle', {volume:0.5})`

n: รอบที่หนึ่ง: *สู้!*

`bb({body:"normal", mouth:"normal", eyes:"normal"});`

h: หึม ในเฟสบุ็คบอกว่าเสาร์อาทิตย์นี้มีปาร์ตี้

`bb({eyes:"uncertain"});`

b: ไม่ใช่ว่าไอ้นั้นมันจัดปาร์ตี้ *ทุก* เสาร์อาทิตย์เหรอ?

`bb({eyes:"uncertain_right"});`

b: เขากำลังพยายามกลบความว่างเปล่าอะไรข้างใน? แบบนี้ไม่ปกติแล้ว!

`hong({eyes:"surprise"});`

h: เอ็ะ เขาเชิญเราด้วย

`bb({eyes:"fear", mouth:"normal"});`

b: เอาสิ!

[ตอบไป ไม่งั้นเหงาตาย!](#act1c_loner)

[ตอบไม่ไป ปาร์ตี้มีวางยาแน่!](#act1c_drugs)

[ไม่ตอบ เราไปแล้วเดี๋ยวปาร์ตี้เขาเสีย](#act1c_sad)

# act1c_loner

{{if _.fifteencigs}}
b: บุหรี่สิบห้ามวนนะมนุษย์! สิบห้ามวน!
{{/if}}

{{if !_.fifteencigs}}
`Game.OVERRIDE_TEXT_SPEED = 1.5;`
{{/if}}

{{if !_.fifteencigs}}
b: แล้วงานศพเราก็จะไม่มีใครมา เถ้าเราก็จะถูกเอาไปโปรยลงทะเล เราจะถูกปลาวาฬกิน
{{/if}}

{{if !_.fifteencigs}}
b: แล้วเราจะกลายเป็นขี้ปลาวาฬ!
{{/if}}

{{if !_.fifteencigs}} `_.whalepoop = true` {{/if}}

(...500)

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`bb({eyes:"normal"});`

{{if !_.fifteencigs}}
b: ถึงต้องไปปาร์ตี้ไง!
{{/if}}

{{if _.parasite}}
b: เอาคอมไปด้วยแล้วกัน จะได้ทำงานแล้วไม่เป็นปรสิตสังคม
{{/if}}

{{if _.whitebread}}
b: ถ้าเขาไม่เซิร์ฟขนมปังขาวนะ
{{/if}}

`hong({mouth:"anger", eyes:"anger"});`

h: เออ ไปก็ได้ถ้าไปแล้วแกจะหุบปาก

h: บอกเขาว่าไปแล้วกัน

{{if _.whalepoop}}
b: ขี้ปลาวาฬนะมนุษย์! ขี้ปลาวาฬ!
{{/if}}

`_.partyinvite="yes"`

(#act1d)

# act1c_drugs

`bb({mouth:"small", eyes:"fear"});`

{{if _.whitebread}}
b: หรือว่าแย่กว่านั้น... ขนมปังขาว
{{/if}}

{{if _.whitebread}}
`Game.OVERRIDE_TEXT_SPEED = 1.5;`
{{/if}}

{{if _.whitebread}}
b: พวกเราจะเล่นยากับขนมปังเกินขนาดจนสัปเหร่อจะยัดศพอ้วนๆของเราลงเมรุไม่ได้!
{{/if}}

{{if !_.whitebread}}
b: พวกเราจะเสพโน่นเสพนี่จนสัปเหร่อจะงงว่าทำไมศพเราถึงกันบูดไว้แล้ว!
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

{{if _.parasite}}
b: อีกอย่างนะ เราไม่มีเวลาปาร์ตี้ เราต้องทำงานไม่งั้นเราก็เป็นแค่ปรสิตสังคมเลวๆ!
{{/if}}

`hong({mouth:"anger", eyes:"anger"});`

h: เออ ไม่ไปก็ได้ถ้าไม่ไปแล้วแกจะหุบปาก

h: บอกเขาว่าไม่ไปแล้วกัน

`_.partyinvite="no"`

(#act1d)

# act1c_sad

`bb({eyes:"uncertain_right", mouth:"normal"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

{{if _.fifteencigs}}
b: วันๆ เราไม่ทำอะไร เอาแต่นั่งบ่นว่าความเหงามันแย่พอๆกับการสูบบุหรี่วันละ 15 มวน
{{/if}}

{{if _.parasite}}
b: ไปปาร์ตี้ก็มีแต่จะคิดมากว่าควรจะทำงานแทนที่จะมาเหล้ายาปลาปิ้งแบบนี้
{{/if}}

{{if _.whitebread}}
b: วันๆ เราไม่ทำอะไร เอาแต่กังวลว่าอาหารที่เรากินเข้าไปจะทำเราตายมั้ย
{{/if}}

```
bb({mouth:"normal", eyes:"normal"});
hong({mouth:"neutral", eyes:"lookaway"});
```

h: ก็เพราะใครล่ะ

`hong({eyes:"neutral"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

b: ถ้าเราไปงานเขาก็กร่อย แต่ถ้าเราปฏิเสธเข้าก็เซ็งเหมือนกัน

`bb({body:"fear", eyes:"fear"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

b: เราไม่ทำอะไรนอกจากทำคนอื่นรู้สึกแย่ๆ เราควรรู้สึกแย่ด้วย!!!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

`hong({mouth:"anger", eyes:"anger"});`

h: เออ ไม่ตอบก็ได้ถ้าไม่ตอบแล้วแกจะหุบปาก

h: ไม่ตอบแล้วกัน

`_.partyinvite="ignore"`

(#act1d)

# act1d

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"neutral", eyes:"annoyed"});
```

h: อ่านเฟสแล้วเครียด ไปทำอย่างอื่นที่สงบกว่านี เครียดน้อยกว่านี้ดีกว่า

`hong({eyes:"neutral"});`

h: ทวิตมีอะไรบ้างตอนนี้?

`bb({eyes:"look"});`

[แย่ละ ดูข่าวไม่ดีนั่นสิ!](#act1d_news)

[แย่ละ มีคนทวิต *เรา* ลับหลังเปล่า?](#act1d_subtweet)

[ดูนั่นสิ รูปแมวกินนม](#act1d_milk)


# act1d_news

```
bb({eyes:"pained1"});
music(null, {fade:2});
```

b: รู้สึกว่าทั้งโลกลุกเป็นไฟใช่ไหมล่ะ

```
bb({eyes:"pained2"});
hong({mouth:"sad", eyes:"sad"});
```

b: รู้สึกว่าทุกอย่างกำลังสิ้นสลาย ทุกคนกำลังตาย พวกเรากำลังตาย แล้วเราทำอะไรไม่ได้ใช่ป่าว

```
Game.OVERRIDE_TEXT_SPEED = 0.5;
bb({mouth:"shut"});
```

b: ...

`bb({mouth:"smile", eyes:"smile"});`

b: รีเลยรออะไร

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

`_.badnews=true`

```
music('battle', {volume:0.5});
hong({mouth:"anger", eyes:"anger"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: โอเค รีแล้ว รีแล้ว เลิกบ่นได้ยัง

`hong({mouth:"neutral", eyes:"annoyed"});`

h: ช่าง^แม่ง^ ไปดู Snapchat ดีกว่า

(#act1e)


# act1d_subtweet

`bb({eyes:"fear"});`

b: แซะกันเห็นๆ แอบเอาเราไปแซะกันชัวร์!

`hong({eyes:"annoyed"});`

h: ไม่น่าใช่มั้ง?

`bb({eyes:"narrow", mouth:"small"});`

b: แล้วถ้าเขาแอบนินทาเราลับหลังกันทุกคนล่ะ

h: เขาคงไม่--

`bb({body:"fear", eyes:"fear", mouth:"normal"});`

b: ลับหน้าเราล่ะ!!

`hong({eyes:"sad", mouth:"sad"});`

h: ไม่--

`bb({eyes:"narrow", mouth:"small"});`

b: แล้ว *ถ้าใช่* ล่ะ

h: อ--

`bb({eyes:"narrow_eyebrow"});`

b: *ถ้าใช่ล่ะ*

```
Game.OVERRIDE_TEXT_SPEED = 0.5;
hong({mouth:"shut"});
```

h: ...

(...1000)

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`_.subtweet=true`

```
hong({mouth:"anger", eyes:"annoyed"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: โอเค Snapchat เถอะ

(#act1e)

# act1d_milk

`hong({mouth:"smile", eyes:"neutral"});`

h: เออ น่ารักดี รีละ คิดว่า--

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: แมวย่อยนมไม่ได้โว้ย พวกเราชอบการทรมานสัตว์!! พวกเรามันถ่อย!!

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
attack("18p", "bad");
```

(...2500)


`_.catmilk=true`

```
hong({mouth:"anger", eyes:"annoyed"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: โอเค Snapchat เถอะ

(#act1e)

# act1e

`hong({mouth:"neutral", eyes:"neutral"});`

h: รูปจากปาร์ตี้คืนที่แล้วล่ะ ปาร์ตี้วันหยุดมันเป็น *แบบนี้* นี่้เอง

{{if _.partyinvite=="yes"}} (#act1e_said_yes) {{/if}}

{{if _.partyinvite=="no"}} (#act1e_said_no) {{/if}}

{{if _.partyinvite=="ignore"}} (#act1e_said_ignore) {{/if}}

# act1e_said_yes

`hong({mouth:"sad", eyes:"annoyed"});`

h: อูย เหมือนคนจะแน่นไปหน่อย

h: บอกเขาว่าไปดีแล้วใช่มั้ย?

```
hong({mouth:"neutral", eyes:"neutral"});
bb({mouth:"normal", eyes:"normal"});
```

[เปลี่ยนคำตอบ? แบบไอ้งั่งเหรอ?!](#act1e_yes_dontchange)

[เปลี่ยนคำตอบ! คนแน่นเกิน!](#act1e_yes_changetono)

{{if _.subtweet}}
[เออเขาแซะเราจริงด้วย](#act1e_ignore_subtweet)
{{/if}}

{{if _.badnews}}
[เดี๋ยวนะ เรารีข่าวนั้นแบบไม่ได้เช็คความถูกต้อง](#act1e_ignore_factcheck)
{{/if}}

{{if (!_.subtweet && !_.badnews)}}
[ท่านั่งของนายมันแย่มาก รู้เปล่า](#act1e_ignore_posture)
{{/if}}

# act1e_yes_dontchange

```
bb({eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: เขาคาดหวังว่าเราจะมาแล้วเรามาหักหลังเขาอย่างนี้มันใช่เหรอ อยากตายคนเดียวหรือไง?!

{{if _.fifteencigs}}
b: สิบห้า! มวน!
{{/if}}

{{if _.whalepoop}}
b: ขี้ปลาวาฬ!
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

```
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: หนวกหูน่า ตอบไปเหมือนเดิมแหละ

(#act1f)

# act1e_yes_changetono

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: ไม่รู้เหรอว่าการแตกตื่นตอนคนเยอะๆ มันอันตราย

```
bb({body:"fear", mouth:"small", eyes:"narrow"});
hong({eyes:"sad", mouth:"sad"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: ในปี 2003 ผับที่นึงใน Rhode Island ไฟไหม้ ทุกคนแตกตื่นแล้วกรูไปติดตรงทางออกจนคนถูกไฟคลอกตายไป 100 คน-

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({mouth:"shock"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: อยากให้แบบนั้นเกิดกับเราหรือไง-

```
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 2.5;
```

b: อย่าไป อย่าไป อย่าไป อย่าไป อย่าไป อย่าไป อย่าไป อย่าไป อย่าไป อย่าไป-


```
bb({body:"normal", eyes:"fear", mouth:"normal"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

```
hong({eyes:"anger", mouth:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: ก็ได้ก็ได้ ไม่ไปก็ได้ ^ห่า^เอ้ย

(#act1f)

# act1e_said_no

`hong({mouth:"sad", eyes:"sad"});`

h: หึม ก็ดูสนุกดีนี่

h: บอกเขาว่าไม่ไปดีแล้วใช่ไหม?

`bb({mouth:"normal", eyes:"normal"});`

[เปลี่ยนคำตอบ? แบบไอ้งั่งเหรอ?!]](#act1e_no_dontchange)

[เปลี่ยนคำตอบ! เดี๋ยวไม่มีใครคบ!]](#act1e_no_changetoyes)

{{if _.subtweet}}
[เออเขาแซะเราจริงด้วย](#act1e_ignore_subtweet)
{{/if}}

{{if _.badnews}}
[เดี๋ยวนะ เรารีข่าวนั้นแบบไม่ได้เช็คว่าจริงไม่จริง](#act1e_ignore_factcheck)
{{/if}}

{{if (!_.subtweet && !_.badnews)}}
[ท่านั่งของนายมันแย่มาก รู้เปล่า](#act1e_ignore_posture)
{{/if}}

# act1e_no_dontchange

`bb({eyes:"anger"})`

b: ทุกคนคาดหวังไว้กับเรา!

b: ...คาดหวังว่าเราจะไม่ไปแล้วให้เขาสนุกกับปาร์ตี้ที่ไม่มีตัวกาลิกิณีน่ารังเกียจ{{if _.whitebread}}ที่ชอบกินขนมปังขาว{{/if}}แบบเร--


```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

```
bb({body:"normal", eyes:"uncertain", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: หุบปากน่า หุบปาก ไม่ไปเหมือนเดิมแหละ!

(#act1f)

# act1e_no_changetoyes

```
bb({body:"fear", eyes:"fear", mouth:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: อาการเหงาระยะยาวเพี่มคอร์ติซอลในตัวเรา แล้วยังทำให้เราเสี่ยงเป็นโรคหัวใจและสโตรค์ด้วย

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

{{if _.fifteencigs}}
b: สิบห้ามวน!!!
{{/if}}

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: หุบปากน่า หุบปาก ไปก็ได้! ^ห่า^เอ้ย!

(#act1f)

# act1e_ignore_subtweet

```
bb({eyes:"fear", mouth:"small"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: ทวิตเก่าๆ ที่ problematic มันกลับมาหลอกหลอนเราแล้ว!

```
bb({body:"fear", eyes:"fear", mouth:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.7;
```

b: เราจะถูก call out และ cancel แล้วเราก็จะถูกลากบนโลกอินเตอร์เน็ต ถูกประจานให้ทุกคนรับรู้!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: เป็น^เหี้ย^อะไรของ^มึง^?!

(#act1f)

# act1e_ignore_factcheck

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: เรากำลังปล่อยเฟคนิวส์! เรากำลังทลายความเชื่อมั่นในสื่อเสรี!

```
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: ที่ระบอบเผด็จการจะลุกขึ้นจากซากปรักหักพังของประชาธิปไตยได้ก็เพราะเรา!

```
bb({body:"normal", eyes:"anger"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

```
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
_.factcheck = true;
```

h: เป็น^เหี้ย^อะไรของ^มึง^?!

(#act1f)

# act1e_ignore_posture

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: อยากมีหลังงอเป็นตะขอหรือไง?! เลิกก้มหน้าดูจอได้แล้ว!

```
bb({body:"meta"});
```

b: นั่นหมายถึงนายด้วยนะ

```
bb({body:"normal", mouth:"normal"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: เป็น^เหี้ย^อะไรของ^มึง^?!

(#act1f)

# act1e_said_ignore

`hong({mouth:"sad", eyes:"sad"});`

h: หึม ก็ดูสนุกดีนี่

h: หรือว่าไม่ควรเมินไม่ตอบแบบนั้น?

`bb({mouth:"normal", eyes:"normal"});`

[เมินต่อไป เราไปงานเขาก็ล่ม](#act1e_ignore_continue)

[จริงๆ แล้วบอกเขาว่าไปดีกว่า](#act1e_ignore_changetoyes)

[จริงๆ แล้วบอกเขาว่าไม่ไปดีกว่า](#act1e_ignore_changetono)

# act1e_ignore_continue

`hong({eyes:"annoyed"});`

h: เมินเขาต่อไปมันไม่ดูหยิ่งไปเหรอ

`bb({eyes:"normal_right"});`

b: คนอื่นยังเมิน *พวกเรา* ได้เลยนี่

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`bb({eyes:"normal"});`

b: ถือว่าเจ๊ากันละกัน

(#act1f)

# act1e_ignore_changetoyes

`hong({eyes:"surprise", mouth:"smile"});`

h: แกยอมให้ฉัน... สนุก?

b: อึม ก็ถ้าเหงาเกินก็ *ตาย* ได้ไง

`hong({eyes:"neutral", mouth:"neutral"});`

(#act1e_no_changetoyes)

# act1e_ignore_changetono

`bb({eyes:"narrow"});`

b: คนเยอะไปน่ะสิ แล้วคนเยอะมันอันตรายนะ

(#act1e_yes_changetono)


# act1f

```
hong({mouth:"neutral", eyes:"neutral"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: ช่างเถอะ ทินเดอร์เข้าล่ะ

`bb({eyes:"uncertain"})`

b: หะ ไอ้แอพนัดเอากันอ่ะนะ

`hong({eyes:"annoyed"})`

h: ไม่ใช่แอพนัด^เย็ด^โว้ย มันคือวิธีหาคนใหม่ๆ--

`bb({eyes:"narrow"})`

b: แบบนั้นแหละที่เรียกว่าแอพนัดเอากัน

```
hong({eyes:"surprise", mouth:"smile"});
bb({eyes:"normal"});
```

h: โห ได้คู่ละ! หน้าตาดีซะด้วยสิ!

```
bb({eyes:"narrow_eyebrow"});
hong({eyes:"sad", mouth:"anger"})
```

h: ขอร้องล่ะ อย่าทำพั--

```
bb({body:"panic"});
Game.OVERRIDE_TEXT_SPEED = 2.0;
```

b: อันตราย! อันตราย! อันตราย! อันตราย! อันตราย! อันตราย!

`bb({body:"fear", eyes:"fear", mouth:"normal"})`

[เรากำลังถูกคนอื่น *หลอกใช้*](#act1f_used_by_others)

[เรากำลัง *หลอกใช้* คนอื่น](#act1f_using_others)

[นายเพี่งจับคู่กับฆาตกรต่อเนี่อง!!!](#act1f_killer)

# act1f_used_by_others

`bb({body:"point_crotch", eyes:"normal", mouth:"normal"})`

b: นัดเจอคนอื่นมันอาจช่วยเติมเต็มความว่างเปล่าระหว่างขาได้

b: แต่ว่ามันไม่อาจเติมเต็มความว่างเปล่า...

`bb({body:"point_heart", eyes:"pretty", mouth:"small"})`

b: *ในนี้* ได้

(...1000)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: ประเด็นหลักคือพวกเราจะตายแบบไม่มีใครคบ!!!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`_.hookuphole=true`

(#act1g)

# act1f_using_others

`bb({eyes:"narrow", mouth:"small"})`

b: คิดว่าอวัยวะคนอื่นเป็นโปเกม่อนให้เราสะสมหรือไง?

```
bb({body:"sing", eyes:"pretty", mouth:"shut"});
music("pokemon");
Game.clearText();
Game.FORCE_CANT_SKIP = true;
```

```
Game.FORCE_TEXT_DURATION = 1000;
Game.FORCE_NO_VOICE = true;
```

b: ♫ (เพลงเปิดโปเกม่อน)-

(...5600)

```
bb({mouth:"normal"});
Game.FORCE_TEXT_DURATION = 2400;
```

b: ♫ ฉันจะเป็นคน ที่^เงี่ยน^ที่สุด-

(...500)

```
bb({eyes:"narrow", mouth:"small"});
Game.FORCE_TEXT_DURATION = 2100;
```

b: ♫ ที่โลกไม่เคยได้เห็น-

(...1500)

```
bb({eyes:"pretty"});
Game.FORCE_TEXT_DURATION = 2300;
```

b: ♫ จับก้นดูนม แถมดูต้นขา-

(...500)

```
bb({eyes:"fear", mouth:"normal"});
Game.FORCE_TEXT_DURATION = 2000;
```

b: ♫ และเที่ยวเลียปิกา^จู๋^-

(...1000)

```
bb({eyes:"smile", mouth:"smile"});
Game.FORCE_TEXT_DURATION = 1000;
```

b: ♫ โปเก^โม็ค^! เราจะจั--

```
Game.FORCE_CANT_SKIP = false;
Game.clearText();
music(false);
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: ประเด็นคือพวกเราเป็นไอ้หื่นที่ชอบเอาเปรียบคนอื่น

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

`_.pokemon=true`

(#act1g)

# act1f_killer

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

{{if _.whitebread}}
b: เขาจะจับนายขังในบ่อน้ำแล้วบังคับให้นายกินขนมปังขาวจนอ้วน จะได้ฆ่านายไปทำเสื้อหนังคนไงล่ะ!
{{/if}}

{{if _.parasite}}
b: เขาจะเอานาฬิกาจับเวลาตีหัวเราแล้วบอกว่า "ไปตายซะไอ้ปรสิตสังคมไร้ประโยชน์!"
{{/if}}

{{if !_.whitebread && !_.parasite}}
b: เขาจะฉีกเนื้อนายเป็นชิ้นๆ เอาไส้นายไปทำริบบิ้น แล้วเอาเลือดนายไปผสมพั้นช์
{{/if}}

{{if !_.whitebread && !_.parasite}}
b: ปาร์ตี้แบบนี้เป็นยังไงล่ะ!
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

`_.serialkiller=true`

(#act1g)

# act1g

```
bb({body:"normal", mouth:"normal", eyes:"look"});
hong({body:"2_tired"});
Game.OVERRIDE_TEXT_SPEED = 0.5;
music(false);
```

h: ...

(...500)

h: ^กู^เบี่อเกมนี้^ฉิบหาย^ว่ะ

(...700)

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

h:
{{if _.fifteencigs}}"ความเหงาทำเราตายได้"... {{/if}}
{{if _.parasite}}"เราเป็นปรสิตสังคม"... {{/if}}
{{if _.whitebread}}"อย่ากินอันนั้น เดี๋ยวเราตาย"... {{/if}}
{{if _.subtweet}}"ทุกคนกำลังนินทาเราลับหลัง"... {{/if}}
{{if _.badnews}}"ทั้งโลกลุกเป็นไฟ"... {{/if}}
{{if _.hookuphole}}"เราจะตายคนเดียว"... {{/if}}
{{if _.serialkiller}}"เขาเป็นฆาตกรต่อเนี่อง"... {{/if}}
{{if _.catmilk}}"แมวย่อยนมไม่ได้"... {{/if}}
{{if _.pokemon}}เพลงล้อเลียน^กาก^ๆ... {{/if}}

h: ก็แค่อยากใช้ชีวิตแบบปกติอ่ะ

h: ก็แค่อยากปลดแอกจาก...การรู้สึกปวดใจแบบนี้

`bb({eyes:"look_sad"});`

b: นี่... มนุษย์...

`Game.OVERRIDE_TEXT_SPEED = 0.5;`

b: ทุกอย่างจะโอเค

(...600)

`bb({body:"point_heart", eyes:"look_sad_smile", mouth:"smile"});`

b: ในฐานะหมาป่าเฝ้าบ้าน ฉันจะคอยระวังอันตรายให้ แล้วก็จะทำทุกอย่างเพี่อให้นายปลอดภัย

`bb({body:"normal", eyes:"look_sad", mouth:"smile"});`

b: ฉันสัญญา

(...600)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({body:"phone1", eyes:"neutral", mouth:"neutral"});
```

h: แอพสุดท้ายละ อินสตา มีอะไรบ้างล่ะ?

`hong({eyes:"sad"});`

h: มี... รูปปาร์ตี้อีกหลายรูป

`hong({mouth:"sad"});`

h: ทุกคนดูมีความสุขดีจัง ไม่กังวล ไม่วิตก

`hong({mouth:"anger"});`

h: ทำไมถึงเป็นอย่างเขาไม่ได้ ทำไมเราถึงไม่ *ปกติ?*

`bb({eyes:"normal_right"});`

b: เอ่อ พูดถึงปาร์ตี้แล้ว เรี่องที่เขาเชิญเราน่ะ ตกลงว่า:

`bb({eyes:"normal"});`

[เราควรไป](#act1g_go) `Game.OVERRIDE_CHOICE_LINE=true`

[เราไม่ควรไป](#act1g_dont) `Game.OVERRIDE_CHOICE_LINE=true`

# act1g_go

`_.act1g = "go"`

(#act1h)

# act1g_dont

`_.act1g = "dont"`

(#act1h)

# act1h

b: เราควร--

```
bb({eyes:"wat", mouth:"small"});
hong({body:"2_fuck"});
```

h: ช่าง

`hong({body:"2_you"});`

h: ^พ่อง^

(...500)

b: ห

(...1500)

`bb({eyes:"wat_2"});`

b: หะ

`hong({body:"phone1", eyes:"anger", mouth:"anger"});`

h: ชั้นจะบอกเขาว่าไป

{{if _.act1g=="go"}}
h: ไม่ใช่เพราะแกอยากให้ไป *ชั้น* อยากไปเอง
{{/if}}

{{if _.act1g=="dont"}}
h: เพราะว่าแกไม่อยากให้ไปไงล่ะ
{{/if}}

```
hong({body:"putaway"});
sfx("rustle");
```

h: แกไม่มีสิทธ์มาบังคับชั้น

```
sfx("rustle2");
hong({body:"0_sammich", eyes:"0_annoyed", mouth:"0_neutral"});
```

h: ถ้าไม่มีอะไรแล้ว ก็ขอตัวนั่ง^แดก^แซนด์วิชอร่อยๆนี้เงียบๆคนเดียวแล้วกัน

`hong({body:"2_sammich_eat"});`

(...601)

```
sfx("sandwich");
hong({body:"2_sammich_eaten", eyes:"0_lookaway", mouth:"0_chew1"})
```

(...601)

```
bb({body:"normal", eyes:"uncertain", mouth:"shut"});
Game.OVERRIDE_TEXT_SPEED = 0.5;
```

b: ...

```
bb({eyes:"normal_right"});
Game.OVERRIDE_TEXT_SPEED = 1;
```

b: ...

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 4;
```

b: ..................

(...500)

`bb({mouth:"normal"});`

[ว้าาาาาาก พวกเราจะตายกันหมด!!!](#act1h_death) `Game.OVERRIDE_CHOICE_LINE = true;`

[ว้าาาาาาก ทุกคนเกลียดเรา!!!](#act1h_loneliness) `Game.OVERRIDE_CHOICE_LINE = true;`

[ว้าาาาาาก พวกเรามันเลว!!!](#act1h_worthless) `Game.OVERRIDE_CHOICE_LINE = true;`

# act1h_death

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: ว้าาาาาาก พวกเราจะตายกันหมด ว้าาาาาาากกกกกกก!!!

```
hong({body:"3_defeated1"});
attack("100p", "harm");
```

(...2500)

(#act1i)

# act1h_loneliness

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: ว้าาาาาาก ทุกคนเกลียดเรา ว้าาาาาาากกกกกกก!!!

```
hong({body:"3_defeated1"});
attack("100p", "alone");
```

(...2500)

(#act1i)

# act1h_worthless

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: ว้าาาาาาก พวกเรามันเลว ว้าาาาาาากกกกกกก!!!

```
hong({body:"3_defeated1"});
attack("100p", "bad");
```

(...2500)

(#act1i)

# act1i

```
bb({mouth:"smile_lock", eyes:"smile", body:"normal"});
music('battle', {volume:0.5});
```

n: ยินดีด้วย

(...500)

n: คุณปกป้องความต้องการทาง ร่างกาย + สังคม + ศีลธรรม ของมนุษย์คุณได้สำเร็จ

n: ดูสิ เขาซาบซึ้งสุดๆ ไปเลย!

(...500)

n: ตอนนี้พลังงานของเขาเหลือศูนย์แล้ว คุณจึงสามารถควบคุมการกระทำของเขาโดยตรงได้

`bb({mouth:"smile", eyes:"normal"});`

n: เลือกท่าไม้ตาย

`bb({mouth:"small_lock", eyes:"fear"});`

n: *จัดการเขาซะ*

[{สู้: ลงทัณฑ์มือถือนั่นซะ! โทษฐานทำเราเครียด!}](#act1i_phone) `Game.OVERRIDE_CHOICE_LINE=true`

[{หนี: ม้วนตัวเป็นลูกบอลแล้วร้องไห้!}](#act1i_cry) `Game.OVERRIDE_CHOICE_LINE=true`

# act1i_phone

`bb({mouth:"normal", eyes:"narrow"})`

b: มือถือนายมันทำให้นายแพนิกแล้ว!

`bb({eyes:"anger"})`

b: มาร์ค สากกระเบือ และผองเพี่อน กำลังปล้นจี้สุขภาพจิตของนายเพี่อเงินตราจากระบอบทุนนิยม!

```
bb({body:"fear", eyes:"fear"});
hong({body:"3_defeated2"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: ลงโทษมือถือนั่นซะ! ทำลายมันทิ้ง! ฆ่ามัน!

```
Game.OVERRIDE_TEXT_SPEED = 2.5;
bb({body:"flail"});
hong({body:"3_defeated3"});
_.act1_ending = "fight";
```

b: ฆ่ามัน! ฆ่ามัน! ฆ่ามัน! ฆ่ามัน! ฆ่ามัน! ฆ่ามัน! ฆ่ามัน! ฆ่ามัน! ฆ่ามัน! ฆ่ามัน! ฆ่ามัน! ฆ่ามัน! ฆ่ามัน! ฆ่ามัน! ฆ่ามัน! ฆ่าม--

(#act1j)

# act1i_cry

`bb({eyes:"fear", mouth:"normal"})`

b: โลกนี้เต็มไปด้วยอันตราย!

```
bb({body:"fear"});
hong({body:"3_defeated2"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: ทำแบบตัวอาร์มาดิลโลสิ! ม้วนตัวเองเพี่อป้องกันตัว!

```
Game.OVERRIDE_TEXT_SPEED = 2.5;
bb({body:"flail"});
hong({body:"3_defeated3"});
_.act1_ending = "flight";
```

b: ม้วนตัวแล้วร้องไห้! ม้วนตัวแล้วร้องไห้! ม้วนตัวแล้วร้องไห้! ม้วนตัวแล้วร้องไห้! ม้วนตัวแล้วร้องไห้! ม้วนตัวแล้วร้องไ-- 

(#act1j)

# act1j

`SceneSetup.act1_outro()`