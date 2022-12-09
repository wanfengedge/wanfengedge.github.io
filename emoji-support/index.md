# Emoji 支持

Emoji 可以通过多种方式在 Hugo 项目中启用.

<!--more-->

[`emojify`](https://gohugo.io/functions/emojify/) 方法可以直接在模板中调用, 或者使用[行内 Shortcodes](https://gohugo.io/templates/shortcode-templates#inline-shortcodes).

要全局使用 emoji, 需要在你的[网站配置](https://gohugo.io/getting-started/configuration/)中设置 `enableEmoji` 为 `true`,
然后你就可以直接在文章中输入 emoji 的代码.

它们以**冒号**开头和结尾，并且包含 emoji 的 **代码**:

```markdown
去露营啦! {?:}tent: 很快就回来.

真开心! {?:}joy:
```

呈现的输出效果如下:

去露营啦! ⛺️ 很快就回来.

真开心! 😂

以下**符号清单**是 emoji 代码的非常有用的参考.

## 表情与情感

### 笑脸表情

| 图标 | 代码                              | 图标 | 代码                 |
| :--: | --------------------------------- | :--: | -------------------- |
|  😀  | `grinning`                      |  😃  | `smiley`           |
|  😄  | `smile`                         |  😁  | `grin`             |
|  😆  | `laughing` <br /> `satisfied` |  😅  | `sweat_smile`      |
|  🤣  | `rofl`                          |  😂  | `joy`              |
|  🙂  | `slightly_smiling_face`         |  🙃  | `upside_down_face` |
|  😉  | `wink`                          |  😊  | `blush`            |
|  😇  | `innocent`                      |      |                      |

### 爱意表情

| 图标 | 代码                    | 图标 | 代码                     |
| :--: | ----------------------- | :--: | ------------------------ |
|  😍  | `heart_eyes`          |  😘  | `kissing_heart`        |
|  😗  | `kissing`             | ☺️ | `relaxed`              |
|  😚  | `kissing_closed_eyes` |  😙  | `kissing_smiling_eyes` |

### 吐舌头表情

| 图标 | 代码                             | 图标 | 代码                             |
| :--: | -------------------------------- | :--: | -------------------------------- |
|  😋  | `yum`                          |  😛  | `stuck_out_tongue`             |
|  😜  | `stuck_out_tongue_winking_eye` |  😝  | `stuck_out_tongue_closed_eyes` |
|  🤑  | `money_mouth_face`             |      |                                  |

### 带手的表情

| 图标 | 代码     | 图标 | 代码         |
| :--: | -------- | :--: | ------------ |
|  🤗  | `hugs` |  🤔  | `thinking` |

### 中性表情

| 图标 | 代码                  | 图标 | 代码             |
| :--: | --------------------- | :--: | ---------------- |
|  🤐  | `zipper_mouth_face` |  😐  | `neutral_face` |
|  😑  | `expressionless`    |  😶  | `no_mouth`     |
|  😏  | `smirk`             |  😒  | `unamused`     |
|  🙄  | `roll_eyes`         |  😬  | `grimacing`    |
|  🤥  | `lying_face`        |      |                  |

### 困倦的表情

| 图标 | 代码         | 图标 | 代码              |
| :--: | ------------ | :--: | ----------------- |
|  😌  | `relieved` |  😔  | `pensive`       |
|  😪  | `sleepy`   |  🤤  | `drooling_face` |
|  😴  | `sleeping` |      |                   |

### 不适的表情

| 图标 | 代码                       | 图标 | 代码                      |
| :--: | -------------------------- | :--: | ------------------------- |
|  😷  | `mask`                   |  🤒  | `face_with_thermometer` |
|  🤕  | `face_with_head_bandage` |  🤢  | `nauseated_face`        |
|  🤧  | `sneezing_face`          |  😵  | `dizzy_face`            |

### 戴帽子的表情

| 图标 | 代码                | 图标 | 代码 |
| :--: | ------------------- | :--: | ---- |
|  🤠  | `cowboy_hat_face` |      |      |

### 戴眼镜的表情

| 图标 | 代码           | 图标 | 代码          |
| :--: | -------------- | :--: | ------------- |
|  😎  | `sunglasses` |  🤓  | `nerd_face` |

### 担心的表情

| 图标 | 代码                       | 图标 | 代码              |
| :--: | -------------------------- | :--: | ----------------- |
|  😕  | `confused`               |  😟  | `worried`       |
|  🙁  | `slightly_frowning_face` | ☹️ | `frowning_face` |
|  😮  | `open_mouth`             |  😯  | `hushed`        |
|  😲  | `astonished`             |  😳  | `flushed`       |
|  😦  | `frowning`               |  😧  | `anguished`     |
|  😨  | `fearful`                |  😰  | `cold_sweat`    |
|  😥  | `disappointed_relieved`  |  😢  | `cry`           |
|  😭  | `sob`                    |  😱  | `scream`        |
|  😖  | `confounded`             |  😣  | `persevere`     |
|  😞  | `disappointed`           |  😓  | `sweat`         |
|  😩  | `weary`                  |  😫  | `tired_face`    |

### 否定的表情

| 图标 | 代码                     | 图标 | 代码                     |
| :--: | ------------------------ | :--: | ------------------------ |
|  😤  | `triumph`              |  😡  | `pout` <br /> `rage` |
|  😠  | `angry`                |  😈  | `smiling_imp`          |
|  👿  | `imp`                  |  💀  | `skull`                |
| ☠️ | `skull_and_crossbones` |      |                          |

### 特殊打扮的表情

| 图标 | 代码                                       | 图标 | 代码                |
| :--: | ------------------------------------------ | :--: | ------------------- |
|  💩  | `hankey` <br /> `poop` <br /> `shit` |  🤡  | `clown_face`      |
|  👹  | `japanese_ogre`                          |  👺  | `japanese_goblin` |
|  👻  | `ghost`                                  |  👽  | `alien`           |
|  👾  | `space_invader`                          |  🤖  | `robot`           |

### 猫脸表情

| 图标 | 代码            | 图标 | 代码                |
| :--: | --------------- | :--: | ------------------- |
|  😺  | `smiley_cat`  |  😸  | `smile_cat`       |
|  😹  | `joy_cat`     |  😻  | `heart_eyes_cat`  |
|  😼  | `smirk_cat`   |  😽  | `kissing_cat`     |
|  🙀  | `scream_cat`  |  😿  | `crying_cat_face` |
|  😾  | `pouting_cat` |      |                     |

### 猴脸表情

| 图标 | 代码              | 图标 | 代码             |
| :--: | ----------------- | :--: | ---------------- |
|  🙈  | `see_no_evil`   |  🙉  | `hear_no_evil` |
|  🙊  | `speak_no_evil` |      |                  |

### 情感

| 图标 | 代码                          |  图标  | 代码                  |
| :--: | ----------------------------- | :----: | --------------------- |
|  💋  | `kiss`                      |   💌   | `love_letter`       |
|  💘  | `cupid`                     |   💝   | `gift_heart`        |
|  💖  | `sparkling_heart`           |   💗   | `heartpulse`        |
|  💓  | `heartbeat`                 |   💞   | `revolving_hearts`  |
|  💕  | `two_hearts`                |   💟   | `heart_decoration`  |
| ❣️ | `heavy_heart_exclamation`   |   💔   | `broken_heart`      |
| ❤️ | `heart`                     |   💛   | `yellow_heart`      |
|  💚  | `green_heart`               |   💙   | `blue_heart`        |
|  💜  | `purple_heart`              |   🖤   | `black_heart`       |
|  💯  | `100`                       |   💢   | `anger`             |
|  💥  | `boom` <br /> `collision` |   💫   | `dizzy`             |
|  💦  | `sweat_drops`               |   💨   | `dash`              |
|  🕳  | `hole`                      |   💣   | `bomb`              |
|  💬  | `speech_balloon`            | 👁‍🗨 | `eye_speech_bubble` |
|  🗯  | `right_anger_bubble`        |   💭   | `thought_balloon`   |
|  💤  | `zzz`                       |        |                       |

## 人与身体

### 张开手掌的手势

| 图标 | 代码                                 | 图标 | 代码                            |
| :--: | ------------------------------------ | :--: | ------------------------------- |
|  👋  | `wave`                             |  🤚  | `raised_back_of_hand`         |
|  🖐  | `raised_hand_with_fingers_splayed` |  ✋  | `hand` <br /> `raised_hand` |
|  🖖  | `vulcan_salute`                    |      |                                 |

### 部分手指的手势

| 图标 | 代码                | 图标 | 代码      |
| :--: | ------------------- | :--: | --------- |
|  👌  | `ok_hand`         | ✌️ | `v`     |
|  🤞  | `crossed_fingers` |  🤘  | `metal` |
|  🤙  | `call_me_hand`    |      |           |

### 一根手指的手势

| 图标 | 代码           | 图标 | 代码                            |
| :--: | -------------- | :--: | ------------------------------- |
|  👈  | `point_left` |  👉  | `point_right`                 |
|  👆  | `point_up_2` |  🖕  | `fu` <br /> `middle_finger` |
|  👇  | `point_down` | ☝️ | `point_up`                    |

### 握紧的手势

| 图标 | 代码                            | 图标 | 代码                                                    |
| :--: | ------------------------------- | :--: | ------------------------------------------------------- |
|  👍  | `+1` <br /> `thumbsup`      |  👎  | `-1` <br /> `thumbsdown`                            |
|  ✊  | `fist` <br /> `fist_raised` |  👊  | `facepunch` <br /> `fist_oncoming` <br /> `punch` |
|  🤛  | `fist_left`                   |  🤜  | `fist_right`                                          |

### 两只手

| 图标 | 代码           | 图标 | 代码             |
| :--: | -------------- | :--: | ---------------- |
|  👏  | `clap`       |  🙌  | `raised_hands` |
|  👐  | `open_hands` |  🤝  | `handshake`    |
|  🙏  | `pray`       |      |                  |

### 握住东西的手势

| 图标 | 代码             | 图标 | 代码          |
| :--: | ---------------- | :--: | ------------- |
| ✍️ | `writing_hand` |  💅  | `nail_care` |
|  🤳  | `selfie`       |      |               |

### 身体部位

| 图标 | 代码       | 图标 | 代码       |
| :--: | ---------- | :--: | ---------- |
|  💪  | `muscle` |  👂  | `ear`    |
|  👃  | `nose`   |  👀  | `eyes`   |
|  👁  | `eye`    |  👅  | `tongue` |
|  👄  | `lips`   |      |            |

### 人

|  图标  | 代码             | 图标 | 代码                                             |
| :----: | ---------------- | :--: | ------------------------------------------------ |
|   👶   | `baby`         |  👦  | `boy`                                          |
|   👧   | `girl`         |  👱  | `blonde_man` <br /> `person_with_blond_hair` |
|   👨   | `man`          |  👩  | `woman`                                        |
| 👱‍♀ | `blonde_woman` |  👴  | `older_man`                                    |
|   👵   | `older_woman`  |      |                                                  |

### 身体动作

|  图标  | 代码                                                                             |  图标  | 代码                                      |
| :----: | -------------------------------------------------------------------------------- | :----: | ----------------------------------------- |
|   🙍   | `frowning_woman` <br /> `person_frowning`                                    | 🙍‍♂ | `frowning_man`                          |
|   🙎   | `person_with_pouting_face` <br /> `pouting_woman`                            | 🙎‍♂ | `pouting_man`                           |
|   🙅   | `ng_woman` <br /> `no_good` <br /> `no_good_woman`                         | 🙅‍♂ | `ng_man` <br /> `no_good_man`         |
|   🙆   | `ok_woman`                                                                     | 🙆‍♂ | `ok_man`                                |
|   💁   | `information_desk_person` <br /> `sassy_woman` <br /> `tipping_hand_woman` | 💁‍♂ | `sassy_man` <br /> `tipping_hand_man` |
|   🙋   | `raising_hand` <br /> `raising_hand_woman`                                   | 🙋‍♂ | `raising_hand_man`                      |
|   🙇   | `bow` <br /> `bowing_man`                                                    | 🙇‍♀ | `bowing_woman`                          |
| 🤦‍♂ | `man_facepalming`                                                              | 🤦‍♀ | `woman_facepalming`                     |
| 🤷‍♂ | `man_shrugging`                                                                | 🤷‍♀ | `woman_shrugging`                       |

### 人物角色

|  图标  | 代码                                                       |    图标    | 代码                          |
| :----: | ---------------------------------------------------------- | :--------: | ----------------------------- |
| 👨‍⚕ | `man_health_worker`                                      |   👩‍⚕   | `woman_health_worker`       |
| 👨‍🎓 | `man_student`                                            |   👩‍🎓   | `woman_student`             |
| 👨‍🏫 | `man_teacher`                                            |   👩‍🏫   | `woman_teacher`             |
| 👨‍⚖ | `man_judge`                                              |   👩‍⚖   | `woman_judge`               |
| 👨‍🌾 | `man_farmer`                                             |   👩‍🌾   | `woman_farmer`              |
| 👨‍🍳 | `man_cook`                                               |   👩‍🍳   | `woman_cook`                |
| 👨‍🔧 | `man_mechanic`                                           |   👩‍🔧   | `woman_mechanic`            |
| 👨‍🏭 | `man_factory_worker`                                     |   👩‍🏭   | `woman_factory_worker`      |
| 👨‍💼 | `man_office_worker`                                      |   👩‍💼   | `woman_office_worker`       |
| 👨‍🔬 | `man_scientist`                                          |   👩‍🔬   | `woman_scientist`           |
| 👨‍💻 | `man_technologist`                                       |   👩‍💻   | `woman_technologist`        |
| 👨‍🎤 | `man_singer`                                             |   👩‍🎤   | `woman_singer`              |
| 👨‍🎨 | `man_artist`                                             |   👩‍🎨   | `woman_artist`              |
| 👨‍✈ | `man_pilot`                                              |   👩‍✈   | `woman_pilot`               |
| 👨‍🚀 | `man_astronaut`                                          |   👩‍🚀   | `woman_astronaut`           |
| 👨‍🚒 | `man_firefighter`                                        |   👩‍🚒   | `woman_firefighter`         |
|   👮   | `cop` <br /> `policeman`                               |   👮‍♀   | `policewoman`               |
|   🕵   | `detective` <br /> `male_detective`                    | 🕵️‍♀️ | `female_detective`          |
|   💂   | `guardsman`                                              |   💂‍♀   | `guardswoman`               |
|   👷   | `construction_worker` <br /> `construction_worker_man` |   👷‍♀   | `construction_worker_woman` |
|   🤴   | `prince`                                                 |     👸     | `princess`                  |
|   👳   | `man_with_turban`                                        |   👳‍♀   | `woman_with_turban`         |
|   👲   | `man_with_gua_pi_mao`                                    |     🤵     | `man_in_tuxedo`             |
|   👰   | `bride_with_veil`                                        |     🤰     | `pregnant_woman`            |

### 幻想的人物

| 图标 | 代码          | 图标 | 代码      |
| :--: | ------------- | :--: | --------- |
|  👼  | `angel`     |  🎅  | `santa` |
|  🤶  | `mrs_claus` |      |           |

### 人物活动

|  图标  | 代码                                                 |  图标  | 代码                                 |
| :----: | ---------------------------------------------------- | :----: | ------------------------------------ |
|   💆   | `massage` <br /> `massage_woman`                 | 💆‍♂ | `massage_man`                      |
|   💇   | `haircut` <br /> `haircut_woman`                 | 💇‍♂ | `haircut_man`                      |
|   🚶   | `walking` <br /> `walking_man`                   | 🚶‍♀ | `walking_woman`                    |
|   🏃   | `runner` <br /> `running` <br /> `running_man` | 🏃‍♀ | `running_woman`                    |
|   💃   | `dancer`                                           |   🕺   | `man_dancing`                      |
|   🕴   | `business_suit_levitating`                         |   👯   | `dancers` <br /> `dancing_women` |
| 👯‍♂ | `dancing_men`                                      |        |                                      |

### 体育

|  图标  | 代码                                                  |    图标    | 代码                         |
| :----: | ----------------------------------------------------- | :--------: | ---------------------------- |
|   🤺   | `person_fencing`                                    |     🏇     | `horse_racing`             |
|   ⛷   | `skier`                                             |     🏂     | `snowboarder`              |
|   🏌   | `golfing_man`                                       | 🏌️‍♀️ | `golfing_woman`            |
|   🏄   | `surfer` <br /> `surfing_man`                     |   🏄‍♀   | `surfing_woman`            |
|   🚣   | `rowboat` <br /> `rowing_man`                     |   🚣‍♀   | `rowing_woman`             |
|   🏊   | `swimmer` <br /> `swimming_man`                   |   🏊‍♀   | `swimming_woman`           |
|   ⛹   | `basketball_man`                                    | ⛹️‍♀️ | `basketball_woman`         |
|   🏋   | `weight_lifting_man`                                | 🏋️‍♀️ | `weight_lifting_woman`     |
|   🚴   | `bicyclist` <br /> `biking_man`                   |   🚴‍♀   | `biking_woman`             |
|   🚵   | `mountain_bicyclist` <br /> `mountain_biking_man` |   🚵‍♀   | `mountain_biking_woman`    |
| 🤸‍♂ | `man_cartwheeling`                                  |   🤸‍♀   | `woman_cartwheeling`       |
| 🤼‍♂ | `men_wrestling`                                     |   🤼‍♀   | `women_wrestling`          |
| 🤽‍♂ | `man_playing_water_polo`                            |   🤽‍♀   | `woman_playing_water_polo` |
| 🤾‍♂ | `man_playing_handball`                              |   🤾‍♀   | `woman_playing_handball`   |
| 🤹‍♂ | `man_juggling`                                      |   🤹‍♀   | `woman_juggling`           |

### 休息

| 图标 | 代码     | 图标 | 代码             |
| :--: | -------- | :--: | ---------------- |
|  🛀  | `bath` |  🛌  | `sleeping_bed` |

### 家庭

|       图标       | 代码                                                         |       图标       | 代码                                       |
| :--------------: | ------------------------------------------------------------ | :--------------: | ------------------------------------------ |
|        👭        | `two_women_holding_hands`                                  |        👫        | `couple`                                 |
|        👬        | `two_men_holding_hands`                                    |        💏        | `couplekiss_man_woman`                   |
| 👨‍❤️‍💋‍👨 | `couplekiss_man_man`                                       | 👩‍❤️‍💋‍👩 | `couplekiss_woman_woman`                 |
|        💑        | `couple_with_heart` <br /> `couple_with_heart_woman_man` |   👨‍❤️‍👨   | `couple_with_heart_man_man`              |
|   👩‍❤️‍👩   | `couple_with_heart_woman_woman`                            |        👪        | `family` <br /> `family_man_woman_boy` |
|    👨‍👩‍👧    | `family_man_woman_girl`                                    |  👨‍👩‍👧‍👦  | `family_man_woman_girl_boy`              |
|  👨‍👩‍👦‍👦  | `family_man_woman_boy_boy`                                 |  👨‍👩‍👧‍👧  | `family_man_woman_girl_girl`             |
|    👨‍👨‍👦    | `family_man_man_boy`                                       |    👨‍👨‍👧    | `family_man_man_girl`                    |
|  👨‍👨‍👧‍👦  | `family_man_man_girl_boy`                                  |  👨‍👨‍👦‍👦  | `family_man_man_boy_boy`                 |
|  👨‍👨‍👧‍👧  | `family_man_man_girl_girl`                                 |    👩‍👩‍👦    | `family_woman_woman_boy`                 |
|    👩‍👩‍👧    | `family_woman_woman_girl`                                  |  👩‍👩‍👧‍👦  | `family_woman_woman_girl_boy`            |
|  👩‍👩‍👦‍👦  | `family_woman_woman_boy_boy`                               |  👩‍👩‍👧‍👧  | `family_woman_woman_girl_girl`           |
|      👨‍👦      | `family_man_boy`                                           |    👨‍👦‍👦    | `family_man_boy_boy`                     |
|      👨‍👧      | `family_man_girl`                                          |    👨‍👧‍👦    | `family_man_girl_boy`                    |
|    👨‍👧‍👧    | `family_man_girl_girl`                                     |      👩‍👦      | `family_woman_boy`                       |
|    👩‍👦‍👦    | `family_woman_boy_boy`                                     |      👩‍👧      | `family_woman_girl`                      |
|    👩‍👧‍👦    | `family_woman_girl_boy`                                    |    👩‍👧‍👧    | `family_woman_girl_girl`                 |

### 人物符号

| 图标 | 代码                    | 图标 | 代码                   |
| :--: | ----------------------- | :--: | ---------------------- |
|  🗣  | `speaking_head`       |  👤  | `bust_in_silhouette` |
|  👥  | `busts_in_silhouette` |  👣  | `footprints`         |

## 动物与自然

### 哺乳动物

| 图标 | 代码                           | 图标 | 代码                |
| :--: | ------------------------------ | :--: | ------------------- |
|  🐵  | `monkey_face`                |  🐒  | `monkey`          |
|  🦍  | `gorilla`                    |  🐶  | `dog`             |
|  🐕  | `dog2`                       |  🐩  | `poodle`          |
|  🐺  | `wolf`                       |  🦊  | `fox_face`        |
|  🐱  | `cat`                        |  🐈  | `cat2`            |
|  🦁  | `lion`                       |  🐯  | `tiger`           |
|  🐅  | `tiger2`                     |  🐆  | `leopard`         |
|  🐴  | `horse`                      |  🐎  | `racehorse`       |
|  🦄  | `unicorn`                    |  🦌  | `deer`            |
|  🐮  | `cow`                        |  🐂  | `ox`              |
|  🐃  | `water_buffalo`              |  🐄  | `cow2`            |
|  🐷  | `pig`                        |  🐖  | `pig2`            |
|  🐗  | `boar`                       |  🐽  | `pig_nose`        |
|  🐏  | `ram`                        |  🐑  | `sheep`           |
|  🐐  | `goat`                       |  🐪  | `dromedary_camel` |
|  🐫  | `camel`                      |  🐘  | `elephant`        |
|  🦏  | `rhinoceros`                 |  🐭  | `mouse`           |
|  🐁  | `mouse2`                     |  🐀  | `rat`             |
|  🐹  | `hamster`                    |  🐰  | `rabbit`          |
|  🐇  | `rabbit2`                    |  🐿  | `chipmunk`        |
|  🦇  | `bat`                        |  🐻  | `bear`            |
|  🐨  | `koala`                      |  🐼  | `panda_face`      |
|  🐾  | `feet` <br /> `paw_prints` |      |                     |

### 鸟类

| 图标 | 代码           | 图标 | 代码               |
| :--: | -------------- | :--: | ------------------ |
|  🦃  | `turkey`     |  🐔  | `chicken`        |
|  🐓  | `rooster`    |  🐣  | `hatching_chick` |
|  🐤  | `baby_chick` |  🐥  | `hatched_chick`  |
|  🐦  | `bird`       |  🐧  | `penguin`        |
|  🕊  | `dove`       |  🦅  | `eagle`          |
|  🦆  | `duck`       |  🦉  | `owl`            |

### 两栖动物

| icon | code     | icon | code |
| :--: | -------- | :--: | ---- |
|  🐸  | `frog` |      |      |

### 爬虫类

| 图标 | 代码            | 图标 | 代码       |
| :--: | --------------- | :--: | ---------- |
|  🐊  | `crocodile`   |  🐢  | `turtle` |
|  🦎  | `lizard`      |  🐍  | `snake`  |
|  🐲  | `dragon_face` |  🐉  | `dragon` |

### 海洋动物

| 图标 | 代码                           | 图标 | 代码         |
| :--: | ------------------------------ | :--: | ------------ |
|  🐳  | `whale`                      |  🐋  | `whale2`   |
|  🐬  | `dolphin` <br /> `flipper` |  🐟  | `fish`     |
|  🐠  | `tropical_fish`              |  🐡  | `blowfish` |
|  🦈  | `shark`                      |  🐙  | `octopus`  |
|  🐚  | `shell`                      |      |              |

### 虫类

| 图标 | 代码                        | 图标 | 代码           |
| :--: | --------------------------- | :--: | -------------- |
|  🐌  | `snail`                   |  🦋  | `butterfly`  |
|  🐛  | `bug`                     |  🐜  | `ant`        |
|  🐝  | `bee` <br /> `honeybee` |  🐞  | `beetle`     |
|  🕷  | `spider`                  |  🕸  | `spider_web` |
|  🦂  | `scorpion`                |      |                |

### 花类植物

| 图标 | 代码             | 图标 | 代码               |
| :--: | ---------------- | :--: | ------------------ |
|  💐  | `bouquet`      |  🌸  | `cherry_blossom` |
|  💮  | `white_flower` |  🏵  | `rosette`        |
|  🌹  | `rose`         |  🥀  | `wilted_flower`  |
|  🌺  | `hibiscus`     |  🌻  | `sunflower`      |
|  🌼  | `blossom`      |  🌷  | `tulip`          |

### 其它植物

| 图标 | 代码                 | 图标 | 代码               |
| :--: | -------------------- | :--: | ------------------ |
|  🌱  | `seedling`         |  🌲  | `evergreen_tree` |
|  🌳  | `deciduous_tree`   |  🌴  | `palm_tree`      |
|  🌵  | `cactus`           |  🌾  | `ear_of_rice`    |
|  🌿  | `herb`             | ☘️ | `shamrock`       |
|  🍀  | `four_leaf_clover` |  🍁  | `maple_leaf`     |
|  🍂  | `fallen_leaf`      |  🍃  | `leaves`         |

## 食物与饮料

### 水果

| 图标 | 代码            | 图标 | 代码                                                |
| :--: | --------------- | :--: | --------------------------------------------------- |
|  🍇  | `grapes`      |  🍈  | `melon`                                           |
|  🍉  | `watermelon`  |  🍊  | `mandarin` <br /> `orange` <br /> `tangerine` |
|  🍋  | `lemon`       |  🍌  | `banana`                                          |
|  🍍  | `pineapple`   |  🍎  | `apple`                                           |
|  🍏  | `green_apple` |  🍐  | `pear`                                            |
|  🍑  | `peach`       |  🍒  | `cherries`                                        |
|  🍓  | `strawberry`  |  🥝  | `kiwi_fruit`                                      |
|  🍅  | `tomato`      |      |                                                     |

### 蔬菜

| 图标 | 代码         | 图标 | 代码           |
| :--: | ------------ | :--: | -------------- |
|  🥑  | `avocado`  |  🍆  | `eggplant`   |
|  🥔  | `potato`   |  🥕  | `carrot`     |
|  🌽  | `corn`     |  🌶  | `hot_pepper` |
|  🥒  | `cucumber` |  🍄  | `mushroom`   |
|  🥜  | `peanuts`  |  🌰  | `chestnut`   |

### 快餐

| 图标 | 代码                  | 图标 | 代码                    |
| :--: | --------------------- | :--: | ----------------------- |
|  🍞  | `bread`             |  🥐  | `croissant`           |
|  🥖  | `baguette_bread`    |  🥞  | `pancakes`            |
|  🧀  | `cheese`            |  🍖  | `meat_on_bone`        |
|  🍗  | `poultry_leg`       |  🥓  | `bacon`               |
|  🍔  | `hamburger`         |  🍟  | `fries`               |
|  🍕  | `pizza`             |  🌭  | `hotdog`              |
|  🌮  | `taco`              |  🌯  | `burrito`             |
|  🥙  | `stuffed_flatbread` |  🥚  | `egg`                 |
|  🍳  | `fried_egg`         |  🥘  | `shallow_pan_of_food` |
|  🍲  | `stew`              |  🥗  | `green_salad`         |
|  🍿  | `popcorn`           |      |                         |

### 亚洲食物

| 图标 | 代码             | 图标 | 代码             |
| :--: | ---------------- | :--: | ---------------- |
|  🍱  | `bento`        |  🍘  | `rice_cracker` |
|  🍙  | `rice_ball`    |  🍚  | `rice`         |
|  🍛  | `curry`        |  🍜  | `ramen`        |
|  🍝  | `spaghetti`    |  🍠  | `sweet_potato` |
|  🍢  | `oden`         |  🍣  | `sushi`        |
|  🍤  | `fried_shrimp` |  🍥  | `fish_cake`    |
|  🍡  | `dango`        |      |                  |

### 海鲜

| 图标 | 代码      | 图标 | 代码       |
| :--: | --------- | :--: | ---------- |
|  🦀  | `crab`  |  🦐  | `shrimp` |
|  🦑  | `squid` |      |            |

### 甜点

| 图标 | 代码          | 图标 | 代码              |
| :--: | ------------- | :--: | ----------------- |
|  🍦  | `icecream`  |  🍧  | `shaved_ice`    |
|  🍨  | `ice_cream` |  🍩  | `doughnut`      |
|  🍪  | `cookie`    |  🎂  | `birthday`      |
|  🍰  | `cake`      |  🍫  | `chocolate_bar` |
|  🍬  | `candy`     |  🍭  | `lollipop`      |
|  🍮  | `custard`   |  🍯  | `honey_pot`     |

### 饮料

| 图标 | 代码               | 图标 | 代码                 |
| :--: | ------------------ | :--: | -------------------- |
|  🍼  | `baby_bottle`    |  🥛  | `milk_glass`       |
| ☕️ | `coffee`         |  🍵  | `tea`              |
|  🍶  | `sake`           |  🍾  | `champagne`        |
|  🍷  | `wine_glass`     |  🍸  | `cocktail`         |
|  🍹  | `tropical_drink` |  🍺  | `beer`             |
|  🍻  | `beers`          |  🥂  | `clinking_glasses` |
|  🥃  | `tumbler_glass`  |      |                      |

### 餐具

| 图标 | 代码                   | 图标 | 代码                       |
| :--: | ---------------------- | :--: | -------------------------- |
|  🍽  | `plate_with_cutlery` |  🍴  | `fork_and_knife`         |
|  🥄  | `spoon`              |  🔪  | `hocho` <br /> `knife` |
|  🏺  | `amphora`            |      |                            |

## 旅游与地理

### 地图

| 图标 | 代码             | 图标 | 代码                     |
| :--: | ---------------- | :--: | ------------------------ |
|  🌍  | `earth_africa` |  🌎  | `earth_americas`       |
|  🌏  | `earth_asia`   |  🌐  | `globe_with_meridians` |
|  🗺  | `world_map`    |  🗾  | `japan`                |

### 地理现象

| 图标 | 代码              | 图标 | 代码               |
| :--: | ----------------- | :--: | ------------------ |
|  🏔  | `mountain_snow` |  ⛰  | `mountain`       |
|  🌋  | `volcano`       |  🗻  | `mount_fuji`     |
|  🏕  | `camping`       |  🏖  | `beach_umbrella` |
|  🏜  | `desert`        |  🏝  | `desert_island`  |
|  🏞  | `national_park` |      |                    |

### 建筑物

| 图标 | 代码                      | 图标 | 代码                     |
| :--: | ------------------------- | :--: | ------------------------ |
|  🏟  | `stadium`               |  🏛  | `classical_building`   |
|  🏗  | `building_construction` |  🏘  | `houses`               |
|  🏚  | `derelict_house`        |  🏠  | `house`                |
|  🏡  | `house_with_garden`     |  🏢  | `office`               |
|  🏣  | `post_office`           |  🏤  | `european_post_office` |
|  🏥  | `hospital`              |  🏦  | `bank`                 |
|  🏨  | `hotel`                 |  🏩  | `love_hotel`           |
|  🏪  | `convenience_store`     |  🏫  | `school`               |
|  🏬  | `department_store`      |  🏭  | `factory`              |
|  🏯  | `japanese_castle`       |  🏰  | `european_castle`      |
|  💒  | `wedding`               |  🗼  | `tokyo_tower`          |
|  🗽  | `statue_of_liberty`     |      |                          |

### 宗教建筑

| 图标 | 代码          | 图标 | 代码              |
| :--: | ------------- | :--: | ----------------- |
| ⛪️ | `church`    |  🕌  | `mosque`        |
|  🕍  | `synagogue` |  ⛩  | `shinto_shrine` |
|  🕋  | `kaaba`     |      |                   |

### 其它地点

| 图标 | 代码             | 图标 | 代码                       |
| :--: | ---------------- | :--: | -------------------------- |
| ⛲️ | `fountain`     | ⛺️ | `tent`                   |
|  🌁  | `foggy`        |  🌃  | `night_with_stars`       |
|  🏙  | `cityscape`    |  🌄  | `sunrise_over_mountains` |
|  🌅  | `sunrise`      |  🌆  | `city_sunset`            |
|  🌇  | `city_sunrise` |  🌉  | `bridge_at_night`        |
| ♨️ | `hotsprings`   |  🎠  | `carousel_horse`         |
|  🎡  | `ferris_wheel` |  🎢  | `roller_coaster`         |
|  💈  | `barber`       |  🎪  | `circus_tent`            |

### 陆路运输

| 图标 | 代码                       | 图标 | 代码                    |
| :--: | -------------------------- | :--: | ----------------------- |
|  🚂  | `steam_locomotive`       |  🚃  | `railway_car`         |
|  🚄  | `bullettrain_side`       |  🚅  | `bullettrain_front`   |
|  🚆  | `train2`                 |  🚇  | `metro`               |
|  🚈  | `light_rail`             |  🚉  | `station`             |
|  🚊  | `tram`                   |  🚝  | `monorail`            |
|  🚞  | `mountain_railway`       |  🚋  | `train`               |
|  🚌  | `bus`                    |  🚍  | `oncoming_bus`        |
|  🚎  | `trolleybus`             |  🚐  | `minibus`             |
|  🚑  | `ambulance`              |  🚒  | `fire_engine`         |
|  🚓  | `police_car`             |  🚔  | `oncoming_police_car` |
|  🚕  | `taxi`                   |  🚖  | `oncoming_taxi`       |
|  🚗  | `car` <br /> `red_car` |  🚘  | `oncoming_automobile` |
|  🚙  | `blue_car`               |  🚚  | `truck`               |
|  🚛  | `articulated_lorry`      |  🚜  | `tractor`             |
|  🏎  | `racing_car`             |  🏍  | `motorcycle`          |
|  🛵  | `motor_scooter`          |  🚲  | `bike`                |
|  🛴  | `kick_scooter`           |  🚏  | `busstop`             |
|  🛣  | `motorway`               |  🛤  | `railway_track`       |
|  🛢  | `oil_drum`               | ⛽️ | `fuelpump`            |
|  🚨  | `rotating_light`         |  🚥  | `traffic_light`       |
|  🚦  | `vertical_traffic_light` |  🛑  | `stop_sign`           |
|  🚧  | `construction`           |      |                         |

### 水路运输

| 图标 | 代码               | 图标 | 代码                         |
| :--: | ------------------ | :--: | ---------------------------- |
| ⚓️ | `anchor`         | ⛵️ | `boat` <br /> `sailboat` |
|  🛶  | `canoe`          |  🚤  | `speedboat`                |
|  🛳  | `passenger_ship` |  ⛴  | `ferry`                    |
|  🛥  | `motor_boat`     |  🚢  | `ship`                     |

### 空中运输

| 图标 | 代码                   | 图标 | 代码                     |
| :--: | ---------------------- | :--: | ------------------------ |
| ✈️ | `airplane`           |  🛩  | `small_airplane`       |
|  🛫  | `flight_departure`   |  🛬  | `flight_arrival`       |
|  💺  | `seat`               |  🚁  | `helicopter`           |
|  🚟  | `suspension_railway` |  🚠  | `mountain_cableway`    |
|  🚡  | `aerial_tramway`     |  🛰  | `artificial_satellite` |
|  🚀  | `rocket`             |      |                          |

### 旅馆

| icon | code             | icon | code |
| :--: | ---------------- | :--: | ---- |
|  🛎  | `bellhop_bell` |      |      |

### 时间

| 图标 | 代码                  | 图标 | 代码                       |
| :--: | --------------------- | :--: | -------------------------- |
| ⌛️ | `hourglass`         |  ⏳  | `hourglass_flowing_sand` |
| ⌚️ | `watch`             |  ⏰  | `alarm_clock`            |
|  ⏱  | `stopwatch`         |  ⏲  | `timer_clock`            |
|  🕰  | `mantelpiece_clock` |  🕛  | `clock12`                |
|  🕧  | `clock1230`         |  🕐  | `clock1`                 |
|  🕜  | `clock130`          |  🕑  | `clock2`                 |
|  🕝  | `clock230`          |  🕒  | `clock3`                 |
|  🕞  | `clock330`          |  🕓  | `clock4`                 |
|  🕟  | `clock430`          |  🕔  | `clock5`                 |
|  🕠  | `clock530`          |  🕕  | `clock6`                 |
|  🕡  | `clock630`          |  🕖  | `clock7`                 |
|  🕢  | `clock730`          |  🕗  | `clock8`                 |
|  🕣  | `clock830`          |  🕘  | `clock9`                 |
|  🕤  | `clock930`          |  🕙  | `clock10`                |
|  🕥  | `clock1030`         |  🕚  | `clock11`                |
|  🕦  | `clock1130`         |      |                            |

### 天空与天气

| 图标 | 代码                              | 图标 | 代码                                    |
| :--: | --------------------------------- | :--: | --------------------------------------- |
|  🌑  | `new_moon`                      |  🌒  | `waxing_crescent_moon`                |
|  🌓  | `first_quarter_moon`            |  🌔  | `moon` <br /> `waxing_gibbous_moon` |
|  🌕  | `full_moon`                     |  🌖  | `waning_gibbous_moon`                 |
|  🌗  | `last_quarter_moon`             |  🌘  | `waning_crescent_moon`                |
|  🌙  | `crescent_moon`                 |  🌚  | `new_moon_with_face`                  |
|  🌛  | `first_quarter_moon_with_face`  |  🌜  | `last_quarter_moon_with_face`         |
|  🌡  | `thermometer`                   | ☀️ | `sunny`                               |
|  🌝  | `full_moon_with_face`           |  🌞  | `sun_with_face`                       |
| ⭐️ | `star`                          |  🌟  | `star2`                               |
|  🌠  | `stars`                         |  🌌  | `milky_way`                           |
| ☁️ | `cloud`                         | ⛅️ | `partly_sunny`                        |
|  ⛈  | `cloud_with_lightning_and_rain` |  🌤  | `sun_behind_small_cloud`              |
|  🌥  | `sun_behind_large_cloud`        |  🌦  | `sun_behind_rain_cloud`               |
|  🌧  | `cloud_with_rain`               |  🌨  | `cloud_with_snow`                     |
|  🌩  | `cloud_with_lightning`          |  🌪  | `tornado`                             |
|  🌫  | `fog`                           |  🌬  | `wind_face`                           |
|  🌀  | `cyclone`                       |  🌈  | `rainbow`                             |
|  🌂  | `closed_umbrella`               | ☂️ | `open_umbrella`                       |
| ☔️ | `umbrella`                      |  ⛱  | `parasol_on_ground`                   |
| ⚡️ | `zap`                           | ❄️ | `snowflake`                           |
| ☃️ | `snowman_with_snow`             | ⛄️ | `snowman`                             |
|  ☄  | `comet`                         |  🔥  | `fire`                                |
|  💧  | `droplet`                       |  🌊  | `ocean`                               |

## 活动

### 事件

| 图标 | 代码                | 图标 | 代码               |
| :--: | ------------------- | :--: | ------------------ |
|  🎃  | `jack_o_lantern`  |  🎄  | `christmas_tree` |
|  🎆  | `fireworks`       |  🎇  | `sparkler`       |
|  ✨  | `sparkles`        |  🎈  | `balloon`        |
|  🎉  | `tada`            |  🎊  | `confetti_ball`  |
|  🎋  | `tanabata_tree`   |  🎍  | `bamboo`         |
|  🎎  | `dolls`           |  🎏  | `flags`          |
|  🎐  | `wind_chime`      |  🎑  | `rice_scene`     |
|  🎀  | `ribbon`          |  🎁  | `gift`           |
|  🎗  | `reminder_ribbon` |  🎟  | `tickets`        |
|  🎫  | `ticket`          |      |                    |

### 奖杯与奖牌

| 图标 | 代码                | 图标 | 代码                |
| :--: | ------------------- | :--: | ------------------- |
|  🎖  | `medal_military`  |  🏆  | `trophy`          |
|  🏅  | `medal_sports`    |  🥇  | `1st_place_medal` |
|  🥈  | `2nd_place_medal` |  🥉  | `3rd_place_medal` |

### 体育运动

| 图标 | 代码                      | 图标 | 代码                        |
| :--: | ------------------------- | :--: | --------------------------- |
| ⚽️ | `soccer`                | ⚾️ | `baseball`                |
|  🏀  | `basketball`            |  🏐  | `volleyball`              |
|  🏈  | `football`              |  🏉  | `rugby_football`          |
|  🎾  | `tennis`                |  🎳  | `bowling`                 |
|  🏏  | `cricket`               |  🏑  | `field_hockey`            |
|  🏒  | `ice_hockey`            |  🏓  | `ping_pong`               |
|  🏸  | `badminton`             |  🥊  | `boxing_glove`            |
|  🥋  | `martial_arts_uniform`  |  🥅  | `goal_net`                |
| ⛳️ | `golf`                  |  ⛸  | `ice_skate`               |
|  🎣  | `fishing_pole_and_fish` |  🎽  | `running_shirt_with_sash` |
|  🎿  | `ski`                   |      |                             |

### 游戏

| 图标 | 代码             | 图标 | 代码                     |
| :--: | ---------------- | :--: | ------------------------ |
|  🎯  | `dart`         |  🎱  | `8ball`                |
|  🔮  | `crystal_ball` |  🎮  | `video_game`           |
|  🕹  | `joystick`     |  🎰  | `slot_machine`         |
|  🎲  | `game_die`     | ♠️ | `spades`               |
| ♥️ | `hearts`       | ♦️ | `diamonds`             |
| ♣️ | `clubs`        |  🃏  | `black_joker`          |
| 🀄️ | `mahjong`      |  🎴  | `flower_playing_cards` |

### 艺术与工艺

| 图标 | 代码                | 图标 | 代码               |
| :--: | ------------------- | :--: | ------------------ |
|  🎭  | `performing_arts` |  🖼  | `framed_picture` |
|  🎨  | `art`             |      |                    |

## 物品

### 服装

| 图标 | 代码                          | 图标 | 代码                        |
| :--: | ----------------------------- | :--: | --------------------------- |
|  👓  | `eyeglasses`                |  🕶  | `dark_sunglasses`         |
|  👔  | `necktie`                   |  👕  | `shirt` <br /> `tshirt` |
|  👖  | `jeans`                     |  👗  | `dress`                   |
|  👘  | `kimono`                    |  👙  | `bikini`                  |
|  👚  | `womans_clothes`            |  👛  | `purse`                   |
|  👜  | `handbag`                   |  👝  | `pouch`                   |
|  🛍  | `shopping`                  |  🎒  | `school_satchel`          |
|  👞  | `mans_shoe` <br /> `shoe` |  👟  | `athletic_shoe`           |
|  👠  | `high_heel`                 |  👡  | `sandal`                  |
|  👢  | `boot`                      |  👑  | `crown`                   |
|  👒  | `womans_hat`                |  🎩  | `tophat`                  |
|  🎓  | `mortar_board`              |  ⛑  | `rescue_worker_helmet`    |
|  📿  | `prayer_beads`              |  💄  | `lipstick`                |
|  💍  | `ring`                      |  💎  | `gem`                     |

### 声音

| 图标 | 代码            | 图标 | 代码           |
| :--: | --------------- | :--: | -------------- |
|  🔇  | `mute`        |  🔈  | `speaker`    |
|  🔉  | `sound`       |  🔊  | `loud_sound` |
|  📢  | `loudspeaker` |  📣  | `mega`       |
|  📯  | `postal_horn` |  🔔  | `bell`       |
|  🔕  | `no_bell`     |      |                |

### 音乐

| 图标 | 代码              | 图标 | 代码                  |
| :--: | ----------------- | :--: | --------------------- |
|  🎼  | `musical_score` |  🎵  | `musical_note`      |
|  🎶  | `notes`         |  🎙  | `studio_microphone` |
|  🎚  | `level_slider`  |  🎛  | `control_knobs`     |
|  🎤  | `microphone`    |  🎧  | `headphones`        |
|  📻  | `radio`         |      |                       |

### 乐器

| 图标 | 代码                 | 图标 | 代码        |
| :--: | -------------------- | :--: | ----------- |
|  🎷  | `saxophone`        |  🎸  | `guitar`  |
|  🎹  | `musical_keyboard` |  🎺  | `trumpet` |
|  🎻  | `violin`           |  🥁  | `drum`    |

### 电话

| 图标 | 代码                           | 图标 | 代码                   |
| :--: | ------------------------------ | :--: | ---------------------- |
|  📱  | `iphone`                     |  📲  | `calling`            |
| ☎️ | `phone` <br /> `telephone` |  📞  | `telephone_receiver` |
|  📟  | `pager`                      |  📠  | `fax`                |

### 电脑

| 图标 | 代码               | 图标 | 代码                 |
| :--: | ------------------ | :--: | -------------------- |
|  🔋  | `battery`        |  🔌  | `electric_plug`    |
|  💻  | `computer`       |  🖥  | `desktop_computer` |
|  🖨  | `printer`        | ⌨️ | `keyboard`         |
|  🖱  | `computer_mouse` |  🖲  | `trackball`        |
|  💽  | `minidisc`       |  💾  | `floppy_disk`      |
|  💿  | `cd`             |  📀  | `dvd`              |

### 灯光与影像

| 图标 | 代码                                   | 图标 | 代码             |
| :--: | -------------------------------------- | :--: | ---------------- |
|  🎥  | `movie_camera`                       |  🎞  | `film_strip`   |
|  📽  | `film_projector`                     |  🎬  | `clapper`      |
|  📺  | `tv`                                 |  📷  | `camera`       |
|  📸  | `camera_flash`                       |  📹  | `video_camera` |
|  📼  | `vhs`                                |  🔍  | `mag`          |
|  🔎  | `mag_right`                          |  🕯  | `candle`       |
|  💡  | `bulb`                               |  🔦  | `flashlight`   |
|  🏮  | `izakaya_lantern` <br /> `lantern` |      |                  |

### 书与纸张

| 图标 | 代码                               | 图标 | 代码               |
| :--: | ---------------------------------- | :--: | ------------------ |
|  📔  | `notebook_with_decorative_cover` |  📕  | `closed_book`    |
|  📖  | `book` <br /> `open_book`      |  📗  | `green_book`     |
|  📘  | `blue_book`                      |  📙  | `orange_book`    |
|  📚  | `books`                          |  📓  | `notebook`       |
|  📒  | `ledger`                         |  📃  | `page_with_curl` |
|  📜  | `scroll`                         |  📄  | `page_facing_up` |
|  📰  | `newspaper`                      |  🗞  | `newspaper_roll` |
|  📑  | `bookmark_tabs`                  |  🔖  | `bookmark`       |
|  🏷  | `label`                          |      |                    |

### 钱

| 图标 | 代码            | 图标 | 代码                 |
| :--: | --------------- | :--: | -------------------- |
|  💰  | `moneybag`    |  💴  | `yen`              |
|  💵  | `dollar`      |  💶  | `euro`             |
|  💷  | `pound`       |  💸  | `money_with_wings` |
|  💳  | `credit_card` |  💹  | `chart`            |

### 邮件

| 图标 | 代码                          | 图标 | 代码                    |
| :--: | ----------------------------- | :--: | ----------------------- |
| ✉️ | `email` <br /> `envelope` |  📧  | `:e-mail:`            |
|  📨  | `incoming_envelope`         |  📩  | `envelope_with_arrow` |
|  📤  | `outbox_tray`               |  📥  | `inbox_tray`          |
|  📦  | `package`                   |  📫  | `mailbox`             |
|  📪  | `mailbox_closed`            |  📬  | `mailbox_with_mail`   |
|  📭  | `mailbox_with_no_mail`      |  📮  | `postbox`             |
|  🗳  | `ballot_box`                |      |                         |

### 书写

| 图标 | 代码                       | 图标 | 代码          |
| :--: | -------------------------- | :--: | ------------- |
| ✏️ | `pencil2`                | ✒️ | `black_nib` |
|  🖋  | `fountain_pen`           |  🖊  | `pen`       |
|  🖌  | `paintbrush`             |  🖍  | `crayon`    |
|  📝  | `memo` <br /> `pencil` |      |               |

### 办公

| 图标 | 代码                           | 图标 | 代码                         |
| :--: | ------------------------------ | :--: | ---------------------------- |
|  💼  | `briefcase`                  |  📁  | `file_folder`              |
|  📂  | `open_file_folder`           |  🗂  | `card_index_dividers`      |
|  📅  | `date`                       |  📆  | `calendar`                 |
|  🗒  | `spiral_notepad`             |  🗓  | `spiral_calendar`          |
|  📇  | `card_index`                 |  📈  | `chart_with_upwards_trend` |
|  📉  | `chart_with_downwards_trend` |  📊  | `bar_chart`                |
|  📋  | `clipboard`                  |  📌  | `pushpin`                  |
|  📍  | `round_pushpin`              |  📎  | `paperclip`                |
|  🖇  | `paperclips`                 |  📏  | `straight_ruler`           |
|  📐  | `triangular_ruler`           | ✂️ | `scissors`                 |
|  🗃  | `card_file_box`              |  🗄  | `file_cabinet`             |
|  🗑  | `wastebasket`                |      |                              |

### 锁

| 图标 | 代码                  | 图标 | 代码                     |
| :--: | --------------------- | :--: | ------------------------ |
|  🔒  | `lock`              |  🔓  | `unlock`               |
|  🔏  | `lock_with_ink_pen` |  🔐  | `closed_lock_with_key` |
|  🔑  | `key`               |  🗝  | `old_key`              |

### 工具

| 图标 | 代码                | 图标 | 代码                  |
| :--: | ------------------- | :--: | --------------------- |
|  🔨  | `hammer`          |  ⛏  | `pick`              |
|  ⚒  | `hammer_and_pick` |  🛠  | `hammer_and_wrench` |
|  🗡  | `dagger`          | ⚔️ | `crossed_swords`    |
|  🔫  | `gun`             |  🏹  | `bow_and_arrow`     |
|  🛡  | `shield`          |  🔧  | `wrench`            |
|  🔩  | `nut_and_bolt`    | ⚙️ | `gear`              |
|  🗜  | `clamp`           | ⚖️ | `balance_scale`     |
|  🔗  | `link`            |  ⛓  | `chains`            |

### 科学

| 图标 | 代码          | 图标 | 代码           |
| :--: | ------------- | :--: | -------------- |
| ⚗️ | `alembic`   |  🔬  | `microscope` |
|  🔭  | `telescope` |  📡  | `satellite`  |

### 医疗

| 图标 | 代码        | 图标 | 代码     |
| :--: | ----------- | :--: | -------- |
|  💉  | `syringe` |  💊  | `pill` |

### 生活用品

| 图标 | 代码               | 图标 | 代码        |
| :--: | ------------------ | :--: | ----------- |
|  🚪  | `door`           |  🛏  | `bed`     |
|  🛋  | `couch_and_lamp` |  🚽  | `toilet`  |
|  🚿  | `shower`         |  🛁  | `bathtub` |
|  🛒  | `shopping_cart`  |      |             |

### 其它物品

| 图标 | 代码            | 图标 | 代码       |
| :--: | --------------- | :--: | ---------- |
|  🚬  | `smoking`     | ⚰️ | `coffin` |
| ⚱️ | `funeral_urn` |  🗿  | `moyai`  |

## 符号

### 交通标识

| 图标 | 代码              | 图标 | 代码                        |
| :--: | ----------------- | :--: | --------------------------- |
|  🏧  | `atm`           |  🚮  | `put_litter_in_its_place` |
|  🚰  | `potable_water` | ♿️ | `wheelchair`              |
|  🚹  | `mens`          |  🚺  | `womens`                  |
|  🚻  | `restroom`      |  🚼  | `baby_symbol`             |
|  🚾  | `wc`            |  🛂  | `passport_control`        |
|  🛃  | `customs`       |  🛄  | `baggage_claim`           |
|  🛅  | `left_luggage`  |      |                             |

### 警告

| 图标 | 代码               | 图标 | 代码                    |
| :--: | ------------------ | :--: | ----------------------- |
| ⚠️ | `warning`        |  🚸  | `children_crossing`   |
| ⛔️ | `no_entry`       |  🚫  | `no_entry_sign`       |
|  🚳  | `no_bicycles`    |  🚭  | `no_smoking`          |
|  🚯  | `do_not_litter`  |  🚱  | `:non-potable_water:` |
|  🚷  | `no_pedestrians` |  📵  | `no_mobile_phones`    |
|  🔞  | `underage`       | ☢️ | `radioactive`         |
| ☣️ | `biohazard`      |      |                         |

### 箭头

| 图标 | 代码                          | 图标 | 代码                        |
| :--: | ----------------------------- | :--: | --------------------------- |
| ⬆️ | `arrow_up`                  | ↗️ | `arrow_upper_right`       |
| ➡️ | `arrow_right`               | ↘️ | `arrow_lower_right`       |
| ⬇️ | `arrow_down`                | ↙️ | `arrow_lower_left`        |
| ⬅️ | `arrow_left`                | ↖️ | `arrow_upper_left`        |
| ↕️ | `arrow_up_down`             | ↔️ | `left_right_arrow`        |
| ↩️ | `leftwards_arrow_with_hook` | ↪️ | `arrow_right_hook`        |
| ⤴️ | `arrow_heading_up`          | ⤵️ | `arrow_heading_down`      |
|  🔃  | `arrows_clockwise`          |  🔄  | `arrows_counterclockwise` |
|  🔙  | `back`                      |  🔚  | `end`                     |
|  🔛  | `on`                        |  🔜  | `soon`                    |
|  🔝  | `top`                       |      |                             |

### 宗教

| 图标 | 代码                  | 图标 | 代码                 |
| :--: | --------------------- | :--: | -------------------- |
|  🛐  | `place_of_worship`  | ⚛️ | `atom_symbol`      |
|  🕉  | `om`                | ✡️ | `star_of_david`    |
| ☸️ | `wheel_of_dharma`   | ☯️ | `yin_yang`         |
| ✝️ | `latin_cross`       | ☦️ | `orthodox_cross`   |
| ☪️ | `star_and_crescent` | ☮️ | `peace_symbol`     |
|  🕎  | `menorah`           |  🔯  | `six_pointed_star` |

### 生肖

| 图标 | 代码            | 图标 | 代码          |
| :--: | --------------- | :--: | ------------- |
| ♈️ | `aries`       | ♉️ | `taurus`    |
| ♊️ | `gemini`      | ♋️ | `cancer`    |
| ♌️ | `leo`         | ♍️ | `virgo`     |
| ♎️ | `libra`       | ♏️ | `scorpius`  |
| ♐️ | `sagittarius` | ♑️ | `capricorn` |
| ♒️ | `aquarius`    | ♓️ | `pisces`    |
|  ⛎  | `ophiuchus`   |      |               |

### 影像符号

| 图标 | 代码                          | 图标 | 代码                      |
| :--: | ----------------------------- | :--: | ------------------------- |
|  🔀  | `twisted_rightwards_arrows` |  🔁  | `repeat`                |
|  🔂  | `repeat_one`                | ▶️ | `arrow_forward`         |
|  ⏩  | `fast_forward`              |  ⏭  | `next_track_button`     |
|  ⏯  | `play_or_pause_button`      | ◀️ | `arrow_backward`        |
|  ⏪  | `rewind`                    |  ⏮  | `previous_track_button` |
|  🔼  | `arrow_up_small`            |  ⏫  | `arrow_double_up`       |
|  🔽  | `arrow_down_small`          |  ⏬  | `arrow_double_down`     |
|  ⏸  | `pause_button`              |  ⏹  | `stop_button`           |
|  ⏺  | `record_button`             |  🎦  | `cinema`                |
|  🔅  | `low_brightness`            |  🔆  | `high_brightness`       |
|  📶  | `signal_strength`           |  📳  | `vibration_mode`        |
|  📴  | `mobile_phone_off`          |      |                           |

### 数学

| 图标 | 代码                       | 图标 | 代码                    |
| :--: | -------------------------- | :--: | ----------------------- |
| ✖️ | `heavy_multiplication_x` |  ➕  | `heavy_plus_sign`     |
|  ➖  | `heavy_minus_sign`       |  ➗  | `heavy_division_sign` |

### 标点符号

| 图标 | 代码                 | 图标 | 代码                                              |
| :--: | -------------------- | :--: | ------------------------------------------------- |
| ‼️ | `bangbang`         | ⁉️ | `interrobang`                                   |
|  ❓  | `question`         |  ❔  | `grey_question`                                 |
|  ❕  | `grey_exclamation` | ❗️ | `exclamation` <br /> `heavy_exclamation_mark` |
| 〰️ | `wavy_dash`        |      |                                                   |

### 货币

| 图标 | 代码                  | 图标 | 代码                  |
| :--: | --------------------- | :--: | --------------------- |
|  💱  | `currency_exchange` |  💲  | `heavy_dollar_sign` |

### 按键符号

| 图标 | 代码           | 图标 | 代码         |
| :---: | -------------- | :---: | ------------ |
| #️⃣ | `hash`       | *️⃣ | `asterisk` |
| 0️⃣ | `zero`       | 1️⃣ | `one`      |
| 2️⃣ | `two`        | 3️⃣ | `three`    |
| 4️⃣ | `four`       | 5️⃣ | `five`     |
| 6️⃣ | `six`        | 7️⃣ | `seven`    |
| 8️⃣ | `eight`      | 9️⃣ | `nine`     |
|  🔟  | `keycap_ten` |      |              |

### 字母符号

| 图标 | 代码             |   图标   | 代码                    |
| :--: | ---------------- | :------: | ----------------------- |
|  🔠  | `capital_abcd` |    🔡    | `abcd`                |
|  🔢  | `1234`         |    🔣    | `symbols`             |
|  🔤  | `abc`          |   🅰️   | `a`                   |
|  🆎  | `ab`           |   🅱️   | `b`                   |
|  🆑  | `cl`           |    🆒    | `cool`                |
|  🆓  | `free`         |   ℹ️   | `information_source`  |
|  🆔  | `id`           |   Ⓜ️   | `m`                   |
|  🆕  | `new`          |    🆖    | `ng`                  |
| 🅾️ | `o2`           |    🆗    | `ok`                  |
| 🅿️ | `parking`      |    🆘    | `sos`                 |
|  🆙  | `up`           |    🆚    | `vs`                  |
|  🈁  | `koko`         |   🈂️   | `sa`                  |
| 🈷️ | `u6708`        |    🈶    | `u6709`               |
| 🈯️ | `u6307`        |    🉐    | `ideograph_advantage` |
|  🈹  | `u5272`        |   🈚️   | `u7121`               |
|  🈲  | `u7981`        | :accept: | `accept`              |
|  🈸  | `u7533`        |    🈴    | `u5408`               |
|  🈳  | `u7a7a`        |   ㊗️   | `congratulations`     |
| ㊙️ | `secret`       |    🈺    | `u55b6`               |
|  🈵  | `u6e80`        |          |                         |

### 几何符号

| 图标 | 代码                                | 图标 | 代码                          |
| :--: | ----------------------------------- | :--: | ----------------------------- |
|  🔴  | `red_circle`                      |  🔵  | `large_blue_circle`         |
| ⚫️ | `black_circle`                    | ⚪️ | `white_circle`              |
| ⬛️ | `black_large_square`              | ⬜️ | `white_large_square`        |
| ◼️ | `black_medium_square`             | ◻️ | `white_medium_square`       |
| ◾️ | `black_medium_small_square`       | ◽️ | `white_medium_small_square` |
| ▪️ | `black_small_square`              | ▫️ | `white_small_square`        |
|  🔶  | `large_orange_diamond`            |  🔷  | `large_blue_diamond`        |
|  🔸  | `small_orange_diamond`            |  🔹  | `small_blue_diamond`        |
|  🔺  | `small_red_triangle`              |  🔻  | `small_red_triangle_down`   |
|  💠  | `diamond_shape_with_a_dot_inside` |  🔘  | `radio_button`              |
|  🔳  | `white_square_button`             |  🔲  | `black_square_button`       |

### 其它符合

| 图标 | 代码                            | 图标 | 代码                         |
| :--: | ------------------------------- | :--: | ---------------------------- |
| ♻️ | `recycle`                     | ⚜️ | `fleur_de_lis`             |
|  🔱  | `trident`                     |  📛  | `name_badge`               |
|  🔰  | `beginner`                    | ⭕️ | `o`                        |
|  ✅  | `white_check_mark`            | ☑️ | `ballot_box_with_check`    |
| ✔️ | `heavy_check_mark`            |  ❌  | `x`                        |
|  ❎  | `negative_squared_cross_mark` |  ➰  | `curly_loop`               |
|  ➿  | `loop`                        | 〽️ | `part_alternation_mark`    |
| ✳️ | `eight_spoked_asterisk`       | ✴️ | `eight_pointed_black_star` |
| ❇️ | `sparkle`                     | ©️ | `copyright`                |
| ®️ | `registered`                  | ™️ | `tm`                       |

## 旗帜

### 常用旗帜

| 图标 | 代码               |   图标   | 代码                        |
| :--: | ------------------ | :------: | --------------------------- |
|  🏁  | `checkered_flag` |    🚩    | `triangular_flag_on_post` |
|  🎌  | `crossed_flags`  |    🏴    | `black_flag`              |
| 🏳️ | `white_flag`     | 🏳️‍🌈 | `rainbow_flag`            |

### 国家和地区旗帜

| 图标 | 代码                             | 图标 | 代码                                     |
| :--: | -------------------------------- | :--: | ---------------------------------------- |
| 🇦🇩 | `andorra`                      | 🇦🇪 | `united_arab_emirates`                 |
| 🇦🇫 | `afghanistan`                  | 🇦🇬 | `antigua_barbuda`                      |
| 🇦🇮 | `anguilla`                     | 🇦🇱 | `albania`                              |
| 🇦🇲 | `armenia`                      | 🇦🇴 | `angola`                               |
| 🇦🇶 | `antarctica`                   | 🇦🇷 | `argentina`                            |
| 🇦🇸 | `american_samoa`               | 🇦🇹 | `austria`                              |
| 🇦🇺 | `australia`                    | 🇦🇼 | `aruba`                                |
| 🇦🇽 | `aland_islands`                | 🇦🇿 | `azerbaijan`                           |
| 🇧🇦 | `bosnia_herzegovina`           | 🇧🇧 | `barbados`                             |
| 🇧🇩 | `bangladesh`                   | 🇧🇪 | `belgium`                              |
| 🇧🇫 | `burkina_faso`                 | 🇧🇬 | `bulgaria`                             |
| 🇧🇭 | `bahrain`                      | 🇧🇮 | `burundi`                              |
| 🇧🇯 | `benin`                        | 🇧🇱 | `st_barthelemy`                        |
| 🇧🇲 | `bermuda`                      | 🇧🇳 | `brunei`                               |
| 🇧🇴 | `bolivia`                      | 🇧🇶 | `caribbean_netherlands`                |
| 🇧🇷 | `brazil`                       | 🇧🇸 | `bahamas`                              |
| 🇧🇹 | `bhutan`                       | 🇧🇼 | `botswana`                             |
| 🇧🇾 | `belarus`                      | 🇧🇿 | `belize`                               |
| 🇨🇦 | `canada`                       | 🇨🇨 | `cocos_islands`                        |
| 🇨🇩 | `congo_kinshasa`               | 🇨🇫 | `central_african_republic`             |
| 🇨🇬 | `congo_brazzaville`            | 🇨🇭 | `switzerland`                          |
| 🇨🇮 | `cote_divoire`                 | 🇨🇰 | `cook_islands`                         |
| 🇨🇱 | `chile`                        | 🇨🇲 | `cameroon`                             |
| 🇨🇳 | `cn`                           | 🇨🇴 | `colombia`                             |
| 🇨🇷 | `costa_rica`                   | 🇨🇺 | `cuba`                                 |
| 🇨🇻 | `cape_verde`                   | 🇨🇼 | `curacao`                              |
| 🇨🇽 | `christmas_island`             | 🇨🇾 | `cyprus`                               |
| 🇨🇿 | `czech_republic`               | 🇩🇪 | `de`                                   |
| 🇩🇯 | `djibouti`                     | 🇩🇰 | `denmark`                              |
| 🇩🇲 | `dominica`                     | 🇩🇴 | `dominican_republic`                   |
| 🇩🇿 | `algeria`                      | 🇪🇨 | `ecuador`                              |
| 🇪🇪 | `estonia`                      | 🇪🇬 | `egypt`                                |
| 🇪🇭 | `western_sahara`               | 🇪🇷 | `eritrea`                              |
| 🇪🇸 | `es`                           | 🇪🇹 | `ethiopia`                             |
| 🇪🇺 | `eu` <br /> `european_union` | 🇫🇮 | `finland`                              |
| 🇫🇯 | `fiji`                         | 🇫🇰 | `falkland_islands`                     |
| 🇫🇲 | `micronesia`                   | 🇫🇴 | `faroe_islands`                        |
| 🇫🇷 | `fr`                           | 🇬🇦 | `gabon`                                |
| 🇬🇧 | `gb` <br /> `uk`             | 🇬🇩 | `grenada`                              |
| 🇬🇪 | `georgia`                      | 🇬🇫 | `french_guiana`                        |
| 🇬🇬 | `guernsey`                     | 🇬🇭 | `ghana`                                |
| 🇬🇮 | `gibraltar`                    | 🇬🇱 | `greenland`                            |
| 🇬🇲 | `gambia`                       | 🇬🇳 | `guinea`                               |
| 🇬🇵 | `guadeloupe`                   | 🇬🇶 | `equatorial_guinea`                    |
| 🇬🇷 | `greece`                       | 🇬🇸 | `south_georgia_south_sandwich_islands` |
| 🇬🇹 | `guatemala`                    | 🇬🇺 | `guam`                                 |
| 🇬🇼 | `guinea_bissau`                | 🇬🇾 | `guyana`                               |
| 🇭🇰 | `hong_kong`                    | 🇭🇳 | `honduras`                             |
| 🇭🇷 | `croatia`                      | 🇭🇹 | `haiti`                                |
| 🇭🇺 | `hungary`                      | 🇮🇨 | `canary_islands`                       |
| 🇮🇩 | `indonesia`                    | 🇮🇪 | `ireland`                              |
| 🇮🇱 | `israel`                       | 🇮🇲 | `isle_of_man`                          |
| 🇮🇳 | `india`                        | 🇮🇴 | `british_indian_ocean_territory`       |
| 🇮🇶 | `iraq`                         | 🇮🇷 | `iran`                                 |
| 🇮🇸 | `iceland`                      | 🇮🇹 | `it`                                   |
| 🇯🇪 | `jersey`                       | 🇯🇲 | `jamaica`                              |
| 🇯🇴 | `jordan`                       | 🇯🇵 | `jp`                                   |
| 🇰🇪 | `kenya`                        | 🇰🇬 | `kyrgyzstan`                           |
| 🇰🇭 | `cambodia`                     | 🇰🇮 | `kiribati`                             |
| 🇰🇲 | `comoros`                      | 🇰🇳 | `st_kitts_nevis`                       |
| 🇰🇵 | `north_korea`                  | 🇰🇷 | `kr`                                   |
| 🇰🇼 | `kuwait`                       | 🇰🇾 | `cayman_islands`                       |
| 🇰🇿 | `kazakhstan`                   | 🇱🇦 | `laos`                                 |
| 🇱🇧 | `lebanon`                      | 🇱🇨 | `st_lucia`                             |
| 🇱🇮 | `liechtenstein`                | 🇱🇰 | `sri_lanka`                            |
| 🇱🇷 | `liberia`                      | 🇱🇸 | `lesotho`                              |
| 🇱🇹 | `lithuania`                    | 🇱🇺 | `luxembourg`                           |
| 🇱🇻 | `latvia`                       | 🇱🇾 | `libya`                                |
| 🇲🇦 | `morocco`                      | 🇲🇨 | `monaco`                               |
| 🇲🇩 | `moldova`                      | 🇲🇪 | `montenegro`                           |
| 🇲🇬 | `madagascar`                   | 🇲🇭 | `marshall_islands`                     |
| 🇲🇰 | `macedonia`                    | 🇲🇱 | `mali`                                 |
| 🇲🇲 | `myanmar`                      | 🇲🇳 | `mongolia`                             |
| 🇲🇴 | `macau`                        | 🇲🇵 | `northern_mariana_islands`             |
| 🇲🇶 | `martinique`                   | 🇲🇷 | `mauritania`                           |
| 🇲🇸 | `montserrat`                   | 🇲🇹 | `malta`                                |
| 🇲🇺 | `mauritius`                    | 🇲🇻 | `maldives`                             |
| 🇲🇼 | `malawi`                       | 🇲🇽 | `mexico`                               |
| 🇲🇾 | `malaysia`                     | 🇲🇿 | `mozambique`                           |
| 🇳🇦 | `namibia`                      | 🇳🇨 | `new_caledonia`                        |
| 🇳🇪 | `niger`                        | 🇳🇫 | `norfolk_island`                       |
| 🇳🇬 | `nigeria`                      | 🇳🇮 | `nicaragua`                            |
| 🇳🇱 | `netherlands`                  | 🇳🇴 | `norway`                               |
| 🇳🇵 | `nepal`                        | 🇳🇷 | `nauru`                                |
| 🇳🇺 | `niue`                         | 🇳🇿 | `new_zealand`                          |
| 🇴🇲 | `oman`                         | 🇵🇦 | `panama`                               |
| 🇵🇪 | `peru`                         | 🇵🇫 | `french_polynesia`                     |
| 🇵🇬 | `papua_new_guinea`             | 🇵🇭 | `philippines`                          |
| 🇵🇰 | `pakistan`                     | 🇵🇱 | `poland`                               |
| 🇵🇲 | `st_pierre_miquelon`           | 🇵🇳 | `pitcairn_islands`                     |
| 🇵🇷 | `puerto_rico`                  | 🇵🇸 | `palestinian_territories`              |
| 🇵🇹 | `portugal`                     | 🇵🇼 | `palau`                                |
| 🇵🇾 | `paraguay`                     | 🇶🇦 | `qatar`                                |
| 🇷🇪 | `reunion`                      | 🇷🇴 | `romania`                              |
| 🇷🇸 | `serbia`                       | 🇷🇺 | `ru`                                   |
| 🇷🇼 | `rwanda`                       | 🇸🇦 | `saudi_arabia`                         |
| 🇸🇧 | `solomon_islands`              | 🇸🇨 | `seychelles`                           |
| 🇸🇩 | `sudan`                        | 🇸🇪 | `sweden`                               |
| 🇸🇬 | `singapore`                    | 🇸🇭 | `st_helena`                            |
| 🇸🇮 | `slovenia`                     | 🇸🇰 | `slovakia`                             |
| 🇸🇱 | `sierra_leone`                 | 🇸🇲 | `san_marino`                           |
| 🇸🇳 | `senegal`                      | 🇸🇴 | `somalia`                              |
| 🇸🇷 | `suriname`                     | 🇸🇸 | `south_sudan`                          |
| 🇸🇹 | `sao_tome_principe`            | 🇸🇻 | `el_salvador`                          |
| 🇸🇽 | `sint_maarten`                 | 🇸🇾 | `syria`                                |
| 🇸🇿 | `swaziland`                    | 🇹🇨 | `turks_caicos_islands`                 |
| 🇹🇩 | `chad`                         | 🇹🇫 | `french_southern_territories`          |
| 🇹🇬 | `togo`                         | 🇹🇭 | `thailand`                             |
| 🇹🇯 | `tajikistan`                   | 🇹🇰 | `tokelau`                              |
| 🇹🇱 | `timor_leste`                  | 🇹🇲 | `turkmenistan`                         |
| 🇹🇳 | `tunisia`                      | 🇹🇴 | `tonga`                                |
| 🇹🇷 | `tr`                           | 🇹🇹 | `trinidad_tobago`                      |
| 🇹🇻 | `tuvalu`                       | 🇹🇼 | `taiwan`                               |
| 🇹🇿 | `tanzania`                     | 🇺🇦 | `ukraine`                              |
| 🇺🇬 | `uganda`                       | 🇺🇸 | `us`                                   |
| 🇺🇾 | `uruguay`                      | 🇺🇿 | `uzbekistan`                           |
| 🇻🇦 | `vatican_city`                 | 🇻🇨 | `st_vincent_grenadines`                |
| 🇻🇪 | `venezuela`                    | 🇻🇬 | `british_virgin_islands`               |
| 🇻🇮 | `us_virgin_islands`            | 🇻🇳 | `vietnam`                              |
| 🇻🇺 | `vanuatu`                      | 🇼🇫 | `wallis_futuna`                        |
| 🇼🇸 | `samoa`                        | 🇽🇰 | `kosovo`                               |
| 🇾🇪 | `yemen`                        | 🇾🇹 | `mayotte`                              |
| 🇿🇦 | `south_africa`                 | 🇿🇲 | `zambia`                               |
| 🇿🇼 | `zimbabwe`                     |      |                                          |

