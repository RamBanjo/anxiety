# act4

```
SceneSetup.act4();
publish("SAVE_GAME", ["act4"]);
Game.FORCE_CANT_SKIP = true;
```

(...5001)

```
publish("set_how_many_prompts", [1]);
Game.FORCE_CANT_SKIP = false;
Game.CLICK_TO_ADVANCE = true;
```

n3: (เกมออโต้เซฟแล้ว)

```
Game.clearText();
Game.FORCE_CANT_SKIP = true;
```

(...1001)

```
var hong_frame = _.INJURED ? 9 : 0;
publish("act4", ["hong_walks_in",hong_frame]);
sfx("grass_step1", {volume:0.1});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.2});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.25});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.3});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.35});
```

(...1667)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.35});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.35});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.35});
```

(...1333)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.20});
```

(...167)

```
publish("act4_hong_sits");
```

(...66)

```
publish("act4", ["hong_transition", "next"]);
sfx("squeak");
```

(...133)

`publish("act4", ["hong_transition", "next"]);`

(...1333)

```
publish("act4", ["hong_transition", "next"]);
sfx("rustle");
```

(...333)

`publish("act4", ["hong_transition", "next"]);`

(...1001)

```
publish("act4", ["hong_transition", "next"]);
```

(...333)

```
publish("act4", ["hong_transition", 9]);
sfx("sandwich");
```

(...333)

`publish("act4", ["hong_transition", 10]);`

(...333)

`publish("act4", ["hong_transition", 9]);`

(...333)

`publish("act4", ["hong_transition", 10]);`

(...333)

`publish("act4", ["hong_transition", 9]);`

(...333)

`publish("act4", ["hong_transition", 10]);`

(...333)

`publish("act4", ["hong_transition", "next"]);`

(...1466)

`publish("act4-out-1");`

(...201)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

```
publish("act4-show-chars");
Game.FORCE_CANT_SKIP = false;
```

(...901)

`hong({body:"sigh_1"})`

(...601)

```
hong({body:"sigh_2"});
bb({eyes:"look_down"});
```

h: *เฮ้อ*

```
hong({body:"hold", eyes:"normal", mouth:"normal"});
bb({eyes:"normal"});
```

h: ตกลงข้อคิดนิทานเรี่องนี้คือ^เชี่ย^อะไรเนี่ย?

`hong({body:"one_up", eyes:"annoyed"})`

h: เราได้ *เรียนรู้* อะไรบ้าง? ฉันทำตัวงี่เง่า "เพี่อน" ของชั้นหลอกใช้ชั้น แถมพวกเรายังเกือบ *ตาย* ด้วย

`hong({body:"normal", eyes:"normal"})`

