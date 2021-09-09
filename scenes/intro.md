# intro

`SceneSetup.intro();`

# intro-play-button

(...51)

```
_.PLAYED_BEFORE = !!window.localStorage.continueChapter;
```

{{if !_.PLAYED_BEFORE}}
`Game.OVERRIDE_FONT_SIZE=30;`
{{/if}}

{{if !_.PLAYED_BEFORE}}
[#play1# เรี่มเล่น! #play2#](#intro-start) `publish("intro-to-game-1"); Game.OVERRIDE_CHOICE_LINE=true;`
{{/if}}

{{if _.PLAYED_BEFORE && window.localStorage.continueChapter=="act2"}}
[_เล่นต่อ_: ปาร์ตี้](#act2) `publish("LOAD_GAME", ["act2"]); Game.OVERRIDE_CHOICE_LINE=true;`
{{/if}}

{{if _.PLAYED_BEFORE && window.localStorage.continueChapter=="act3"}}
[_เล่นต่อ_: ปาร์ตี้อีกที](#act3) `publish("LOAD_GAME", ["act3"]); Game.OVERRIDE_CHOICE_LINE=true;`
{{/if}}

{{if _.PLAYED_BEFORE && window.localStorage.continueChapter=="act4"}}
[_เล่นต่อ_: แซ็นด์วิชอีกชิ้น](#act4) `publish("LOAD_GAME", ["act4"]); Game.OVERRIDE_CHOICE_LINE=true;`
{{/if}}

{{if _.PLAYED_BEFORE && window.localStorage.continueChapter=="replay"}}
`Game.OVERRIDE_FONT_SIZE=30;`
{{/if}}

{{if _.PLAYED_BEFORE && window.localStorage.continueChapter=="replay"}}
[#play1# เล่นใหม่! #play2#](#intro-start) `publish("intro-to-game-1"); Game.OVERRIDE_CHOICE_LINE=true;`
{{/if}}

{{if _.PLAYED_BEFORE}}
[เลือกตอน](#chapter-select) `Game.OVERRIDE_CHOICE_LINE=true;`
{{/if}}

[(เกี่ยวกับเนื้อหา)](#intro-play-button) `Game.OVERRIDE_CHOICE_LINE=true; publish('show_cn');`

# chapter-select

`publish("HACK_chselect");`

[I. แซ็นด์วิช](#intro-start) `publish("HACK_chselect_end"); publish("intro-to-game-1"); Game.OVERRIDE_CHOICE_LINE=true;`

[II. ปาร์ตี้]](#act2) `publish("HACK_chselect_end"); publish("LOAD_GAME", ["act2"]); Game.OVERRIDE_CHOICE_LINE=true;`

{{if window.localStorage.act3}}
[III. ปาร์ตี้อีกที](#act3) `publish("HACK_chselect_end"); publish("LOAD_GAME", ["act3"]); Game.OVERRIDE_CHOICE_LINE=true;`
{{/if}}

{{if !window.localStorage.act3}}
[III. ปาร์ตี้อีกที]()
{{/if}}

{{if window.localStorage.act4}}
[IV. แซ็นด์วิชอีกชิ้น](#act4) `publish("HACK_chselect_end"); publish("LOAD_GAME", ["act4"]); Game.OVERRIDE_CHOICE_LINE=true;`
{{/if}}

{{if !window.localStorage.act4}}
[III. แซ็นด์วิชอีกชิ้น]()
{{/if}}

{{if window.localStorage.credits}}
[V. เครดิท](#to-credits) `publish("HACK_chselect_end"); Game.OVERRIDE_CHOICE_LINE=true;`
{{/if}}

{{if !window.localStorage.credits}}
[V. เครดิท]()
{{/if}}

[(หน้าหลัก)](#intro-play-button) `publish("HACK_chselect_end"); Game.OVERRIDE_CHOICE_LINE=true;`

# to-credits

`stopAllSounds();`

(...101)

(#credits)

# intro-start

(...500)

`clearText()`

n3: ยินดีต้อนรับ! นี่อาจไม่ค่อยเป็น "เกม" เท่าไหร่ จะออกแนวเนื้อ\
เรี่องเลือกได้มากกว่า หวังว่าคุณจะชอบการอ่านนะ

n3: ก่อนเราจะเรี่มกัน *คุณ* อยากอ่านเร็วแค่ไหน?

`publish("show_options_bottom")`

# intro-start-2

n3: เยี่ยม! เพี่มเติม: การตั้งค่าสามารถทำได้ตลอดด้วยการกดปุ่ม ⚙ ข้างล่าง และเกมจะออโต้เซฟทุกบท

n3: เรามาเรี่มเรี่องของเรากันเลย...

`clearText()`

(...1000)

`publish("intro-to-game-2")`

n2: นี่คือมนุษย์

(...600)

`clearText()`

(...300)

`publish("intro-to-game-3")`