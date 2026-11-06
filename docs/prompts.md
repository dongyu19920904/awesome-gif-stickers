# 原生 GIF 提示词与作者案例

[返回首页](../README.md) · [生成与后处理工具](tools.md)

这里收录 **5 条可直接复制的外部模板（中英对照）**，以及 **5 篇附原词位置和结果展示的作者教程**。核查日期：2026-11-06。模板与作者案例分开列出。

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

## 从提示词继续到微信

先在作者原页看输入与完整循环，再取用原词。用自己的照片、原创角色或有授权素材替换参考图时，应保留相应权利依据。开放许可模板允许按许可转载，不同时授权任何第三方角色、肖像或品牌。

继续阅读：[微信添加与投稿教程](wechat.md) · [已有 GIF 的处理工具](tools.md) · [变现教程与经验](monetization.md)。
