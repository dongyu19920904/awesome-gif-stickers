# 原生 GIF 提示词与作者案例

[返回首页](../README.md) · [生成与后处理工具](tools.md)

补充入口：[X 原始提示词与教程帖](x-tutorials.md) · [可选现成 Skills](skills.md) · [OpenAI 官方提示指南](https://developers.openai.com/api/docs/guides/image-prompting#generate-a-looping-gif)。

这里收录 **5 条可直接复制的外部模板（中英对照）**、**6 篇附原词位置和结果展示的作者教程**，另有 **41 条带示例的外部原提示目录**。核查日期：2026-11-07。

先确认所用入口支持 GIF。[OpenAI 的 ChatGPT 帮助](https://help.openai.com/en/articles/11084440-images-in-chatgpt)说明，可以上传静态图并要求动画，GIF 功能仍在逐步推出。需要参考图的原词，应连同自己有权使用的图片一起提交。API 用户以[当前官方指南的 GIF 章节](https://developers.openai.com/api/docs/guides/image-generation#generate-animated-gif-output)为准；不要照搬第三方教程中的旧参数表。

## 可直接复制：5 条开放许可模板

以下英文原词全文摘录自 **Anil-matcha** 发布的 [Awesome-GPT-Image-2.6-API-Prompts — Animated GIFs](https://github.com/Anil-matcha/Awesome-GPT-Image-2.6-API-Prompts/blob/426032b613a85eef2936a226db2b0698ad698782/README.md#animated-gifs)，版本日期 2026-11-05，固定版本 `426032b613a85eef2936a226db2b0698ad698782`。来源仓库以 [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)授权，见其[许可声明](https://github.com/Anil-matcha/Awesome-GPT-Image-2.6-API-Prompts/blob/426032b613a85eef2936a226db2b0698ad698782/LICENSE)。

**改动说明：**英文原词逐字保留，中文块为本库翻译，另加中文标题、导读和适用说明。来源没有为每条另列创作者，故按仓库署名归属。作者将这些词称为起步模板，未附对应 GIF 成品或生成日志；以下不是五个已实测案例。

### 1. 吉祥物挥手

原题：Looping Brand Mascot。用于文字描述一个固定角色，观察抬手、挥手、回位的短循环。

```text
A looping animated GIF of a friendly round teal robot mascot waving its right arm: frame 1 arm down, middle frames arm raised and swinging side to side, final frame returning to arm down so the loop is seamless. Flat vector style, clean white background, identical character proportions and colors in every frame.
```

**中文译文（本库翻译）：**

```text
制作一个循环播放的动画 GIF：友善、圆滚滚的青绿色机器人吉祥物挥动右臂。第1帧手臂垂下，中间几帧抬起手臂左右挥动，最后一帧回到手臂垂下的状态，让循环首尾无缝。扁平矢量风格，干净的白色背景，每一帧的角色比例和颜色保持一致。
```

### 2. 猫咪惊讶反应

原题：Reaction Meme。含英文台词，取用时需检查每帧的表情和文字。

```text
An animated reaction GIF of a cartoon cat slowly turning from a calm expression to wide-eyed shock, then a small "WAIT, WHAT?" caption popping in at the end. Bold outlines, pastel background, consistent character design across all frames.
```

**中文译文（本库翻译）：**

```text
制作一个卡通猫的反应动画 GIF：表情慢慢从平静变为瞪大眼睛的震惊，最后弹出一行小字幕“WAIT, WHAT?”。粗线条轮廓，淡彩背景，所有帧中的角色设计保持一致。
```

### 3. 纸船经过水洼

原题：Animated Storyboard Beat。适合参考短动作的描述方式；原词包含入画和出画，未承诺首尾无缝。

```text
An animated storyboard GIF of a paper boat drifting across a puddle: boat enters from the left, ripples expand beneath it, boat exits to the right. Soft watercolor look, overhead camera, same puddle and lighting in every frame.
```

**中文译文（本库翻译）：**

```text
制作一个纸船漂过水洼的分镜动画 GIF：纸船从左侧进入，下方的涟漪向外扩散，纸船从右侧离开。柔和的水彩风格，俯视镜头，每一帧保持相同的水洼与光照。
```

### 4. 正在输入的小角色

原题：Typing-Indicator Character。原词的 `transparent-looking` 是外观描述，不是透明通道或微信适配保证。

```text
A tiny looping GIF of a cute blob character bouncing three times as if typing, simple two-color palette, transparent-looking pastel background, same character shape and size in every frame.
```

**中文译文（本库翻译）：**

```text
制作一个小型循环 GIF：可爱的团状角色弹跳三次，仿佛正在打字。简单的双色配色，看起来透明的淡彩背景，每一帧保持相同的角色形状与大小。
```

### 5. 手绘草图变动画角色

原题：Sketch to Animated Character。需要在支持参考图的入口附上手绘草图；单独复制文字没有提供原词要求的输入。

```text
Turn the attached hand-drawn sketch into an animated character GIF: keep the sketch's shape and line quality, add a gentle idle animation (blinking, slight head tilt), consistent proportions in all frames, plain background.
```

**中文译文（本库翻译）：**

```text
把附上的手绘草图变成角色动画 GIF：保留草图的形状和线条质感，添加轻微的待机动画（眨眼、略微歪头），所有帧中的比例保持一致，背景简洁。
```

以上五条的适用入口按来源说明为 GPT Image 2.6 Flare / Sunburst，作者称多数也适用于 ChatGPT Images 2.6。实际入口、参数及输出需各自确认；来源中的接口说明不随本页摘录。

## 作者案例：到原文取用提示词、查看结果

下面各篇都能在原文找到提示词，但未确认开放转载许可，因此本页只提供独立导读和准确位置。**“有作者展示”表示原页有结果或记录，不表示本项目下载检查过文件、在微信可用、过审或产生收入。** 媒体保留在原作者页面，不在本仓库镜像。

### 1. 从自己的照片开始：蔡明淳的猫咪与真人 GIF

[阅读原文：ChatGPT Images 2.6 怎么用？免费做 GIF 动图教学](https://gretatsai.com/chatgpt-images-2-6-gif/) — 蔡明淳，2026-11-05。

**入口与原词：**作者使用 ChatGPT 网页 Plus 实测。查找「用自己的照片做 GIF：讓照片動起來實測」，可取得照片输入条件、完整原词和成品；「實測：用 ChatGPT 做一張『股市大跌，小貓跳舞』GIF」另有三版原词与结果。

**值得看：**作者把“换风格”“调整动作”“改比例”分别展示，还记录了要求 9:16 却返回正方形，以及真人动作和数字的小瑕疵。适合看第一次输出不合意后怎样具体修改。文中的股市画面是创作内容，不是行情资料；作者照片与成品没有因此授权读者商用。

### 2. 参考图与角色一致性：程序员鱼皮的实测

[阅读原文：一键生成 GIF 动图](https://cloud.tencent.com.cn/developer/article/2777024) — 程序员鱼皮，2026-11-05。

**入口与原词：**ChatGPT 图像创建、上传参考照片。查找「2、鱼皮线上报错，当场瘫坐」取得真人照片案例原词；「5、修好 Bug 的火柴人」是草图案例；「7、鱼皮喂大肥鱼」记录了保存参考照片读取失败后重试的过程。

**值得看：**各段有提示词和结果图，作者同时承认真人还原有限、部分帧眼镜消失。文章中的奶龙等角色适合阅读方法，不能凭能生成就当作可销售素材。原文明确未经许可不得转载，本页不搬运全文提示词或媒体；关于模型内部原理的作者猜测不作为本库技术结论。

### 3. 从一张定妆图扩成常用语：UPGPTs 的水豚教程

[阅读原文：用参考图生成 GIF 表情包、贺卡和电商动图](https://upgpts.com/tutorials/chatgpt/chatgpt-image-2.6-guide) — UPGPTs 团队，2026-11-06。

**入口与原词：**教程使用 ChatGPT。查找「玩法一：做一套水豚『躺平组长』表情包」：第一步给定妆图原词，第二步给单个 GIF 原词和六种常用语动作表。

**值得看：**原页展示定妆图与点头回应的示例，适合把同一参考图衔接到多条聊天话术。六种动作表不等于展示了六个完整生成记录，也没有微信过审或成交凭据。网站包含代充服务推广；套餐、账号权限和平台参数请另查官方，不据本教程判断。

### 4. 帧数与文件体积：CreateVision 的两段商品 GIF

[阅读原文：GPT Image 2.6 实测](https://createvision.ai/zh/gpt-image-2-6) — CreateVision AI，测试日期 2026-11-05。

**入口与原词：**供应商自有工作台，作者标为 GPT Image 2.6 Sunburst。查找「04 / 商品循环动图」下的「提示词与设置」取得原词；「按动作需要选择 GIF 帧数」并列展示 4 帧与 16 帧结果，完整测试记录另给原文件入口。

**值得看：**同一商品参考图、同一原词，能比较循环长度、体积及细微形变。它不是微信表情案例，但对准备压缩动图有参考价值。页面的 20 次请求包含静态图，只有两段是 GIF；积分是当时报价，不是已对账扣费或收益。参数和样本结论仅代表该供应商的记录。

### 5. 单个小动作：Lightlyn 的吉祥物、商品和照片

[阅读原文：GPT Image 2.6 is here: animated GIFs and SVG vectors](https://image.lightlyn.com/gpt-image-2-6?lang=en) — Linger / Lightlyn Images，2026-11-05。

**入口与原词：**供应商 Lightlyn Images，选择 GPT Image 2.6 后在 Advanced 中选 GIF。查找「Describe the motion, get a loop」下的「Prompts」，有猫咪挥手、耳机盒开合、咖啡照片蒸汽三条英文原词，以及对应结果；照片案例须附参考照片。

**值得看：**三种主体都聚焦小动作，便于对照哪些细节保持不动。作者展示的是自有平台结果，九帧、耗时与界面选项不能推广为所有入口的统一规则。页面含产品推广；本项目未验证其服务或扣费。

### 6. 生成后保持动作改表情：npaka 的三段上手原词

[阅读原文：GPT-Image-2.6の概要 - ChatGPTがアニメーションGIF生成に対応](https://note.com/npaka/n/n7e86091b23c3) — npaka / 布留川英一，2026-11-05。

**入口与原词：**第 2 章「クイックスタート」的 2-1 是文字生成跳舞猫 GIF；2-2 是上传角色图、保留角色和背景后生成 GIF；2-3 是给已生成 GIF 追加指令，保持同一动作改成笑脸。三段日文原词均在原页，另嵌四条作者 X 结果入口。

**值得看：**能顺着同一流程比较文字生成、角色参考与后续修改。本库未下载嵌入媒体复现；文中的提速表述存在过时之处，API 参数与价格请查当前官方指南。

## 来源跳转：41 条带示例的 GIF 原提示

来源：[ailingqu / Awesome AI GIF Prompts](https://github.com/ailingqu/awesome-ai-gif-prompts/blob/2672b8fe04e75275de70a8d5d2992da6271ce8f5/README.md)，固定版本 `2672b8fe04e75275de70a8d5d2992da6271ce8f5`（2026-11-06）；[CC BY 4.0](https://github.com/ailingqu/awesome-ai-gif-prompts/blob/2672b8fe04e75275de70a8d5d2992da6271ce8f5/LICENSE)。本表由该版 `data/prompts.json` 的 41 个唯一条目整理，英文标题与中文标题均沿用来源，中文列是来源作者的译名；完整英文原词与提示中的循环后缀请到原页读取。

作者说明这些提示词由网上思路改写并生成测试，仓库附对应 GIF；这是来源作者的报告，本库未运行请求或逐个解码媒体。下表是一个仓库的 41 条提示，不是 41 条 X 帖子。生成示例使用第三方服务，接口参数和素材规格以实际入口为准。

### 表情包与贴纸 GIF（15 条）

| 编号 | 原文标题 | 来源中文标题 | 原提示入口 |
| --- | --- | --- | --- |
| 1 | Jelly bear wobble | Q 弹果冻熊摇晃 | [英文原词](https://github.com/ailingqu/awesome-ai-gif-prompts/blob/2672b8fe04e75275de70a8d5d2992da6271ce8f5/data/prompts.json#L27) |
| 2 | Bunny thumbs-up | 兔兔点赞 | [英文原词](https://github.com/ailingqu/awesome-ai-gif-prompts/blob/2672b8fe04e75275de70a8d5d2992da6271ce8f5/data/prompts.json#L41) |
| 3 | Bunny laughing to tears | 兔兔笑出眼泪 | [英文原词](https://github.com/ailingqu/awesome-ai-gif-prompts/blob/2672b8fe04e75275de70a8d5d2992da6271ce8f5/data/prompts.json#L55) |
| 4 | Sleepy bunny | 兔兔犯困 | [英文原词](https://github.com/ailingqu/awesome-ai-gif-prompts/blob/2672b8fe04e75275de70a8d5d2992da6271ce8f5/data/prompts.json#L67) |
| 5 | Cartoon cat waving hello | 卡通猫挥手打招呼 | [英文原词](https://github.com/ailingqu/awesome-ai-gif-prompts/blob/2672b8fe04e75275de70a8d5d2992da6271ce8f5/data/prompts.json#L79) |
| 6 | Confused shiba head tilt | 柴犬歪头疑惑 | [英文原词](https://github.com/ailingqu/awesome-ai-gif-prompts/blob/2672b8fe04e75275de70a8d5d2992da6271ce8f5/data/prompts.json#L93) |
| 7 | Cat typing furiously | 猫猫疯狂打字 | [英文原词](https://github.com/ailingqu/awesome-ai-gif-prompts/blob/2672b8fe04e75275de70a8d5d2992da6271ce8f5/data/prompts.json#L105) |
| 8 | Frog blowing a heart | 青蛙吹出爱心 | [英文原词](https://github.com/ailingqu/awesome-ai-gif-prompts/blob/2672b8fe04e75275de70a8d5d2992da6271ce8f5/data/prompts.json#L119) |
| 9 | Penguin facepalm | 企鹅捂脸 | [英文原词](https://github.com/ailingqu/awesome-ai-gif-prompts/blob/2672b8fe04e75275de70a8d5d2992da6271ce8f5/data/prompts.json#L131) |
| 10 | Basketball shot celebration | 投篮命中庆祝 | [英文原词](https://github.com/ailingqu/awesome-ai-gif-prompts/blob/2672b8fe04e75275de70a8d5d2992da6271ce8f5/data/prompts.json#L143) |
| 11 | Cat chef tossing fried rice | 猫厨师颠勺炒饭 | [英文原词](https://github.com/ailingqu/awesome-ai-gif-prompts/blob/2672b8fe04e75275de70a8d5d2992da6271ce8f5/data/prompts.json#L157) |
| 12 | Black cat punch | 黑猫出拳 | [英文原词](https://github.com/ailingqu/awesome-ai-gif-prompts/blob/2672b8fe04e75275de70a8d5d2992da6271ce8f5/data/prompts.json#L169) |
| 13 | Office cat: exhausted | 打工猫：累瘫 | [英文原词](https://github.com/ailingqu/awesome-ai-gif-prompts/blob/2672b8fe04e75275de70a8d5d2992da6271ce8f5/data/prompts.json#L181) |
| 14 | Office cat: clocking out | 打工猫：下班啦 | [英文原词](https://github.com/ailingqu/awesome-ai-gif-prompts/blob/2672b8fe04e75275de70a8d5d2992da6271ce8f5/data/prompts.json#L195) |
| 15 | Roaring duck | 咆哮的小黄鸭 | [英文原词](https://github.com/ailingqu/awesome-ai-gif-prompts/blob/2672b8fe04e75275de70a8d5d2992da6271ce8f5/data/prompts.json#L207) |

### 快闪与品牌动效 GIF（5 条）

| 编号 | 原文标题 | 来源中文标题 | 原提示入口 |
| --- | --- | --- | --- |
| 16 | Flower macro flash cut | 花卉微距快闪 | [英文原词](https://github.com/ailingqu/awesome-ai-gif-prompts/blob/2672b8fe04e75275de70a8d5d2992da6271ce8f5/data/prompts.json#L219) |
| 17 | Cat-head logo brand reel | 猫头 Logo 品牌快闪 | [英文原词](https://github.com/ailingqu/awesome-ai-gif-prompts/blob/2672b8fe04e75275de70a8d5d2992da6271ce8f5/data/prompts.json#L233) |
| 18 | Sneaker colorway flash | 球鞋配色快闪 | [英文原词](https://github.com/ailingqu/awesome-ai-gif-prompts/blob/2672b8fe04e75275de70a8d5d2992da6271ce8f5/data/prompts.json#L247) |
| 19 | One tree, four seasons | 一棵树的四季 | [英文原词](https://github.com/ailingqu/awesome-ai-gif-prompts/blob/2672b8fe04e75275de70a8d5d2992da6271ce8f5/data/prompts.json#L261) |
| 20 | Magazine collage panels pop in | 杂志拼贴逐格弹出 | [英文原词](https://github.com/ailingqu/awesome-ai-gif-prompts/blob/2672b8fe04e75275de70a8d5d2992da6271ce8f5/data/prompts.json#L273) |

### 氛围循环 GIF（12 条）

| 编号 | 原文标题 | 来源中文标题 | 原提示入口 |
| --- | --- | --- | --- |
| 21 | Reading by the window, day to night | 窗边读书·白天到夜晚 | [英文原词](https://github.com/ailingqu/awesome-ai-gif-prompts/blob/2672b8fe04e75275de70a8d5d2992da6271ce8f5/data/prompts.json#L287) |
| 22 | Steaming coffee loop | 冒热气的咖啡 | [英文原词](https://github.com/ailingqu/awesome-ai-gif-prompts/blob/2672b8fe04e75275de70a8d5d2992da6271ce8f5/data/prompts.json#L301) |
| 23 | Rainy window and plant | 雨窗与绿植 | [英文原词](https://github.com/ailingqu/awesome-ai-gif-prompts/blob/2672b8fe04e75275de70a8d5d2992da6271ce8f5/data/prompts.json#L313) |
| 24 | Goldfish in a bowl | 鱼缸里的金鱼 | [英文原词](https://github.com/ailingqu/awesome-ai-gif-prompts/blob/2672b8fe04e75275de70a8d5d2992da6271ce8f5/data/prompts.json#L325) |
| 25 | Lighthouse at night | 夜晚的灯塔 | [英文原词](https://github.com/ailingqu/awesome-ai-gif-prompts/blob/2672b8fe04e75275de70a8d5d2992da6271ce8f5/data/prompts.json#L337) |
| 26 | Cat sleeping by the fireplace | 壁炉边睡觉的猫 | [英文原词](https://github.com/ailingqu/awesome-ai-gif-prompts/blob/2672b8fe04e75275de70a8d5d2992da6271ce8f5/data/prompts.json#L349) |
| 27 | Lantern monkey in the snow | 雪林提灯的小猴子 | [英文原词](https://github.com/ailingqu/awesome-ai-gif-prompts/blob/2672b8fe04e75275de70a8d5d2992da6271ce8f5/data/prompts.json#L363) |
| 28 | Sleepy fox on a mossy rock | 苔石上打盹的小狐狸 | [英文原词](https://github.com/ailingqu/awesome-ai-gif-prompts/blob/2672b8fe04e75275de70a8d5d2992da6271ce8f5/data/prompts.json#L377) |
| 29 | Lo-fi study loop | Lo-fi 学习循环 | [英文原词](https://github.com/ailingqu/awesome-ai-gif-prompts/blob/2672b8fe04e75275de70a8d5d2992da6271ce8f5/data/prompts.json#L389) |
| 30 | Café cinemagraph | 街角咖啡馆动态照片 | [英文原词](https://github.com/ailingqu/awesome-ai-gif-prompts/blob/2672b8fe04e75275de70a8d5d2992da6271ce8f5/data/prompts.json#L401) |
| 31 | Ink-wash galloping horse | 水墨奔马 | [英文原词](https://github.com/ailingqu/awesome-ai-gif-prompts/blob/2672b8fe04e75275de70a8d5d2992da6271ce8f5/data/prompts.json#L415) |
| 32 | Doodle monster comes alive | 涂鸦小怪兽活了 | [英文原词](https://github.com/ailingqu/awesome-ai-gif-prompts/blob/2672b8fe04e75275de70a8d5d2992da6271ce8f5/data/prompts.json#L427) |

### 像素风与界面动效 GIF（9 条）

| 编号 | 原文标题 | 来源中文标题 | 原提示入口 |
| --- | --- | --- | --- |
| 33 | Pixel art campfire | 像素风篝火 | [英文原词](https://github.com/ailingqu/awesome-ai-gif-prompts/blob/2672b8fe04e75275de70a8d5d2992da6271ce8f5/data/prompts.json#L439) |
| 34 | Bouncing dots loader | 弹跳圆点加载动画 | [英文原词](https://github.com/ailingqu/awesome-ai-gif-prompts/blob/2672b8fe04e75275de70a8d5d2992da6271ce8f5/data/prompts.json#L451) |
| 35 | Pixel knight run cycle | 像素骑士跑步循环 | [英文原词](https://github.com/ailingqu/awesome-ai-gif-prompts/blob/2672b8fe04e75275de70a8d5d2992da6271ce8f5/data/prompts.json#L465) |
| 36 | Like button heart burst | 点赞爱心爆开 | [英文原词](https://github.com/ailingqu/awesome-ai-gif-prompts/blob/2672b8fe04e75275de70a8d5d2992da6271ce8f5/data/prompts.json#L479) |
| 37 | Hourglass loading | 沙漏加载 | [英文原词](https://github.com/ailingqu/awesome-ai-gif-prompts/blob/2672b8fe04e75275de70a8d5d2992da6271ce8f5/data/prompts.json#L491) |
| 38 | Arcade VS screen | 街机对战 VS 画面 | [英文原词](https://github.com/ailingqu/awesome-ai-gif-prompts/blob/2672b8fe04e75275de70a8d5d2992da6271ce8f5/data/prompts.json#L503) |
| 39 | 8-bit slime boss battle | 8-bit 史莱姆 Boss 战 | [英文原词](https://github.com/ailingqu/awesome-ai-gif-prompts/blob/2672b8fe04e75275de70a8d5d2992da6271ce8f5/data/prompts.json#L517) |
| 40 | Love-burst skill animation | 爱心爆发技能动画 | [英文原词](https://github.com/ailingqu/awesome-ai-gif-prompts/blob/2672b8fe04e75275de70a8d5d2992da6271ce8f5/data/prompts.json#L529) |
| 41 | Junkyard robot walk cycle | 废品场机器人行走 | [英文原词](https://github.com/ailingqu/awesome-ai-gif-prompts/blob/2672b8fe04e75275de70a8d5d2992da6271ce8f5/data/prompts.json#L541) |

## 原帖公开的24条GIF原词入口

线索来自 [GPTProto 的 GIF 案例目录](https://github.com/GPTProto/awesome-gpt-image-2.6-gif/tree/5312eaa46714a6881e145026e4664e4fb4c89845)。以下24条均已核对作者原帖正文，确有实际提示词；保留原语言，完整原词与参考素材请到原帖取用。表中“见原文”表示尚未核清生成路线，不把网格/精灵图措辞自动判为原生或外部拼帧。

| 原帖题材与作者 | 原文语言 | 路线 |
|---|---|---|
| [小说片段转人物GIF · @MrGafish](https://x.com/MrGafish/status/2118147815008518564) | 中文 | 原生请求 |
| [劈柴老人和转身眨眼：同帖两个短提示 · @koe_ai414](https://x.com/koe_ai414/status/2118153765094351279) | 日文 | 原生请求 |
| [纸船循环GIF短提示与角色一致性模板 · @thinkszyg](https://x.com/thinkszyg/status/2118166234495947044) | 中文 | 见原文 |
| [像素勇者挥剑特效GIF · @YaReYaRu30Life](https://x.com/YaReYaRu30Life/status/2118166505603153922) | 日文 | 原生请求 |
| [三视图转像素角色紫色闪电GIF · @YaReYaRu30Life](https://x.com/YaReYaRu30Life/status/2118167174053597233) | 日文 | 原生请求 |
| [角色扭动动作GIF短提示 · @TaikiTaiki04](https://x.com/TaikiTaiki04/status/2118177315176001988) | 日文 | 原生请求 |
| [意外自拍风格GIF提示 · @nixus404](https://x.com/nixus404/status/2118180448840872167) | 英文 | 原生请求 |
| [着火房间喝茶小狗的表情变化循环 · @shitunote](https://x.com/shitunote/status/2118187063241777311) | 中文 | 原生请求 |
| [纽约雪景球GIF短提示 · @dreamwieber](https://x.com/dreamwieber/status/2118190877567037732) | 英文 | 原生请求 |
| [黏土小猫在球池玩耍GIF · @dreamwieber](https://x.com/dreamwieber/status/2118191599872344467) | 英文 | 原生请求 |
| [白底线条小狗摇尾巴循环表情包 · @CalosLaw](https://x.com/CalosLaw/status/2118199125707547102) | 中文 | 原生请求 |
| [单张角色图转挥手微笑GIF · @okan_aitool](https://x.com/okan_aitool/status/2118201578406772887) | 日文 | 原生请求 |
| [文字生成与上传照片生成GIF的双入口教程 · @o_adeeko](https://x.com/o_adeeko/status/2118203950306410729) | 英文 | 原生请求 |
| [机器人泡咖啡GIF实测短提示 · @sousoccer6](https://x.com/sousoccer6/status/2118210705585537226) | 日文 | 原生请求 |
| [勤劳小蜜蜂签到GIF提示 · @MrGafish](https://x.com/MrGafish/status/2118217749680025722) | 中文 | 原生请求 |
| [两行文字的聊天活动标题GIF · @iidaatcnt](https://x.com/iidaatcnt/status/2118218668408746367) | 日文 | 原生请求 |
| [参考角色图片转跳舞GIF · @munou_ac](https://x.com/munou_ac/status/2118220485150535796) | 日文 | 原生请求 |
| [一句话参考图转GIF及六格替代路线线索 · @daifuku_ailover](https://x.com/daifuku_ailover/status/2118224031518454108) | 日文 | 见原文 |
| [角色参考图变Q版可爱动作GIF · @shinshin86](https://x.com/shinshin86/status/2118225428976705908) | 日文 | 原生请求 |
| [同一IP的砸电脑与大肥鱼两张GIF · @Gimi_min](https://x.com/Gimi_min/status/2118243060064964703) | 中文 | 原生请求 |
| [上传猫图制作晚安喵GIF · @eeseverlasting](https://x.com/eeseverlasting/status/2118248165396848968) | 日文 | 原生请求 |
| [烧杯漩涡与发光颜色的GIF场景提示 · @ZHENGJUNTING92](https://x.com/ZHENGJUNTING92/status/2118252052556255364) | 中文 | 原生请求 |
| [象征平成时代的社交GIF短提示 · @rem_rev](https://x.com/rem_rev/status/2118252486360498485) | 日文 | 原生请求 |
| [迷幻跳舞猫GIF短提示 · @xedrik7](https://x.com/xedrik7/status/2118258491043483978) | 英文 | 原生请求 |

这里只整理署名导读和原帖跳转，不复制未明确授权转载的完整原词或媒体。

## 从作者时间线、回复和案例目录补核的原词

| 原词入口 | 适合参考 | 路线 |
|---|---|---|
| [crayon1267 · 下班啦](https://x.com/crayon1267/status/2118636908175859897) | 角色参考、中文配字和透明底循环 | 直接 GIF 请求 |
| [crayon1267 · 品牌快闪](https://x.com/crayon1267/status/2118521104075837700) | 让 GIF 按多格参考图的顺序切换内容 | 多格输入，直接 GIF 请求 |
| [AXIS 实验室 · 水獭设定图和早安动图](https://x.com/AXIS95277/status/2118320301259788490) | 分开定义角色三视图与早安循环 | 设定图后请求 GIF |
| [AXIS 实验室 · 保留原图文字的九个动作](https://x.com/AXIS95277/status/2118264156885221681) | 让现有表情图动起来，保留字形与角色 | 直接 GIF 请求 |
| [AXIS 实验室 · 无参考图的挥手对照](https://x.com/AXIS95277/status/2118264180239184369) | 查看从文字开始生成的对照指令 | 直接 GIF 请求 |
| [弎弎水 · 藏狐参考图和动作槽位](https://x.com/vastxie/status/2118586752915095805) | 改动作和配字，并参考作者的透明 GIF 去白边方法 | 动画请求与 Pillow 后处理 |
| [半格 · 十二种心情的表情原词](https://x.com/ai_bange/status/2118339589144490122) | 同一角色覆盖多种聊天场景，按参考图换动作和表情 | 作者混合工作流 |
| [Derek · 中英双语敬礼原词](https://x.com/derek_wall90176/status/2118175241390436830) | 动作回到起始姿势，字幕留在固定位置 | 直接 GIF 请求，透明底是原词要求 |
| [abc123 · 现有表情图的微动作](https://x.com/abc123953468547/status/2118188187193634981) | 保留原图内容，将动作集中在角色细节 | 直接 GIF 请求 |
| [op7418 · 按主题换动作的大肥鱼](https://x.com/op7418/status/2118181972451438662) | 固定参考角色，按主题改动作与短配字 | 直接 GIF 请求 |
| [Voxyz · 角色挥杖回位](https://x.com/Voxyz_ai/status/2118750260549796019) | 参考角色、12 帧循环的原词和作者画质比较 | 直接 GIF 请求 |
| [Ed Son · 封面图转自然循环](https://x.com/ai_edisonZ/status/2118677271880073230) | 保留文章封面的设计，用小范围运动做循环 | 直接 GIF 请求 |

## 从提示词继续到微信

先在作者原页看输入与完整循环，再取用原词。用自己的照片、原创角色或有授权素材替换参考图时，应保留相应权利依据。开放许可模板允许按许可转载，不同时授权任何第三方角色、肖像或品牌。

继续阅读：[微信添加与投稿教程](wechat.md) · [已有 GIF 的处理工具](tools.md) · [变现教程与经验](monetization.md)。