{{if _.INJURED}}
[ช่าย แล้วนี่ยังไม่พูดถึงค่าหมอนะ](#act4a_bill)
{{/if}}

{{if !_.INJURED}}
[ช่าย แล้วนี่ยังไม่พูดถึงตับวายนะ](#act4a_liver)
{{/if}}

[ช่าย นั่นมันเป็นเคสที่แย่ที่สุด](#act4a_worst)

[ช่าย ฉันพูดถูกแล้ว](#act4a_right)

# act4a_bill

`hong({eyes:"annoyed_l", mouth:"narrow"});`

h: นั่นสินะ ชั่นว่า "การทำตัวงี่เง่า" ประกันไม่จ่ายนะ

`hong({eyes:"annoyed", mouth:"normal"});`

b: ถึงยังไงแล้ว...เราก็ยังรอดมาได้!

`hong({eyes:"normal"});`

h: ?

(#act4b)

# act4a_liver

`bb({eyes:"normal_d"});`

b: พวกเราน่าจะกินอายุขัยเราให้สั้นลงไปหลายปีล่ะ...

`bb({eyes:"surprise"});`

b: แต่อย่างน้อยพวกเราก็ *ยังมี* อายุขัย! พวกเรารอดมาได้!

```
hong({eyes:"surprise"});
bb({eyes:"normal"});
```

h: ?

(#act4b)

# act4a_worst

`bb({eyes:"normal_d"});`

b: ถึงยังไงแล้ว...

h: หึม?

`bb({eyes:"surprise"});`

b: เราก็ยังรอดมาได้!

(#act4b)

# act4a_right

`bb({eyes:"normal_d"});`

b: แต่... นายก็พูดถูกเหมือนกัน

`hong({eyes:"surprise"});`

h: หึม?

`bb({eyes:"normal"});`

b: ฉันเป็นหมาป่าเลี้ยงแกะ พอเกิดอันตรายขึ้น *จริงๆ* การที่นายไม่เชี่อฉันมันก็ไม่แปลก

`bb({eyes:"surprise_r"});`

b: ถึงอย่างนั้นเราก็ยังรอดมาได้!

(#act4b)

# act4b

```
bb({eyes:"normal", mouth:"normal"});
hong({eyes:"normal", mouth:"normal"});
```

b: ไม่ว่าจะเกิดอะไรขึ้นไปแล้ว พวกเราก็ยังอยู่ตรงนี้

`hong({eyes:"suspect"});`

{{if _.INJURED}}
h: แกดูเหมือนจะใจเย็นแปลกๆ ทั้งที่พวกเราได้เกือบตายกันแท้ๆ
{{/if}}

{{if !_.INJURED}}
h: แกดูเหมือนจะใจเย็นแปลกๆ ทั้งที่พวกเราได้ *เกือบ* เกือบตายกันแท้ๆ
{{/if}}

```
hong({eyes:"normal"});
bb({eyes:"annoyed_d", mouth:"narrow"});
```

b: เอ่อ ก็มันทำให้รู้สึกว่าพอเทียบกันแล้วทุกอย่างมันน่ากลัวน้อยลงน่ะ มันทำให้ฉันได้คิดด้วย

`bb({eyes:"normal", mouth:"normal"});`

b: ถ้าการที่ฉันมาสู้กับนายมันแย่ เพราะว่ามันไม่ได้ปกป้องนาย...

h: แต่การที่ชั้นสู้กับแกก็แย่ *เหมือนกัน* เพราะว่ามันทำให้แกตะโกนดังขึ้น...

`bb({eyes:"normal_r"})`

b: บางที...

`bb({eyes:"normal"})`

h: บางทีเราไม่ต้องสู้กันก็ได้

```
Game.FORCE_CANT_SKIP = true;
Game.clearText();
```

(...301)

`publish("smash",[0]);`

(...2001)

```
publish("smash",[1]);
sfx("smash_glass");
```

(...2601)

```
publish("smash",[2]);
bb({eyes:"normal", mouth:"normal"});
hong({eyes:"normal", mouth:"normal"});
```

(...2001)

`Game.FORCE_CANT_SKIP = false;`

(#act4b_2)

# act4b_2

```
music('dontfight',{fade:5, volume:0.6});
bb({eyes:"annoyed_d"});
```

b: ฉันไม่ใช่หมาป่าใจร้าย แต่ฉันก็ไม่ใช่หมาป่าเฝ้าบ้านด้วย

`bb({eyes:"sad_d"})`

b: ฉันเป็นหมารับเลี้ยงที่เคยถูกทำร้าย

`bb({eyes:"sad"})`

b: เราเคยผ่านอะไรร้ายๆ มา อาจเคยเป็นทรอม่า อาจเคยถูกทอดทิ้ง บางครั้งฉันก็โอเวอร์ไปหน่อยแล้วก็:

```
sfx("yaps", {volume:0.6});
bb({body:"yap_1"});
Game.FORCE_CANT_SKIP = true;
Game.WORDS_HEIGHT_BOTTOM = 215;
Game.FORCE_TEXT_DURATION = 90;
Game.FORCE_NO_VOICE = true;
```

b: โฮ่ง โฮ่ง โฮ่ง โฮ่ง โฮ่ง

(...1884)

```
Game.WORDS_HEIGHT_BOTTOM = -1;
Game.FORCE_CANT_SKIP = false;
bb({body:"normal", mouth:"scream", eyes:"scream_sad"});
```

b: แต่ฉันไม่อยาก *เป็น* หมาขี้ขลาด! ฉันอยากปกป้องนาย! ฉันอยากเป็นหมาที่ดี!

`bb({eyes:"sad", mouth:"normal"});`

b: มนุษย์... นายจะช่วยทำให้หมาป่าตัวนี้เชี่องมั้ย?

`hong({eyes:"sad"})`

h: ชั้น... ชั้นจะลองดูแล้วกัน

`hong({eyes:"normal_l", body:"chin", mouth:"narrow"})`

h: โอเค การสัมพันธ์ที่ดีกับอารมณ์ ความสัมพันธ์ที่ดีต้องสื่อสารกัน เรามาคุยกันเถอะ

`hong({eyes:"normal", body:"hands_1", mouth:"normal"})`

h: ห้านาทีต่อจากนี้จะฟังดูฝืนๆฝืดๆ แต่ว่าเรามาพยายามไปด้วยกันเถอะ

```
hong({body:"hands_2", mouth:"normal"});
```

h: ถึงหมาป่าในตัวชั้น... *แก* รู้สึกยังไงบ้าง

n2: ความกลัวที่ใช้ทั้งหมด:

n2: *ถูกทำร้าย* {{_.attack_harm_total}}, *คนไม่รัก* {{_.attack_alone_total}}, *เป็นคนไม่ดี* {{_.attack_bad_total}}

n2: คุณอยากพูดถึงความกลัวไหนก่อน? (คุณสามารถอ่านอันอื่นทีหลังได้)

```
_.a4_fears_discussed = 0;
_.num_thanks = 0;
hong({body:"normal"});
bb({eyes:"normal"});
```

[ฉันกลัวว่าเราจะถูกทำร้าย](#act4_harm)

[ฉันกลัวว่าพวกเราจะเดียวดาย](#act4_alone)

[ฉันกลัวว่าพวกเราเป็นคนไม่ดี](#act4_bad)

# act4_harm

```
_.a4_talked_about_harm = true;
_.a4_fears_discussed += 1;
```

`bb({eyes:"normal_d"})`

b: ฉันอยากปกป้องความปลอดภัยทางร่างกายของนาย

`bb({eyes:"sad_d"})`

b: แต่ *ทั้งโลก* นี้มันช่างอันตรายเหลือเกิน มันเต็มไปด้วยความโศกเศร้าและความชั่วร้าย

`bb({eyes:"sad"})`

{{if _.a4_fears_discussed==1}}
b: อึม ก็ไม่รู้ล่ะ *ฉัน* เป็นคนเลือกคำพูดมาสักพักนึงละ *นาย* ว่ายังไงบ้างมนุษย์?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: ไปที่นายอีกที นายคิดว่ายังไงบ้าง?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: คิดว่าไงมนุษย์?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[แกพูดถูก เรามาปกป้องตัวเองกันเถอะ](#act4_harm_skills)

[เรามาพยายาม *เข้าหา* อันตรายกันเถอะ](#act4_harm_exposure)

[ขอบใจนะ](#act4_thanks) `_.thanks_for = "ความปลอดภัยทางร่างกาย";`

# act4_harm_skills

`bb({eyes:"look_down", body:"paw"})`

b: แต่...ทำยังไงล่ะ? ฉันมีเขี้ยวเล็บก็จริง แต่ฉันเป็นแค่การอุปมานี่สิ

```
bb({ body:"normal", eyes:"normal" });
hong({ body:"one_up", eyes:"surprise" });
```

h: เราเรียนวิธีป้องกันตัวเองได้ หรือเข้าหาชุมชนที่ป้องกันซึ่งกันและกัน ปรับปรุงสุขภาพและขอบเขตความส่วนตัว?

```
bb({ eyes:"annoyed_r" });
hong({ body:"normal", eyes:"normal" });
```

b: ก็ได้นะ แต่ว่า...

[เราเรี่มจากไหนดีล่ะ?](#act4_harm_skills_start)

[แล้วถ้ามันยังไม่เวิร์คล่ะ?](#act4_harm_skills_work)

[แล้วถ้าเรา "ปลอดภัย" เกินไปล่ะ?](#act4_harm_skills_overboard)

# act4_harm_skills_start

`bb({ eyes:"sad_d" })`

b: มีอะไรให้ทำหลายอย่าง มีหลายเรี่องที่ต้องแก้ไข เราควร *เรี่ม* จากที่ไหนล่ะ?

`hong({ body:"shrug", eyes:"surprise" })`

h: ตอนนี้ก็ถือว่าเรี่มนะ

`bb({ eyes:"normal", mouth:"narrow" })`

b: เอ๋?

```
bb({ body:"normal", mouth:"normal" });
hong({ body:"normal", mouth:"normal", eyes:"normal"});
```

h: เรากำลังฝึกการสื่อสารที่ดีอยู่ มันจะช่วยให้เรามองเห็นอันตรายได้ดีขึ้น เห็นผลบวกลวงน้อยลง

`hong({ eyes:"surprise" });`

h: *นั่นแหละ* จะปกป้องเราจากอันตราย!

`hong({ eyes:"normal", mouth:"normal" });`

h: ดังนั้น: นี่ *เป็น* การฝึกป้องกันตัวเอง

`bb({ eyes:"normal_r" })`

b: เอ่อ ฉันคิดว่ามันจะเป็นแบบนี้ซะอีก:

```
Game.FORCE_CANT_SKIP = true;
Game.clearText();
hong({ eyes:"sad", mouth:"smile" });
bb({ body:"karate_1" });
sfx("hiya");
```

(...1001)

`Game.FORCE_CANT_SKIP = false;`

(#act4_something_else)

# act4_harm_skills_work

`bb({ eyes:"normal" });`

h: ก็จริงอยู่แหละ เราปกป้องตัวเอง 100% ไม่ได้...

`hong({ body:"one_up" });`

h: แต่อย่างน้อยการที่ดีขึ้น 1% ก็ยังดีกว่าไม่มีอะไรดีขึ้นเลยนะ

```
bb({ eyes:"annoyed" });
hong({ normal:"one_up" });
```

b: นายมองว่าแก้วไม่ได้ว่าง 99% แต่ว่ามีน้ำ 1% เหรอ?

`bb({ eyes:"normal" });`

h: มันก็ควรค่าแก่การมีถ้าติดอยู่ในทะเลทรายอ่ะนะ

`bb({ eyes:"closed" });`

b: อึม งั้นก็หมดแก้ว

(#act4_something_else)

# act4_harm_skills_overboard

`bb({ body:"chest", eyes:"annoyed" })`

b: คิดดูสิ ก็เพราะ *ฉัน* พยายามทำให้นายปลอดภัยมากเกินไปไม่ใช่เหรอนายถึงไม่ฟังคำเตือน!

`bb({ body:"normal", eyes:"normal" })`

h: ม่ายๆ แกพูดถูกแล้ว เราต้องปลอดภัยแบบพอดีๆ ทุกอย่างแบบพอดี

`bb({ eyes:"suspect" })`

b: โทษทีนะ *ทุกอย่าง* แบบพอดี?

`hong({ eyes:"annoyed" })`

h: *บางอย่างที่จำนวนพอดี* แบบพอดี

```
bb({ eyes:"closed" });
hong({ eyes:"normal" });
```

b: ขอบคุณที่ทำให้คำพูดนายตรงกับที่ตัวเองพูดแบบซ้อนไปซ้อนมานะ

(#act4_something_else)


# act4_harm_exposure

`bb({ mouth:"scream_talk", eyes:"scream", MOUTH_LOCK:true });`

b: *หะ*

```
bb({ mouth:"narrow", eyes:"suspect" });
hong({ body:"one_up" });
```

h: ลองสมมุติว่ามีหมาตัวนึงกลัวฟ้าผ่า

`hong({ body:"hands_1" });`

h: วิธีนึงที่คนฝึกหมาเขาทำกันคือ เปิดเสียงฟ้าผ่าแบบหรี่เสียงลง แล้วให้รางวัลหมาถ้ามันอยู่นิ่งๆ

`hong({ body:"hands_2" });`

h: หลายๆวันต่อจากนั้น คนฝึกก็ค่อยๆเพี่มเสียงให้ดังขึ้น จนหมาตัวนั้นไม่กลัวเสียงฟ้าผ่าอีกต่อไป

```
hong({ body:"normal", eyes:"surprise" });
bb({ mouth:"normal", eyes:"normal" });
```

h: อันนี้เรียกว่าการบำบัดด้วยการเข้าหาสิ่งที่กลัว (exposure therapy) ไงล่ะ!

`hong({ body:"point", eyes:"normal" });`

h: แล้วแกก็เป็นหมาด้วย มันควรจะได้ผลกับแกถูกมั้ย? สัตว์เลี้ยงลูกด้วยนมมีการตอบโต้แบบสู้หรือหนีทั้งนั้น

`hong({ body:"normal" });`

[แล้วถ้าเราชิน *เกินไป* ล่ะ?](#act4_harm_exposure_overboard)

[แล้วถ้าเราเจออันตราย *จริงๆ* ล่ะ?](#act4_harm_exposure_hurt)

[ฉันเป็นหมาป่านะ ไม่ใช่หมา](#act4_harm_exposure_dog) `bb({ eyes:"suspect" })`

# act4_harm_exposure_dog

h: แล้วชั้นจะแสดงความเมตตากับความอดทนกับแก จนแกเชี่องเป็นน้องหมาน่ารัก

`bb({ MOUTH_LOCK:true })`

b: ...

`bb({ eyes:"sad", mouth:"smile" })`

b: อั๊ยย่ะะะะ

(#act4_something_else)

# act4_harm_exposure_overboard

`bb({ eyes:"annoyed" })`

b: เพี่งเห็นกันไป *หมาดๆ* ว่าจะเกิดอะไรขึ้นถ้านายปิดกั้นความกลัวของนาย - นายเอาตัวเองไปอยู่ในสถานการณ์ที่อันตราย *จริง*ๆ

`bb({ eyes:"angry_r", body:"one_up" })`

b: อีกอย่างนะ การที่เราชิน *เกินไป* ไม่ทำให้เราเป็นพวกโรคจิตเหรอ?

`bb({ mouth:"scream", eyes:"scream", body:"two_up" })`

b: อีกหน่อยพวกเราคงได้ให้รางวัลตัวเองเวลาดูหนังโป๊ฆาตกรรมเลือดสาดแน่ๆ

`hong({ eyes:"annoyed" })`

h: ชั้นว่า... มันมีเส้นแบ่งระหว่างแบบนั้นกับฟ้าผ่านะ

`bb({ body:"normal", mouth:"normal", eyes:"suspect" })`

b: แล้วมันอยู่ *ตรงไหน* ละมนุษย์? *ที่ไหน*?!

`hong({ eyes:"surprise", body:"one_up" })`

h: ชั้นก็ไม่รู้ล่ะ แต่ *แก* ช่วยชั้นได้!

`hong({ eyes:"normal", body:"normal" })`

h: ทำงานกับแก ต่อรองกับแก เราจะมาขีดเส้นนั้นด้วยกัน

`bb({ body:"paw", mouth:"narrow", eyes:"closed" })`

b: โอเค แต่ฉันไม่มีมือเหมือนนาย นายต้องเป็นคนวาดนะ

(#act4_something_else)

# act4_harm_exposure_hurt

`bb({ body:"two_up", eyes:"angry_r" })`

{{if _.INJURED}}
b: ยกตัวอย่างนะ: เรากระโดดจาก *หลังคาตึก!*
{{/if}}

{{if !_.INJURED}}
b: ยกตัวอย่างนะ: เราเกือบกระโดดจาก *หลังคาตึก!*
{{/if}}

```
hong({ eyes:"annoyed" });
bb({ body:"normal", eyes:"annoyed" });
```

h: ม่าย แกพูดถูกแล้ว มัน *สามารถ* ทำเกินไปได้

`hong({ eyes:"normal" });`

h: นั่นแหละ ถ้าเราจะทำ exposure therapy เราจะเรี่มจากเล็กๆ ก่อน แล้วค่อยๆ ก้าวหาสิ่งที่เรากลัว

h: ก่อนที่จะเจออันตราย *จริงๆ* พวกเราก็หยุด

`bb({ eyes:"annoyed_r", mouth:"narrow" });`

b: เออ ฉันว่าฉันวาดเส้นระหว่างได้ยินเสียงฟ้าผ่ากับยืนตากฝนในพายุแล้วชูสายล่อฟ้าอ่ะนะ

(#act4_something_else)

# act4_thanks

`_.num_thanks += 1`

{{if _.num_thanks==1}}
(#act4_thanks_1)
{{/if}}

{{if _.num_thanks==2}}
(#act4_thanks_2)
{{/if}}

{{if _.num_thanks==3}}
(#act4_thanks_3)
{{/if}}

# act4_thanks_1

`bb({ MOUTH_LOCK:true })`

b: ...

`bb({ eyes:"annoyed" })`

b: เดี๋ยวนะ ไม่เห็นด้วยตกลงหรือไม่โต้แย้งเลยเหรอ? แค่..."ขอบใจ"?

`hong({ eyes:"surprise", body:"shrug" })`

h: ใช่! ขอบใจที่แกเป็นห่วงถึง{{_.thanks_for}}ของฉัน

```
bb({ eyes:"closed_annoyed", MOUTH_LOCK:true });
hong({ eyes:"normal", body:"normal" });
```

b: ...

h: แกโอเคมั้ย?

`bb({ eyes:"super_sad", mouth:"narrow" });`

b: นายไม่เคยพูด *ขอบคุณ* ฉันมาก่อนเลย

`hong({ mouth:"smile" });`

h: ง้ออว เจ้าหมาป่าขนฟูจอมวิตก

(#act4_something_else)

# act4_thanks_2

h: ถึงแกจะทำเกินไป แต่ชั้นก็ดีใจนะที่แกคอยระวัง{{_.thanks_for}}ของชั้น

`bb({ eyes:"annoyed" })`

b: เดี๋ยวนะ... นายไม่ได้พูด "ขอบใจ" ซ้ำๆเพี่อเลี่ยงการพูดถึงความกลัวพวกนี้ใช่มั้ย?

```
bb({ eyes:"normal" });
hong({ eyes:"annoyed", body:"chin" });
```

h: ก็ เรี่องมันซับซ้อน บางทีชั้นก็ไม่มีคำตอบทุกเรี่อง

`hong({ eyes:"annoyed_l", body:"one_up" })`

h: ชีวิตจริงมันไม่มีคำตอบตัวเลือก 3 ข้อหรอกนะ

`hong({ eyes:"normal", mouth:"smile", body:"normal" })`

h: แต่ตอนนี้ อย่างน้อยชั้นก็ขอบใจแกได้

b: ขอบใจเหมือนกันนะ ที่รับฟังฉันอย่างอดทน

`bb({ eyes:"closed" });`

b: เจ้าสัตว์เลี้ยงลูกด้วยนมไม่มีขนต้วน้อย

(#act4_something_else)

# act4_thanks_3

h: ถึงการโวยวายของแกทำชั้นกลัว  แกก็แค่พยายามปกป้อง{{_.thanks_for}}ของชั้น

`bb({ eyes:"smile_r" });`

b: โอเค ถ้านายมัวแต่ชมฉันแบบนี้ พวกบนเว็บคงจะคิดอะไรแปลกๆเกี่ยวกับเราแน่ๆ

```
bb({ eyes:"smile" });
hong({ eyes:"annoyed" });
```

h: เอาน่า ชั้นเป็นเด็กมหาลัยที่อ่อนไหว แกเป็นหมาป่าตัวใหญ่น่ากลัว อย่างแย่ที่สุดก็--

`hong({ eyes:"normal", body:"point" });`

h: เอ่อ จริงๆไม่ต้องรู้ก็ได้นะ

(#act4_something_else)




# act4_alone

```
_.a4_talked_about_alone = true;
_.a4_fears_discussed += 1;
```

`bb({ eyes:"sad_d" });`

b: ฉันต้องการช่วยให้นายเติมเต็มความต้องการทางสังคม แบบที่มนุษย์ทุกคนมี...

`bb({ eyes:"sad_u" });`

b: แต่ฉันก็กลัวว่าถ้ามีใครรู้ตัวตนของเรา - ตัวตน *ที่แท้จริง* ของเรา - ทุกคนก็จะกลัวเรา

`bb({ eyes:"sad" });`

{{if _.a4_fears_discussed==1}}
b: อึม ก็ไม่รู้ล่ะ *ฉัน* เป็นคนเลือกคำพูดมาสักพักนึงละ *นาย* ว่ายังไงบ้างมนุษย์?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: ไปที่นายอีกที นายคิดว่ายังไงบ้าง?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: คิดว่าไงมนุษย์?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[ชั้นเห็นด้วย เรามาปรับปรุงการเข้าสังคมของเราเถอะ](#act4_alone_skills)

[ชั้นว่าคนอื่นๆ ชอบเรานะ ลองดูมั้ย](#act4_alone_experiment)

[ขอบใจนะ](#act4_thanks) `_.thanks_for = "การมีที่ยืนในสังคม";`

# act4_alone_skills

```
bb({ eyes:"normal" });
hong({ body:"chin" });
```

h: เราสามารถฝึกทักษะการสื่อสาร เช่น การถามคำถาม การฟังและการทำความเข้าใจ การเปิดใจและยอมรับจุดอ่อนของเรา เป็นต้น?

`hong({ eyes:"normal_l" });`

h: หรือพยายามฝึกนิสัยการเข้าสังคมของเรา แบ่งเวลาให้เพี่อนของเรา หรือนัดกับเพี่อนเป็นประจำ?

`hong({ body:"one_up" });`

h: จริงๆ ฝึกให้รับการปฏิเสธได้ด้วยก็ดี

`hong({ eyes:"normal" });`

h: หรือฝึกให้มองออกว่าคนอื่น *ไม่ได้* ปฏิเสธเรา เขาอาจแค่เหนี่อย หรือว่าเขาอาจหน้าชาแต่เกิดก็ได้

```
hong({ body:"normal" });
bb({ eyes:"annoyed_r" });
```

b: มีให้เลือกหลายอย่างแฮะ แต่ไอ้ "สกิลเข้าสังคม" เนี่ย...

[มันไม่ *เอาเปรียบคนอื่น* เหรอ?](#act4_alone_skills_manipulative)

[มันไม่ทำให้เรา *ถูกเอาเปรียบ* เหรอ?](#act4_alone_skills_manipulated)

[แล้วถ้าเราล้มเหลวล่ะ?](#act4_alone_skills_fail)

# act4_alone_skills_manipulative

`bb({ eyes:"suspect" });`

b: พวกฆาตกรต่อเนี่องนี่เขาอ่านอารมณ์เหยื่อออก ไม่ใช่เพราะ "ความเห็นใจ" เหรอ?

`bb({ eyes:"annoyed" });`

b: แบบ Charles Manson เขาไม่ได้ชนะใจเพี่อนกับโน้มน้าวคนหรือไง?

`hong({ eyes:"annoyed", body:"chin" });`

h: ไม่ แกพูดถูก

h: "สกิลเข้าสังคม" จะไม่มีความหมาย ถ้าเราไม่แคร์คนอื่นจริงๆ

`hong({ body:"normal" });`

h: พูดง่ายๆ คืออย่าทำตัว^เหี้ย^

`bb({ eyes:"annoyed", mouth:"smile" });`

b: เอาเป็นคำคมไปแปะโปสเตอร์ได้เลยนะเนี่ย

`hong({ body:"shrug", mouth:"narrow" });`

h: “อย่าทำตัว^เหี้ย^™”

(#act4_something_else)

# act4_alone_skills_manipulated

`bb({ eyes:"angry" })`

b: พวกเราจะกลายเป็นเสื่อรองต้อนรับ ขอบคุณชาวบ้านที่มาเหยียบย่ำเช็ดเท้าบนตัวเรา!

`bb({ mouth:"scream", eyes:"scream" })`

b: เราจะเลียตูดใครต่อใครจนปากจะมีน้ำตาล!

```
bb({ mouth:"normal", eyes:"normal" });
hong( body:"chin" });
```

h: ม่าย แกพูดถูก "สกิลเข้าสังคม" ไม่ใช่ทำให้คนอื่นพอใจอย่างเดียว เราต้องเขียน *ขอบเขต* ของเราด้วย

`hong( body:"one_up" });`

h: เราจะเชิญคนอื่นเข้าบ้านเราไม่ได้ ถ้าบ้านเรามันไม่มีกำแพง

```
hong( eyes:"angry", mouth:"narrow" });
bb( eyes:"annoyed", mouth:"smile" });
```

h: อีกอย่าง... เรี่องปากนี่มัน... *แหวะ??*

(#act4_something_else)

# act4_alone_skills_fail

`bb({ eyes:"annoyed" });`

h: เราอาจล้มเหลว ไม่สิ เรา *จะ* ล้มเหลว

```
bb({ eyes:"normal" });
hong({ eyes:"surprise", body:"shrug" });
```

h: แต่ก็ไม่เป็นไร! การล้มเหลวก็เป็นวิธีที่ทุกคนเรียนรู้สิ่งใหม่!

`hong({ body:"normal", eyes:"normal" });`

h: เรามาล้มเหลวไปข้างหน้าด้วยกันเนอะ?

`bb({ eyes:"normal_r" });`

b: ก็ได้... อย่างแย่ที่สุด เราหนีไปอยู่เมืองใหม่แล้วเปลียนชื่อ

`bb({ eyes:"normal" });`

h: เออเดี๋ยวนี้แบบนั้นก็ตกอยู่ที่ 2 Bitcoin มั้ง

(#act4_something_else)

# act4_alone_experiment

```
hong({ body:"one_up" });
bb({ eyes:"normal" });
```

h: เรามาลองทดลองกันดูก็ได้นะ!

`hong({ body:"chin" });`

h: เราจะลองชวนเพี่อนมาเดินเล่นกัน หรือว่าจะลองไปคุยกับเพี่อนเก่า หรือไม่ก็แค่คุยกับบาริสต้ายังได้เลย

`hong({ body:"normal" });`

h: บางที เราอาจค้นพบว่ามีคนชอบเรามากกว่าที่เราคิดนะ

`bb({ eyes:"annoyed" });`

[แล้วถ้านี่เป็นแค่ "ชัยชนะ" แบบง่ายๆ ถูกๆ ล่ะ?](#act4_alone_experiment_cheap)

[แล้วถ้ามันทำให้เราเป็นภาระคนอื่นล่ะ?](#act4_alone_experiment_burden)

[แต่ไอ้การคุยยิบย่อยมันไม่ใช่ตัวตนเรา *จริงๆ* นะ!](#act4_alone_experiment_real_us)

# act4_alone_experiment_real_us

`bb({ eyes:"sad" });`

b: ถ้าเราแค่ยิ้มแบบตื้นๆ เราจะไม่สามารถสนิทกับใครได้เลย

`bb({ eyes:"super_sad" });`

b: *แต่* ถ้าเราเปิดตัวตนของเรา คนอื่นก็จะเห็นอะไรแย่ๆของเราทุกอย่าง!

`hong({body:"chin", mouth:"narrow", MOUTH_LOCK:true})`

h: ...

```
hong({body:"normal", mouth:"normal"});
bb({eyes:"normal"});
```

h: กลิ้งตัวหน่อยสิ

b: หะ

`hong({body:"hands_1"})`

h: เวลาหมาอยากแสดงให้เห็นว่ามันรักมันเชื่อใจ มันจะทำให้ตัวเองดูอ่อนโยนลงโดยการนอนหงายท้อง

`hong({body:"one_up"})`

h: บางทีเราอาจ *ยังไม่* รู้สึกมั่นใจพอที่จะยอมรับจุดอ่อนเราแบบนั้น แต่ถ้าเราฝึกมากพอ

`hong({body:"normal", eyes:"surprise"})`

h: วันนึงเราอาจเปิดเผยให้คนเห็นตัวตนเราที่จริง - ตัวตนที่ยุ่งเหยิง ตัวตนที่เป็นมนุษย์

```
hong({eyes:"normal"});
bb({ eyes:"super_sad", mouth:"smile", body:"chest" });
```

b: ฉันจะกลิ้งตัวถ้านายให้ขนมฉันชิ้นนึง

`bb({ eyes:"normal", mouth:"normal" });`

h: ไม่

(#act4_something_else)


# act4_alone_experiment_cheap

b: แค่การทักทายบาริสต้าเฉยๆ นี่มันไม่ได้ใกล้เหรียญทองโอลิมปิกการเข้าสังคมเลยนะ

```
hong({ body:"point", eyes:"surprise" });
bb({ eyes:"normal" });
```

h: แต่ *สำหรับเรา* มันใช่ไง!

`hong({ body:"one_up", eyes:"annoyed" });`

h: ในเวทีเข้าสังคมเรายังไม่ได้รุ่น เฟเธอร์เวทด้วยซ้ำ เราคงเป็น... ขี้ผงเวทมั้ง

`hong({ body:"normal", eyes:"normal" });`

h: ถ้าเราต้องเรี่มจาก "ชัยชนะ" แบบง่ายๆ ถูกๆ แล้วหนักหัวใครล่ะ จะปีนไปถึงขั้นที่ 1000 ก็ต้องผ่านขึ้นที่ 1 ก่อน

b: จริงด้วย! บางทีพอเราพูด "หวัดดี" แล้ว เราอาจข้ามขั้นไปพูด...

`bb({ body:"two_up", mouth:"smile", eyes:"smile_u" });`

b: *"เป็นไงบ้าง?"*

`hong({ body:"shrug", mouth:"smile", eyes:"surprise_l" });`

h: *"สบายดี!"*

(#act4_something_else)

# act4_alone_experiment_burden

`bb({ eyes:"suspect_r" })`

b: บางทีบาริสต้าเขาอาจอยากแค่ทำกาแฟเฉยๆ ไม่ได้อยากมาเป็น *หนูทดลอง* ให้เรารู้ว่าเราเข้าสังคมห่วยแค่ไหนอ่ะนะ

`bb({ eyes:"annoyed" })`

h: เอ่อ ถ้ากลายเป็นว่าไอ้ที่เราทำมัน *เป็น* การรบกวนคนอื่น...

```
hong({ eyes:"surprise" });
bb({ eyes:"normal" });
```

h: รู้ไว้ก็ดีเหมือนกัน!

`hong({ eyes:"normal" });`

h: เราก็จะได้รู้ว่าเราจะถามคนอื่นว่าเขารู้สึกสบายใจกับอะไร แล้วเคารพในขอบเขตของเขา

```
hong({ eyes:"annoyed_l", mouth:"narrow" });
bb({ eyes:"annoyed", mouth:"smile" });
```

h: แบบว่า ไอ้พวก "ทักษะการสื่อสาร" ^ห่าเหว^ที่นักจิตวิทยาชอบใส่ในใบปลิวน่ะ

(#act4_something_else)



# act4_bad

```
_.a4_talked_about_bad = true;
_.a4_fears_discussed += 1;
```

`bb({ eyes:"annoyed_r" })`

b: ฉันต้องการปกป้องความต้องการทางศีลธรรมของนาย ที่ช่วยผลักดันให้นายเป็นคนดีขึ้น

`bb({ eyes:"sad_d" })`

b: แต่บางทีมันก็รู้สึกว่าลึกๆ แล้วพวกเรามัน...พังตั้งแต่พื้นฐาน

`bb({ body:"two_up", eyes:"angry" })`

{{if _.INJURED}}
b: นายพูดไม่ได้นะว่าพวกเรา *ไม่* เพี้ยน พวกเราเพี่งโดด *หลังคา* ไปหยกๆ
{{/if}}

{{if !_.INJURED}}
b: นายพูดไม่ได้นะว่าพวกเรา *ไม่* เพี้ยน พวกเราเพี่งเกือบโดด *หลังคา* ไปหยกๆ
{{/if}}

`bb({ body:"normal", eyes:"sad" })`

{{if _.a4_fears_discussed==1}}
b: อึม ก็ไม่รู้ล่ะ *ฉัน* เป็นคนเลือกคำพูดมาสักพักนึงละ *นาย* ว่ายังไงบ้างมนุษย์?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: ไปที่นายอีกที นายคิดว่ายังไงบ้าง?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: คิดว่าไงมนุษย์?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[พวกเราพังเหรอ งั้นก็ต้องซ่อม](#act4_bad_fix)

[พวกเราพังเหรอ งั้นก็ต้องยอมรับมัน](#act4_bad_accept)

[ขอบใจนะ](#act4_thanks) `_.thanks_for = "ความเป็นอยู่ทางศีลธรรม";`

# act4_bad_fix

```
bb({eyes:"normal"});
hong({body:"chin"});
```

h: เราสามารถค่อยๆ ฝึกนิสัยที่ดีขึ้นได้ ทำให้ชีวิตเข้าทรงกับสิ่งที่เราให้ค่า

`hong({body:"one_up"});`

h: แล้วถ้าจำเป็น เราก็อาจไปให้ผู้เชี่ยวชาญช่วย - นักจิตวิทยาหรือนักบำบัดเป็นต้น

`hong({body:"normal"});`

h: มันก็มีทางแก้ไขอ่ะนะ

[แล้วถ้าเราแก้ไม่ได้ทุกอย่างล่ะ?](#act4_bad_fix_cant)

[แล้วถ้าเราแก้ *มากเกินไป* ละ?](#act4_bad_fix_too_much)

[เราไม่มีตังค์ไปหาผู้เชี่ยวชาญหรอกนะ](#act4_bad_fix_afford)

# act4_bad_fix_cant

`hong({eyes:"annoyed"});`

h: ม่าย ชั้นว่าแกพูดถูก

h: เราแก้ไม่ได้ทุกอย่างหรอก

`bb({mouth:"scream", eyes:"scream_sad"});`

b: อ้าาาก ฉันว่าแล้วเชียวว่าเราจะเป็นคนพังๆ ไปตลอด!

`hong({eyes:"surprise"});`

h: แต่อย่างน้อยเราก็พัง *น้อยลง* ได้

```
bb({mouth:"normal", eyes:"annoyed"});
hong({eyes:"sad", mouth:"smile"});
```

h: แผลเป็นเยียวยาด้วยเวลา แต่มันจะไม่จางหาย มันก็ไม่เป็นไร

`bb({eyes:"annoyed_r"});`

b: นั้นสินะ อีกอย่าง

```
Game.FORCE_TEXT_Y = 460;
Game.clearText();
publish("act4-sexy", [true]);
```

b: แผลเป็นมัน *เซ็กซี่*

```
Game.FORCE_TEXT_Y = -1;
Game.clearText();
publish("act4-sexy", [false]);
bb({body:"chest", mouth:"smile_talk", MOUTH_LOCK:true, eyes:"sexy"}, 0);
hong({eyes:"normal", mouth:"normal"}, 0);
```

h: อย่าหาทำเลย

(#act4_something_else)

# act4_bad_fix_too_much

`bb({ eyes:"angry_d" })`

b: รู้สึกแย่นะที่ต้องยอมรับ แต่ว่า... บางส่วนในตัวฉัน *อยาก* มีอาการนี้

`bb({ eyes:"angry" })`

b: หมายความว่า ถ้าไม่เป็นแล้ว เราจะไม่ *น่าเบื่อ* เหรอ?

`bb({ eyes:"sad_r", body:"one_up" })`

b: ถ้าไม่มีอาการผิดปกติแล้ว งานศิลป์ที่เราสร้างจะไม่จืดชืดไร้ชีวิตเหรอ?

`bb({ eyes:"sad_u", body:"two_up" })`

b: ถ้าไม่มีอาการผิดปกติแล้ว เราจะไม่สามารถเข้าใจเพี่อนเราที่มีอาการนี้เปล่า?

`bb({ eyes:"sad", body:"chest" })`

b: ถ้าเราพอใจกับชีวิตเรา เราจะไม่หยุดผลักดันตัวเองให้ทำอะไรที่ยิ่งใหญ่เหรอ?

`hong({ MOUTH_LOCK:true })`

h: ...

h: ถ้าเรากลัวแม้กระทั่ง... "การไม่มีอะไรให้กลัว"...

h: ชั้นว่าเราจะไม่มีวันที่จะหมดความกลัวล่ะถ้างั้น

`bb({ eyes:"smile_u", body:"normal", mouth:"smile" })`

b: เออ จริงด้วย! เฮ้อ! โล่งอกไปที!

(#act4_something_else)

# act4_bad_fix_afford

`bb({ body:"one_up", eyes:"sexy", mouth:"normal" })`

b: "คุณหมอ ฉันกังวลว่าฉันกำลังจ่ายเงิน $100 ต่อชั่วโมงแค่เพี่อฟังหมอถามว่า *แล้วมันทำให้คุณรู้สึกยังไงบ้าง?*"

`bb({ body:"paw", eyes:"closed", mouth:"narrow" })`

b: "อึม แล้วมันทำให้คุณรู้สึกยังไงบ้าง?"

```
bb({ body:"normal", eyes:"normal", mouth:"normal" });
hong({ eyes:"sad" });
```

h: ม่าย นั่นก็เป็นเรี่องที่ควรจะกังวลแหละ

`hong({ eyes:"annoyed", mouth:"sad" });`

h: จริงๆ มันก็แย่ที่บริการสุขภาพจิตมันแพงเกินไปสำหรับหลายๆ คน

`hong({ eyes:"normal", mouth:"normal" });`

h: อย่างน้อยก็มีทางเลือกที่ถูกกว่า ไม่ก็ฟรี:

`hong({ body:"chin" })`

h: กลุ่มช่วยเหลือ บำบัดจิตออนไลน์ ศูนย์สุขภาพนักศึกษาหรือที่ไม่เอากำไร...

`hong({ body:"hands_1" })`

h: ฝึกนิสัยเช่นนั่งสมาธิ นอนให้ดี คุยกับเพี่อนบ่อยๆ ฝึกทำอะไรใหม่ๆ...

`hong({ body:"hands_2" })`

h: ไปห้องสมุดหาหนังสือเกี่ยวกับการบำบัดจิตมาดู...

`hong({ body:"one_up" })`

h: หลังเกมนี้จบจะมีลิสต์ของแหล่งต่างๆ ให้ดูด้วยนะ

```
hong({ body:"normal" });
bb({ eyes:"annoyed", mouth:"narrow" });
```

b: ออ ไอกำแพงที่สี่นี่พังไปแล้วสินะ

`hong({ body:"point" });`

h: ก็เรื่องบางอย่างมันสำคัญกว่าการเล่าเรี่องน่ะ สุขภาพจิตเป็นต้น

(#act4_something_else)


# act4_bad_accept

```
bb({ eyes:"normal" });
hong({ eyes:"normal_l", body:"one_up", mouth:"narrow" });
```

h: แบบว่า นักจิตวิทยาชอบพูดกันใช่มั้ยล่ะ? ยอมรับอารมณ์ของเรา รวมถึงอารมณ์ทางลบด้วย?

```
bb({ eyes:"annoyed" });
hong({ eyes:"normal", body:"normal", mouth:"normal" });
```

b: เดี๋ยวนะ

["ยอมรับ" นี่คือ *ยอมแพ้*?](#act4_bad_accept_give_up)

["ยอมรับ" นี่คือ *เห็นด้วย*?](#act4_bad_accept_approve)

["ยอมรับ" นี่คือ *รับแบบตรงๆ*?](#act4_bad_accept_literally)

# act4_bad_accept_give_up

`bb({ eyes:"angry", body:"one_up" });`

b: นายคิดว่า Martin Luther King จะพูดว่า "หว่า แย่จังที่เรานั่งหน้ารถเมล์ไม่ได้ คงต้อง *ยอมรับ* อ่ะนะ" เหรอ?

`bb({ eyes:"angry_r", body:"two_up" });`

b: ทำไมอุตสาหกรรมการช่วยเหลือตัวเองถึงคิดว่าการโบกธงขาวเป็น *สัจธรรมอันบรรเจิด*?

`bb({ eyes:"annoyed", body:"normal" });`

h: ชั้นว่านักจิตวิทยาหมายถึง "ยอมรับ" สิ่งที่ไม่ดีว่า มันมีอยู่ และมันยากที่จะเปลี่ยน

h: ไม่ได้หมายความว่าเราจะยอมแพ้กับการเปลี่ยนแปลงนะ

`bb({ eyes:"suspect" });`

b: งั้นพวกนักจิตวิทยาก็ควรพูดว่า *รับรู้* สิ ไม่ใช่ *ยอมรับ*

`hong({ body:"chin", eyes:"annoyed" });`

h: เออจะว่าไปแล้ว "ยอมรับ" เป็นคำที่น่าสับสนไปหน่อยนะ

`bb({ eyes:"closed", mouth:"narrow" });`

b: เออ ฉัน *รับรู้* ไว้แล้วกัน

(#act4_something_else)

# act4_bad_accept_approve

`bb({ eyes:"angry" });`

b: แบบว่ามัน *ดี* แล้วเหรอที่เราพังเราป่วย? ไม่เฟ้ย!

`bb({ eyes:"angry_r", body:"one_up" });`

b: ไอ้พวกนักเขียนฮอลลี่วู้ดที่ชอบทำให้การป่วยทางจิตมันดูน่าหลงไหลมันเหลวไหลทั้งเพ!

`bb({ eyes:"angry", body:"two_up" });`

b: การป่วยทางจิตมัน *แย่*! มันปล้นชีวิตที่ดีจาก *ทุกคน*! ทำไมเราต้องไป "ยอมรับ" มันด้วย?!

`bb({ body:"normal" });`

h: ชั้นว่านักจิตวิทยาหมายถึง "ยอมรับ" อารมณ์เราว่า ให้อดทนกับมัน

```
hong({ body:"one_up" });
bb({ eyes:"normal" });
```

h: คล้ายๆ กับถ้าเราดิ้นในทรายดูดแล้วจะจมเร็วขึ้น วิธีแก้คือนอนนิ่งๆ

`hong({ eyes:"surprise" });`

{{if _.INJURED}}
h: การสู้กับแก สู้กับความกลัว จบด้วยชั้นกระโดดลงจากหลังคา
{{/if}}

{{if !_.INJURED}}
h: การสู้กับแก สู้กับความกลัว เกือบจบด้วยชั้นกระโดดลงจากหลังคา
{{/if}}

`hong({ body:"normal", eyes:"normal" });`

h: แทนที่จะต่อสู้ วิธีแก้คือที่เราทำอยู่ตอนนี้ - ไม่ใช่ต่อสู้ แต่ต้องทนอยู่กับกันและกัน

`bb({ eyes:"annoyed" });`

b: งั้นเขาควรจะพูด *แบบนั้น* แทนที่จะพูดคำที่มีปัญหาแบบ "ยอมรับ" นะ

`hong({ body:"chin", eyes:"annoyed" });`

h: เออจะว่าไปแล้ว "ยอมรับ" เป็นคำที่ไม่ค่อยดีเท่าไหร่ล่ะ

`bb({ eyes:"closed_annoyed", mouth:"narrow" });`

b: ฉันไม่ยอมรับ "ยอมรับ"

(#act4_something_else)

# act4_bad_accept_literally

`bb({ eyes:"sad", body:"one_up" });`

b: แต่เราก็ *รู้* แล้วนี่ว่านายไม่ควรฟังฉันแล้วทำตามทุกอย่าง!

`bb({ eyes:"sad_u", body:"two_up" });`

b: ปัญหาทั้งหมดก็คือฉันอยากช่วยนาย แต่ฉันห่วยแตกเรี่องการใช้คำพูดมาช่วยนายนี่สิ!

`bb({ eyes:"sad", body:"normal" });`

h: ชั้นว่านักจิตวิทยาหมายถึง "ยอมรับ" อารมณ์เราว่า "อย่าต่อสู้ อย่าเมินเฉย"

`hong({ eyes:"surprise", body:"one_up" });`

h: รับฟังแก ทำงาน *กับ* แก แต่ไม่ต้องตีทุกอย่างที่แกพูดว่าเป็นจริง 100%

```
hong({ eyes:"normal", body:"normal" });
bb({ eyes:"annoyed", mouth:"normal" });`
```

b: ถ้างั้นนักจิตวิทยาควรจะพูด *แบบนั้น* แทนที่จะพูดคำที่คลุมเครือสับสนอย่าง "ยอมรับ" อ่ะนะ

`hong({ body:"chin", eyes:"annoyed" });`

h: ชั้นว่าพวกเขาคงห่วยแตกเรี่องใช้คำพูดเหมือนกัน

(#act4_something_else)




# act4_something_else

```
bb({ body:"normal", mouth:"normal", eyes:"normal" });
hong({ body:"normal", mouth:"normal", eyes:"normal" });
```

{{if _.a4_fears_discussed==1}}
h: นอกจากนี้แกอยากคุยอะไรอีกมั้ย?
{{/if}}

{{if _.a4_fears_discussed==2}}
h: มีอะไรฝังอยู่ในใจอีกมั้ย?
{{/if}}

{{if _.a4_fears_discussed==3}}
(#act4_something_else_2)
{{/if}}

{{if _.a4_talked_about_harm!=true}}
[ฉันกลัวว่าเราจะถูกทำร้าย](#act4_harm)
{{/if}}

{{if _.a4_talked_about_alone!=true}}
[ฉันกลัวว่าพวกเราจะเดียวดาย](#act4_alone)
{{/if}}

{{if _.a4_talked_about_bad!=true}}
[ฉันกลัวว่าพวกเราเป็นคนไม่ดี](#act4_bad)
{{/if}}

[ม่าย พอแค่นี้ก่อน](#act4c_prelude)

# act4_something_else_2

h: โอเค ชั้นว่าเราคุยเรี่องความกลัวครบทุกอย่างละ

b: ใช่ มีความกลัวแค่สามอย่าง

h: อึม สามอย่างพอดี

b: สะดวกจัง

(#act4c)

# act4c_prelude

h: คุยได้ดี

(#act4c)

# act4c

```
Game.clearText();
music(null,{fade:3});
bb({body:"normal", eyes:"normal", mouth:"normal", MOUTH_LOCK:true},0);
hong({body:"normal", eyes:"normal", mouth:"normal"},0);
```

b: ...

`hong({MOUTH_LOCK:true},0)`

h: ...

`bb({eyes:"annoyed_d"})`

b: นี่มันไม่ใช่แค่ *เกม* นะ รู้มั้ย

`bb({eyes:"angry_d", body:"one_up"})`

b: การสร้างเสริมความสัมพันธ์ที่ดีกับอารมณ์มันไม่ได้ง่ายเหมือนการกดปุ่มบนหน้าจอหรอกนะ

`bb({eyes:"sad", body:"normal"})`

b: เราดีกัน *ได้ไหม*?

b: เราทำงานด้วยกัน เป็นทีม *ได้ไหม*?

`hong({eyes:"sad", body:"one_up"})`

h: เอ่อ

```
hong({eyes:"surprise_l"});
bb({eyes:"normal"});
```

a: ท-โทษทีนะ...

```
Game.clearText();
publish("act4-in-2");
music('campus', {volume:0.5, fade:1});
```

(...2101)

(#act4d)

# act4d

`Game.WORDS_HEIGHT_BOTTOM = 221;`

`publish("act4", ["alshire", 0]);`

a: ถ-ถ-ถ้าเราจะนั่งกินข้าวด้วยคนจะรังเกียจมั้ย?

`publish("act4", ["alshire", 1]);`

{{if _.TOP_FEAR=="harm"}}
s: *นี่* คนที่แกชอบเหรอ? ทำไมเขาถึงนั่งคนเดียวเหมือนฆาตกรโรคจิต?
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: แกขอนั่งกับคนที่แกชอบเหรอ? รู้มั้ยว่ามันฟังดู *เห็นแก่ตัว* แค่ไหน?!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: *นี่* คนที่แกชอบเหรอ? เราไปรบกวนความเงียบสงบเขาอยู่นะ! เรานี่มันกวนคนอื่นตลอดเลยนี่หว่า!
{{/if}}

`publish("act4", ["alshire", 2]);`

a: ถ-ถ-ถ้าไม่ได้นะ ไม่ได้ก็ไม่เป็นไร เราก็อยากแค่...

`publish("act4", ["alshire", 3]);`

`Game.OVERRIDE_CHOICE_SPEAKER = "h2"`

[เดี๋ยวนะ ชั้นไม่ได้เห็นแกที่ปาร์ตี้เหรอ?](#act4d_recognition) `publish("act4", ["hong_to_alshire",1])`

[ได้สิ! นั่งได้เลย](#act4d_yes) `publish("act4", ["hong_to_alshire",2])`

[โทษนะ แต่ตอนนี้ชั้นอยากอยู่คนเดียว](#act4d_no) `publish("act4", ["hong_to_alshire",8])`

# act4d_recognition

`publish("act4", ["hong_to_alshire",2]);`

h2: ใช่ แกอยู่บนโซฟานี่นา! ในปารตี้แรกที่ชั้นไป...

`publish("act4", ["hong_to_alshire",10]);`

{{if _.a2_ending=="fight"}}
h2: ที่ชั้นเกิดแพนิกแล้วชกหน้าคนจัดงาน
{{/if}}

{{if _.a2_ending=="flight"}}
h2: ที่ชั้นเกิดแพนิกแล้ววิ่งหนีไปร้องไห้ไป
{{/if}}

```
publish("act4", ["hong_to_alshire", 0]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: เดี๋ยวนะมนุษย์ เราอาจกำลังทำให้เขาไม่สบายใจ

```
publish("act4", ["hong_to_alshire", 3]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: อ้อ ไม่ได้ตั้งใจทำให้ตกใจหรอกนะ!

`publish("act4", ["hong_to_alshire",4]);`

h2: แค่จำหน้าที่เป็นมิตรได้เท่านั้นเอง

```
publish("act4", ["hong_to_alshire",5]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: ว้าาาก ว่าแล้วเชียว! นี่มันเป็นโรคจิตเจ้าแพนิกอันตราย!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: ว้าาาก ความทรงจำแรกของเขาเกี่ยวกับเราคือ "เห็นบาดแผลทางอารมณ์ของชั้น"! หมายความว่าเขาเกลียดเรา!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: ว้าาาก เราทำให้คนอื่นจำเหตุการร้ายๆ การมีอยู่ของเราทำให้คนอื่นเจ็บปวด
{{/if}}

(#act4e)

# act4d_yes

```
publish("act4", ["hong_to_alshire", 5]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: เดี๋ยวนะมนุษย์ เขาดูไม่สบายใจยังไงก็ไม่รู้

```
publish("act4", ["hong_to_alshire", 6]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: อ้อ ไม่เป็นไรนะ!

`publish("act4", ["hong_to_alshire", 4]);`

h2: แค่จะบอกแค่ว่า ถ้าอยากนั่งตรงนี้ก็มาได้

```
publish("act4", ["hong_to_alshire", 5]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: เขาดูเป็นมิตร *เกินไป*! แบบ Ted Bundy ที่เป็นฆาตกรต่อเนี่องไง!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: เขาก็แค่เชิญตามมารยาท! ไม่มีใครอยากเป็นเพี่อนเรา *จริงๆ* หรอก!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: ว้าาาก เราทำให้คนอื่นรู้สึกอักอ่วม! เรามันเป็นรอยแปดเปื้อนบนโลกนี้!
{{/if}}

(#act4e)

# act4d_no

```
publish("act4", ["hong_to_alshire", 9]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: เดี๋ยวนะมนุษย์ เราอาจกำลังทำให้เขาไม่สบายใจ

```
publish("act4", ["hong_to_alshire", 3]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: อ้อ ไม่ได้จงใจหยาบคายนะ

`publish("act4", ["hong_to_alshire", 6]);`

h2: ชั้นแค่ขอเวลาประมวลอารมณ์แปปนึง อย่าถือว่าเป็นการปฎิเสธเลยนะ

```
publish("act4", ["hong_to_alshire", 7]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: เขาคิดอะไรแปลกๆ ในหัวอยู่?! ไอโรคจิตนั่นมันมันมีอะไรในใจเหรอ?!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: เราเพี่งถูกปฎิเสธนะ! เราจะไม่มีใครรักตลอดกาล!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: เราไปรบกวนการประมวลอารมณืเขา! เขาจะทุกข์ทรมานไปทั้งชีวิตแล้วนั่นเป็นความผิดของเรา!
{{/if}}

(#act4e)

# act4e

```
Game.WORDS_HEIGHT_BOTTOM = 195;
publish("act4", ["alshire", 6]);
```

s: วิ่ง! วิ่ง! วิ่ง! วิ่ง! วิ่ง! วิ่ง! วิ่ง! วิ่ง! วิ่ง! วิ่ง! วิ่ง! วิ่ง! วิ่ง! วิ่ง! วิ่ง!

```
Game.clearText();
publish("act4", ["hong_to_alshire", 0]);
publish("act4", ["alshire", 10]);
sfx("pop");
```

(...1001)

```
publish("act4", ["alshire", 11]);
sfx("alshire_run");
```

(...2601)

```
publish("act4-out-3");
Game.WORDS_HEIGHT_BOTTOM = -1; /* reset */
```

(...1201)

`publish("act4-jumpcut-hong");`

h: เอ้อ แปลกแฮะ สงสัยจังว่าในหัวเขาคิดอะไรอยู่

`publish("act4", ["hong_closer", 2]);`

h: เออจะว่าไปแล้ว ตะกี้แกว่าไงนะ

```
publish("act4", ["hong_closer", 1]);
publish("act4", ["bb_closer", 6]);
```

b: เอ่อ ฉันลืมไปแล้ว อะไรเกี่ยวกับทีมกับทำงานนี่แหละ

```
publish("act4", ["bb_closer", 0]);
publish("act4", ["hong_closer", 3]);
```

h: ¯\_(ツ)_/¯

```
publish("act4", ["hong_closer", 1]);
publish("act4", ["bb_closer", 4]);
```

b: หลายคนชอบพูดว่าต้อง "รักษาความสงบ" กับอารมณ์ตัวเอง อย่างกับว่าอารมณ์คือ *อาชญากรสงคราม*

`publish("act4", ["bb_closer", 7]);`

b: แต่ฉันอยากได้ *มากกว่า* แค่สงบสุขสิ! ฉันอยากเป็น *พันธมิตร* กับนาย!

`publish("act4", ["bb_closer", 3]);`

b: ฉันอยากเป็นหมาเฝ้าบ้านที่ดีนะ เหมือนดั่งว่าความหิวกับความกระหายเป็นการเตือนถึงความต้องการทางร่างกาย

`publish("act4", ["bb_closer", 8]);`

b: ฉันอยากเป็นการเตือนถึงความต้องการทาง *จิตใจ* - ความต้องการความปลอดภัย การมีที่ยืน ความเป็นคนดี

`publish("act4", ["bb_closer", 1]);`

b: แต่... ฉันทำหน้าที่ไม่เก่งน่ะสิ นายจะต้องฝึกฉัน

`publish("act4", ["bb_closer", 4]);`

b: ฉันไม่ได้ "ถูกต้องเสมอ" หรือ "ไร้เหตุผลเสมอ" ฉันแค่... พยายามเต็มที่ ขอร้องล่ะ

`publish("act4", ["bb_closer", 30]);`

b: ช่วยฉันช่วยนาย!

`publish("act4", ["bb_closer", 6]);`

b: แต่บางที ไม้แก่มันก็ดัดยาก อาจใช้เวลานาน อาจเป็น *ปีๆ*

`publish("act4", ["bb_closer", 3]);`

b: แล้วบางครั้งฉันก็จะกลับไปทำแบบเดิม ติดนิสัยเก่า

`publish("act4", ["bb_closer", 2]);`

b: ฉันจะเห่าเงาบ้าง ใช้คำพูดขู่ให้กลัวบ้าง ฉันอาจบังคับให้นายดูรูป...อะไรที่ไม่น่าดูบ้าง

`publish("act4", ["bb_closer", 9]);`

b: ฉันขอโทษด้วย! ฉันเป็นหมาที่เคยถูกทำร้าย! บางทีหมาแบบนั้นก็อึรดเตียงนาย!

`publish("act4", ["bb_closer", 4]);`

b: แต่ถ้านายอดทนกับฉัน... แล้วนั่งอยู่กับฉัน...

`publish("act4", ["bb_closer", 8]);`

b: นายอาจทำให้หมาป่าตัวนี้เชี่องได้นะ

`publish("act4", ["bb_closer", 0]);`

`Game.clearText();`

(...1000)

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[หมาน่ารัก](#act4f-pat-bb) `Game.OVERRIDE_CHOICE_SPEAKER = "h"; publish("act4", ["hong_closer", 2]);`

`Game.OVERRIDE_CHOICE_SPEAKER = "b"`

[มนุษย์น่ารัก](#act4f-pat-hong) `Game.OVERRIDE_CHOICE_SPEAKER = "b"; publish("act4", ["bb_closer", 8]);`

# act4f-pat-hong

```
Game.clearText();
publish("hide_tabs");
Game.FORCE_CANT_SKIP = true;
music(null,{fade:0.5});
sfx("youbothwin");
```

```
publish("act4", ["hong_closer", 4]);
publish("act4", ["bb_closer", 13]);
```

(...501)

`publish("act4", ["bb_closer", 14]);`

(...501)

`publish("act4", ["bb_closer", 13]);`

(...501)

`publish("act4", ["bb_closer", 14]);`

(...501)

`publish("act4", ["bb_closer", 13]);`

(...501)

`publish("act4", ["bb_closer", 14]);`

(...6501)

`publish("act4", ["bb_closer", 15]);`

(...1001)

(#act4f)

# act4f-pat-bb

```
Game.clearText();
publish("hide_tabs");
Game.FORCE_CANT_SKIP = true;
music(null,{fade:0.5});
sfx("youbothwin");
```

```
publish("act4", ["hong_closer", 4]);
publish("act4", ["bb_closer", 10]);
```

(...501)

`publish("act4", ["bb_closer", 11]);`

(...501)

`publish("act4", ["bb_closer", 10]);`

(...501)

`publish("act4", ["bb_closer", 11]);`

(...501)

`publish("act4", ["bb_closer", 10]);`

(...501)

`publish("act4", ["bb_closer", 11]);`

(...6501)

`publish("act4", ["bb_closer", 12]);`

(...1001)

(#act4f)

# act4f

```
Game.FORCE_CANT_SKIP = false;
publish("act4", ["bb_closer", 16]);
publish("act4", ["hong_closer", 5]);
```

{{if _.fifteencigs}}
b: ว้าาาาก นายยังกินคนเดียว บุหรี่สิบห้ามวน ว้าาาาาก!!!
{{/if}}

{{if _.parasite}}
b: ว้าาาาก นายยังไม่ทำงานหระหว่างกิน พวกเราเป็นปรสิตสังคม ว้าาาาาก!!!
{{/if}}

{{if _.whitebread}}
b: ว้าาาาก นายกินขนมปังขาวอีกแล้ว ว้าาาาาก!!!
{{/if}}

```
publish("act4", ["bb_closer", 18]);
publish("act4", ["hong_closer", 6]);
sfx("yaps", {volume:0.6});
Game.FORCE_CANT_SKIP = true;
Game.WORDS_HEIGHT_BOTTOM = 205;
Game.FORCE_TEXT_DURATION = 90;
Game.FORCE_NO_VOICE = true;
```

b: โฮ่ง โฮ่ง โฮ่ง โฮ่ง โฮ่ง

(#credits)
