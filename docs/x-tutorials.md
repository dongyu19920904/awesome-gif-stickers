# X 教程与原帖：从一句话 GIF 到微信表情

[返回首页](../README.md) · [原始提示词与案例](prompts.md) · [现成 Skills](skills.md) · [微信规则](wechat.md)

更多已核正文的原帖：[完整素材索引](x-index.md) · [结构化索引](../data/x-materials.json)。

这里整理作者原帖和有独立地址的后续回复，优先保留原始提示词位置、实际做法与结果说明。具体步骤和完整原词请看原帖；原文为中文的材料保留中文来源，不把机器翻译当作英文原文。英文栏是本库导读的翻译。

## 先读这几条 / Start here

| 原作者与原帖 | 中文导读 | English summary |
|---|---|---|
| [路飞：角色参考＋主题槽位](https://x.com/0xluffy_eth/status/2118235547454083357) | 直接请求GIF的原词；另已补核[三步路线](https://x.com/0xluffy_eth/status/2118235549609955443)和[投稿规范入口回复](https://x.com/0xluffy_eth/status/2118235551631610085)的独立地址。原词、流程与规范按原帖分别定位。 | A reference-image GIF prompt, with independently linked workflow and submission-reference replies. |
| [Gorden Sun：吃米饭反应 GIF](https://x.com/Gorden_Sun/status/2118166046175908016) | 一句话指定参考角色、吃米饭动作和“真香”配字，原帖区分参考图与作者展示的结果。 | A short reference-based reaction GIF prompt with Chinese text and a creator example. |
| [Fred：单张 GIF 与整套 Skill](https://x.com/Frederickkk07/status/2118546394797728093) | 有单张直接 GIF 原词，并指向整套 Skill、微信材料和经营来源；单张生成与 Skill 合成是两条不同路线。 | Direct-GIF examples alongside a separate pack-building Skill and submission reading. |
| [零点 Drift：橘猫打工的一天](https://x.com/karanwithai/status/2118190621886165099) | 12张专辑的制作和提交自述：保留角色参考，每次修改动作。此帖为待审，“评论区原词”未完整读到，不补写。 | A creator reports preparing and submitting a 12-GIF pack; this post does not establish approval. |
| [麻酱：猫咪 GIF 投稿长文](https://x.com/zhongying14/status/2118326311030591942) | 重点读专辑材料、含义词、艺术家资料和赞赏配图。作者选8个表情提交；本文不是整套生成提示词库。 | A detailed account of preparing album, creator and optional tipping materials. |
| [杰哥：五步投稿教程](https://x.com/jev_chat/status/2118511250275704964) | 包含直接 GIF 示例、压缩和投稿指引，但作者自己的8张成品用四宫格切片、抠底再合成。 | Direct-GIF guidance and submission notes; the author's own pack uses assembled frames. |
| [杰哥：独立后续回复](https://x.com/jev_chat/status/2118568297243558160) | 作者随后自述已上架，可与前文待审状态对照；尚无本库核到的商店直链或收入。 | An independently linked follow-up reports approval; store listing and income are not verified here. |

## 完整教程与补充帖子

| 原帖 | 适合读什么 | 必要说明 |
|---|---|---|
| [路飞：Image 2.6 的10个玩法](https://x.com/0xluffy_eth/status/2118274913337552992) | 直接 GIF 原词、角色一致性、其他参考图用途 | 同文也给六帧合成方案，展示示例采用后者；10种玩法只是一篇文章 |
| [麻酱：投稿材料补充](https://x.com/zhongying14/status/2118621472847532215) | 对前篇投稿与赞赏材料的简要索引 | 内容与前篇重叠，申请不等于通过或到账 |
| [麻酱：表情IP与商业路径](https://x.com/zhongying14/status/2118619825559793672) | 表情、红包封面、品牌曝光与角色辨识的经营观点 | 是路径讨论，不是本人已经取得收入的证明 |
| [铁柱：照片表情的投稿经历](https://x.com/cgnot996/status/2118567853515575380) | 以往儿童照片投稿的身份材料经历，以及杰哥教程入口 | 是个人经历和再次尝试的计划，不能推广为所有人的统一要求 |
| [Vane：16张表情的制作长文](https://x.com/VaneAILab/status/2118584425009344644) | 提示词、动作图集、素材组织、GIF和微信配套图 | 静态图层位移/形变合成；作者自述已提交待审 |
| [Vane：原项目发布帖](https://x.com/VaneAILab/status/2118367371643719978) | 项目仓库、生成与导出流程 | 对应现成 Skill 的来源；报价或上传不等于成交和审核通过 |
| [Levi：pixel-gif-sticker-pack](https://x.com/Leviwoyun/status/2118197971112366538) | 原项目、交付方式与作者示例 | 代码使用图集/关键帧导出，见[Skills页](skills.md)的源码归类 |
| [往事随风：表情包工坊](https://x.com/bywind_art/status/2118633386445066345) | ray-sticker-shop 的使用报告与入口 | 原仓库有安装说明，所核生成器采用精灵图合成 |
| [AdrianPunk：Punk-IP](https://x.com/AdrianPunk115/status/2117923653019136368) | 个人IP及文章配图 Skill 线索 | 属于静态配图用途，不冒充原生GIF或自动投稿系统 |
| [cheerselflin：提示词库线索](https://x.com/cheerselflin/status/2118671118345310606) | Evolink 的图像提示词/API资料入口 | 属于服务与资料库推广，不是独立GIF Skill |
| [黄啊码：已有专辑赞赏](https://x.com/ama_huangama/status/2118154620744708599) | 创作者已有作品的赞赏经验及背景 | 自述金额不能归因于刚发布的Image 2.6，也不是新人收益保证 |
| [ai_ai_ailover：白龙 GIF 与图像长文](https://x.com/ai_ai_ailover/status/2118232059571544139) | 日文文章展示通过Higgsfield选择GPT Image 2.6制作白龙GIF的作者记录 | 同文包含静态图创作；没有微信发行或收入证据 |

## 从关键词搜索新增的教程

以下为种子之外的增量；均已读取目标正文，保留原词入口，不将目录标签或搜索摘要当教程。

| 作者与原帖 | 值得读的内容 |
|---|---|
| [wolfqing1：角色母图与单个笑点](https://x.com/wolfqing1/status/2118294955236208942) · [独立原词回复](https://x.com/wolfqing1/status/2118295068788621429) | 橘猫、咖啡杯与循环动作的英文原词；先固定角色，再换一个主题 |
| [crayon1267：投篮GIF](https://x.com/crayon1267/status/2118186300339892472) | 以动作顺序图作参考，再要求模型输出投篮GIF；分镜参考不等同于外部拼帧 |
| [Ozan Sihay：猫照片变GIF](https://x.com/ozansihay/status/2118238946412953985) | 以家庭猫照片指定眨眼、落帽及帽上名字，提供简短动作指令 |
| [ai_artworkgen：咖啡馆循环](https://x.com/ai_artworkgen/status/2118235687686140253) | 写实人物局部动作，限定搅咖啡、眨眼和蒸汽，并要求首尾匹配 |
| [Shoji Kai：API实测](https://x.com/Shoji_ai/status/2118523767626559889) | 原生GIF请求、帧数/帧时长、回起点、耗时与画风失效；费用是作者个案 |
| [Midori：照片到Q版再到GIF](https://x.com/midori_tatsuta/status/2118519276848185637) | 独立回复给出两步方法；先准备Q版图，再重新附图要求循环动作 |
| [SUOHA：定制与赞赏](https://x.com/SUOHA_AI/status/2118564255867777123) · [平台与授权回复](https://x.com/SUOHA_AI/status/2118564264491287014) | 比较两种经营路径，补官方入口和原创/肖像授权提醒；没有可核实订单 |
| [gbroai：Codex原生GIF拼贴B-roll](https://x.com/gbroai/status/2118589683819262346) | 参考静帧、原生GIF、导出MP4的完整创作文章；作者当时公开的Skill仍是旧视频模型版 |

## 新增实测与排错 / More tests and troubleshooting

以下原帖核读于 2026-11-07。数值与结果属于作者当次记录，未在本库复现。

| 原作者与原帖 | 中文导读 | English summary |
|---|---|---|
| [r360studio：角色 GIF 演示](https://x.com/r360studio/status/2118843579712123227) | 作者附从输入到生成完成的视频讲解，报告角色与尾巴循环保持、307×307像素、16帧及约8.3fps。可看输入操作和结果；这组尺寸不等于微信投稿规格。 | A narrated character-GIF demonstration; the creator reports dimensions, frame count and loop behavior. |
| [Superboy：帧数、时长与回位](https://x.com/Superboy4949/status/2118785150368743814) | 报告每帧120ms时，8帧为0.96秒、16帧为1.92秒；建议结合帧时长调整循环长度，并在提示词中安排动作回到起始姿势。 | A duration example at 120ms per frame, with advice to return the action to its starting pose. |
| [Felnart：先让模型提议场景](https://x.com/felnartstories/status/2118758557537710141) | 原帖有场景提议指令和魔法循环结果，并明确记录手臂、长矛晃动的问题；可参考动作约束与失败表现。 | A scene-ideation request and magical-loop example, including reported arm and spear artifacts. |
| [1stLight：较长生成的失真反馈](https://x.com/1stLight_Ai/status/2118784492227965350) | 作者报告较长的GIF生成出现崩坏，提出下一次尝试参考照片；后者尚属计划，不当作已经验证的修复办法。 | A reported failure with longer GIF generations; a reference-photo retry is proposed, not demonstrated. |
| [Hemi：两头身角色跳舞、转身与循环](https://x.com/Hemi3AI/status/2118450538966823011) | 原帖给出先改为两头身、再跳舞转一圈并循环的短指令，指出模型对“转一圈”的理解偏离预期。角色属于原作者示例，不能据此取得其商业授权。 | Short character-motion instructions, with a reported mismatch in the interpretation of one full turn. |
| [HeartlessCat：参考图与极短动作词](https://x.com/dokken92047824/status/2118293666456559762) | 作者附图后只指定男性弹木吉他，展示这种极简输入的结果；可对照参考图和动作描述的作用，不是完整专辑教程。 | A reference image and a minimal guitar-playing instruction, presented as a creator test. |
| [seosoyoung：Flare 参考图 GIF 实测](https://x.com/seosoyoung_ai/status/2118142838198169750) | 作者报告一张Q版参考图、一次调用，约14秒返回6帧GIF，并反馈转得过快。耗时和帧数是该次记录；文中对当时文档的转述不能代替当前官方能力说明。 | A reported reference-image Flare test returning six frames, including feedback that the rotation was too fast. |
| [vastxie：两套微信动态表情的四步流程](https://x.com/vastxie/status/2118265895613346263) | 锚点图、批量动作、深色背景去白边与配套图整理；原帖给出调用设置与避坑短提示。约4美元赠金额消耗是作者报告，未证明审核或盈利；[微信页导读](wechat.md#10--弎弎水锚点图两套动态表情与深色背景处理)。 | An anchor-image workflow and WeChat display fixes, with reported credit use rather than verified earnings. |

## 官方对照与相关资料库

- [OpenAI Image prompting](https://developers.openai.com/api/docs/guides/image-prompting#generate-a-looping-gif)：官方循环GIF样例，说明起始姿态、回位动作和镜头约束。API参数另看[生成指南](https://developers.openai.com/api/docs/guides/image-generation#generate-animated-gif-output)。
- [微信制作和投稿教程](wechat.md)：把作者经验中的规格、入口与当前公开规则对应起来。
- [zhuyansen / Awesome ChatGPT Images 2.6](https://github.com/zhuyansen/awesome-chatgpt-images-2.6)：已有中英资料仓库，按原帖、作者、类别、媒体类型和原词出处组织；有[可浏览案例页](https://jasonzhu.ai/en/prompts/chatgpt-images-2-6)。作者未公开的原词明确留空，本库链接参考其组织方式，不复制媒体或未授权数据。

## 怎样理解这些资料

“原帖正文已读”只说明导读有原始依据。直接请求GIF的提示词、作者实际采用的成品路线、提交状态和收入分别核对：同一篇文章可能混合多条路线；作者报告不等于本库复现或平台确认。

公开页只做署名导读和原文导航。未经确认可转载的长文、完整提示词及媒体不整包发布；原文和素材继续归各自作者。
