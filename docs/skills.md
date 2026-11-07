# 现成 Skills：按用途选，再去原仓库安装

[返回首页](../README.md) · [生成入口与工具](tools.md) · [微信制作与投稿](wechat.md)

收录 **11 个 Skill、10 个项目入口**，包括 5 个原生 GIF 请求入口（6 个 Skill）、4 个素材合成与交付入口、1 个依赖宿主的聊天表情工作流。核查日期为 2026-11-07。链接指向固定版本的安装说明、Skill 和代码。本库核查了文档和源码，安装与运行效果尚待使用者按自己的环境验证。

## 原生 GIF 请求型 Skills

这里的“原生”指请求接口直接返回 GIF。已核对下面的请求示例明确选择 GIF 格式；**未执行请求，不等于本库已经测通**。服务商参数只适用于对应服务，不能直接照搬为 OpenAI 官方 API 参数。

### 1. gpt-image-gif：先做一张循环动图

[原安装说明](https://github.com/vargHQ/skills/blob/72e8109188e3366ba8d365902a84d6b237dec1d7/gpt-image-gif/README.md) · [完整 Skill](https://github.com/vargHQ/skills/blob/72e8109188e3366ba8d365902a84d6b237dec1d7/gpt-image-gif/SKILL.md)

- **适合什么：** 把角色、吉祥物、标志或文字描述做成一张循环 GIF，再转成网页用 WebP、展示用 MP4。
- **需要准备：** 支持 Agent Skills 的客户端；varg 账户及其 API Key 或 MCP 连接。生成使用第三方付费服务；后处理需要 FFmpeg/ffprobe，WebP 编码另需相应支持。
- **核到哪一步：** [Skill 的请求代码块](https://github.com/vargHQ/skills/blob/72e8109188e3366ba8d365902a84d6b237dec1d7/gpt-image-gif/SKILL.md#2-workflow-approve-a-still-first)明确使用 `model: gpt_image_2_6` 和 `provider_options.fal.output_format: gif`，参考图放在 `files`；[gif2web.sh](https://github.com/vargHQ/skills/blob/72e8109188e3366ba8d365902a84d6b237dec1d7/gpt-image-gif/scripts/gif2web.sh)读取已有 GIF 转码，不负责生成动作。
- **到哪里结束：** GIF 与展示格式导出；没有微信投稿或自动提交功能。作者给出的成品和测试记录属于作者报告。
- **许可：** [MIT](https://github.com/vargHQ/skills/blob/72e8109188e3366ba8d365902a84d6b237dec1d7/LICENSE)。

### 2. gpt-image-sticker-pack：同一角色做一组，再适配平台

[原安装说明](https://github.com/vargHQ/skills/blob/72e8109188e3366ba8d365902a84d6b237dec1d7/gpt-image-sticker-pack/README.md) · [完整 Skill](https://github.com/vargHQ/skills/blob/72e8109188e3366ba8d365902a84d6b237dec1d7/gpt-image-sticker-pack/SKILL.md)

- **适合什么：** 先确认角色母版，每种情绪生成一个 GIF，再导出微信、Telegram、WhatsApp、LINE、Discord、Slack 等平台所需的文件。
- **需要准备：** 与上一项相同的 varg 付费生成入口；本地导出需要 Bash、FFmpeg/ffprobe、ImageMagick 7，Gifsicle 为可选优化工具。Windows 使用者须另备兼容的 Bash 环境。
- **核到哪一步：** [Skill](https://github.com/vargHQ/skills/blob/72e8109188e3366ba8d365902a84d6b237dec1d7/gpt-image-sticker-pack/SKILL.md)中的请求明确选 `output_format: gif`；[export.sh](https://github.com/vargHQ/skills/blob/72e8109188e3366ba8d365902a84d6b237dec1d7/gpt-image-sticker-pack/scripts/export.sh)的 `wechat()` 读取已有 GIF，缩放、减色并导出 GIF、封面和聊天图标，进行文件技术检查。
- **到哪里结束：** 生成指导、部分投稿素材导出、人工上传说明。脚本没有自动提交微信，也不补齐专辑所有运营素材。它内置的尺寸、体积与数量说明须按[当前微信入口](wechat.md)复核，脚本 PASS 不表示审核通过。
- **许可：** [MIT](https://github.com/vargHQ/skills/blob/72e8109188e3366ba8d365902a84d6b237dec1d7/LICENSE)。

### 3. higgsfield-generate：已有 Higgsfield 账户时使用

[原安装说明](https://github.com/higgsfield-ai/skills/blob/27000402070db19d958789d05b3b52b6f4718d7c/INSTALL.md) · [完整 Skill](https://github.com/higgsfield-ai/skills/blob/27000402070db19d958789d05b3b52b6f4718d7c/higgsfield-generate/SKILL.md) · [GIF 命令示例](https://github.com/higgsfield-ai/skills/blob/27000402070db19d958789d05b3b52b6f4718d7c/higgsfield-generate/references/model-catalog.md)

- **适合什么：** 在统一的生成客户端中请求单张原生 GIF；它是综合生成 Skill，不是微信表情专用工厂。
- **需要准备：** 支持 Skills 的客户端、Higgsfield CLI、已登录且具有可用额度的 Higgsfield 账户。原安装流程还会处理 CLI 和认证。
- **核到哪一步：** 官方 Skill 的命令示例明确使用 `higgsfield generate create gpt_image_2_6` 与 `--output_format gif`，还列有帧数、帧时长和尺寸参数。这里核对的是命令示例；[CLI 公开仓库的所核版本](https://github.com/higgsfield-ai/cli/tree/fd21e7cb550b5835cc00c6b4abfea0c02fe77ff2)只有文档、许可和安装入口，不能据此称已审计 CLI 内部或生成服务。
- **到哪里结束：** 等待任务并交付生成结果链接；未发现本 Skill 的微信专辑适配、投稿或自动提交实现。
- **许可：** Skill 为 [MIT](https://github.com/higgsfield-ai/skills/blob/27000402070db19d958789d05b3b52b6f4718d7c/LICENSE)；服务使用和素材权利另按实际条款处理。

### 4. Sogni Creative Agent：已有 Sogni 生成环境时使用

[原安装说明](https://github.com/Sogni-AI/sogni-creative-agent-skill/blob/864b74113b96a4dd18dbd3eb0125ba3e299820c2/README.md) · [完整 Skill](https://github.com/Sogni-AI/sogni-creative-agent-skill/blob/864b74113b96a4dd18dbd3eb0125ba3e299820c2/SKILL.md) · [GIF 模型说明](https://github.com/Sogni-AI/sogni-creative-agent-skill/blob/864b74113b96a4dd18dbd3eb0125ba3e299820c2/references/models.md)

- **适合什么：** 通过 Sogni 的 CLI 请求 Image 2.6 GIF，并明确帧数和节奏。它是综合创作 Skill，没有专门的微信投稿流程。
- **需要准备：** Node.js ≥22.11.0、Sogni API Key 及可用服务额度。支持 Windows、macOS、Linux；本地转码等附加功能另需 FFmpeg/ffprobe。服务生成会消耗账户用量。
- **核到哪一步：** 固定版本 `864b74113b96a4dd18dbd3eb0125ba3e299820c2` 的模型说明明确使用 `gpt-image-2.6-flare` / `gpt-image-2.6-sunburst` 和 `--output-format gif`，并列出 `--image-frame-count`、`--image-frame-duration-ms`。这些是 **Sogni CLI 的封装选项**，不代表 OpenAI 或其他服务的参数、默认值与范围；没有发起生成请求。
- **到哪里结束：** GIF 请求与文件交付。仓库中的 Loop Maker 使用 LTX 等视频路线，是另一项工作流；不要把它与本条 GIF 请求混用计数。
- **许可：** [MIT](https://github.com/Sogni-AI/sogni-creative-agent-skill/blob/864b74113b96a4dd18dbd3eb0125ba3e299820c2/LICENSE)；服务条款和参考素材权利另核。

### 5. Frevana Flare / Sunburst：两个独立的 GIF 请求 Skill

[原仓库说明](https://github.com/FinpeakInc/frevana-skills/blob/7952e54fe1ec45e571898ee77b83612054159bbd/README.md) · [Flare Skill](https://github.com/FinpeakInc/frevana-skills/blob/7952e54fe1ec45e571898ee77b83612054159bbd/skills/gpt-image-2-6-flare/SKILL.md) · [Sunburst Skill](https://github.com/FinpeakInc/frevana-skills/blob/7952e54fe1ec45e571898ee77b83612054159bbd/skills/gpt-image-2-6-sunburst/SKILL.md)

- **适合什么：** 已使用 Frevana 的用户选择固定的 Flare 或 Sunburst 请求入口。不是微信专用表情包工具。
- **需要准备：** Bash、curl、Python 3、`FREVANA_TOKEN`，以及服务端的模型支持和可用额度。Windows 需要兼容的 Bash 环境；生成会使用第三方服务账户。
- **核到哪一步：** 固定版本 `7952e54fe1ec45e571898ee77b83612054159bbd` 的两个 Skill 和[Flare 请求脚本](https://github.com/FinpeakInc/frevana-skills/blob/7952e54fe1ec45e571898ee77b83612054159bbd/skills/gpt-image-2-6-flare/scripts/generate_image.sh)明确经 **Frevana 的 `/openai/image/generate`** 发送 `gif` 输出请求。文档要求 GIF 使用 `size auto` 等兼容设置，并保留原始错误。当前封装的 GIF 分支仅文生，不接受参考图、mask 或透明背景；这不代表其他入口的能力限制。
- **到哪里结束：** 返回 JSON 和托管 GIF 链接；没有微信配套素材、投稿或自动上架。文档的生产日志配置是作者报告，本库未验证服务部署、实际扣费或 GIF 文件。
- **许可：** 固定版本的递归文件树未找到 LICENSE，GitHub API 也未识别开放许可。这里只提供原文链接，不按 MIT 或本库许可复制其代码。

## 静态素材合成、收尾与交付 Skills

这些项目可以拿来处理素材和组织流程，但所核代码走静态图集、动作帧或图层形变，**不算 Image 2.6 原生 GIF 请求实现**。

| Skill 与原安装入口 | 可以拿来做什么 | 准备条件、源码依据与限制 | 许可 |
|---|---|---|---|
| **[pixel-gif-sticker-pack / Levi 卧云](https://github.com/WoYun520/pixel-gif-sticker-pack/blob/a4559f8aa8bcdec352f98b621d7500c913da1b6b/README.md#怎么用)** | 角色参考、批量中文表情、GIF/ZIP/播放预览，区分轻动效和完整动作 | 需要能生图和运行脚本的 Codex，Python/Pillow、中文字体；视频预览另需 FFmpeg。[Skill](https://github.com/WoYun520/pixel-gif-sticker-pack/blob/a4559f8aa8bcdec352f98b621d7500c913da1b6b/SKILL.md)要求生成 atlas；[export_pack.py](https://github.com/WoYun520/pixel-gif-sticker-pack/blob/a4559f8aa8bcdec352f98b621d7500c913da1b6b/scripts/export_pack.py)裁切后施加运动，[export_keyframes.py](https://github.com/WoYun520/pixel-gif-sticker-pack/blob/a4559f8aa8bcdec352f98b621d7500c913da1b6b/scripts/export_keyframes.py)合成连续姿势。默认聊天输出不代表微信投稿规格；未见自动提交 | [MIT](https://github.com/WoYun520/pixel-gif-sticker-pack/blob/a4559f8aa8bcdec352f98b621d7500c913da1b6b/LICENSE)，示例中的字体、配乐及角色权利分别核对 |
| **[vane-portrait-gif-stickers / 不叫韦恩](https://github.com/VaneAi888/vane-portrait-gif-stickers/blob/d83ee786a4aa72d5229f88247d2da44855182360/README.md#使用教程)** | 照片转 Q 版角色、按主题制作中文表情，导出透明 GIF、ZIP 和预览 | 需要图像生成助手、Python/Pillow、字体，MP4 预览另需 FFmpeg。[Skill](https://github.com/VaneAi888/vane-portrait-gif-stickers/blob/d83ee786a4aa72d5229f88247d2da44855182360/SKILL.md)和[导出器](https://github.com/VaneAi888/vane-portrait-gif-stickers/blob/d83ee786a4aa72d5229f88247d2da44855182360/scripts/export_pack.py)明确是静态图层位移、缩放、形变，不生成逐帧手脚动作。原帖说“已经上传微信”，不是审核通过证据 | [MIT](https://github.com/VaneAi888/vane-portrait-gif-stickers/blob/d83ee786a4aa72d5229f88247d2da44855182360/LICENSE)，保留[WoYun 导出器声明](https://github.com/VaneAi888/vane-portrait-gif-stickers/blob/d83ee786a4aa72d5229f88247d2da44855182360/references/third-party-LICENSE) |
| **[ray-sticker-shop](https://github.com/imraywang/ray-sticker-shop/blob/d274a8831b73a9f41504c66d330ca90119582119/README.md#安装)** | 角色设计、合成 GIF、投稿素材组织、上架文案与客户交付包 | Python 3.9+/Pillow；API 模式需要 Key，无 Key 可手动生成素材再交给脚本。[Skill](https://github.com/imraywang/ray-sticker-shop/blob/d274a8831b73a9f41504c66d330ca90119582119/SKILL.md)虽然写 2.6，[sticker.py](https://github.com/imraywang/ray-sticker-shop/blob/d274a8831b73a9f41504c66d330ca90119582119/scripts/sticker.py)实际请求 4×4 静态精灵图，再切帧编码。Skill 明确不代注册和提交；其成本及规格不当作本库实测 | [MIT](https://github.com/imraywang/ray-sticker-shop/blob/d274a8831b73a9f41504c66d330ca90119582119/LICENSE) |
| **[kim-sticker-pack / 老金](https://github.com/KimYx0207/Kim_Service/blob/aceed1895f61cc4681cabb41b1afe6911c9d8a58/skills/kim-sticker-pack/README.md)** | 角色与样片确认、动作素材整理、中文文字设计、GIF 收尾与交付验收 | 宿主需具备相应生图/播放能力；本地收尾用 Python 3.10+、Pillow、fontTools 和字体。[Skill](https://github.com/KimYx0207/Kim_Service/blob/aceed1895f61cc4681cabb41b1afe6911c9d8a58/skills/kim-sticker-pack/SKILL.md)要求先有真实连续动作帧；[finish_frames.py](https://github.com/KimYx0207/Kim_Service/blob/aceed1895f61cc4681cabb41b1afe6911c9d8a58/skills/kim-sticker-pack/scripts/finish_frames.py)只接收静态 PNG 帧，明确不生成运动。不是完整自动生成或投稿系统 | Skill 目录内 [MIT](https://github.com/KimYx0207/Kim_Service/blob/aceed1895f61cc4681cabb41b1afe6911c9d8a58/skills/kim-sticker-pack/LICENSE) |

## 从 X 教程找到的原项目

### 半格 · wechat-sticker-pack

默认交付 9 个独立循环 GIF 和一份动态九宫格总览。Skill 依赖宿主的图像与动图工具，可按宿主能力直接生成或从连续关键帧制作。微信投稿规格处理和提交需另行完成。仓库含 Skill 与分类菜单，采用 MIT 许可。 [安装说明](https://github.com/ban-ge/wechat-sticker-pack/blob/29656dae1d8024312a5f26bbbe3c8b8d1472613f/README.md) · [Skill](https://github.com/ban-ge/wechat-sticker-pack/blob/29656dae1d8024312a5f26bbbe3c8b8d1472613f/SKILL.md) · [许可](https://github.com/ban-ge/wechat-sticker-pack/blob/29656dae1d8024312a5f26bbbe3c8b8d1472613f/LICENSE) · [作者发布帖](https://x.com/ai_bange/status/2118740802545574019)

- [Levi 卧云原帖](https://x.com/Leviwoyun/status/2118197971112366538)关联 `WoYun520/pixel-gif-sticker-pack`。原帖展示与开源说明可以核对；“拿去上架”不等于已成交或已审核。
- [往事随风原帖](https://x.com/bywind_art/status/2118633386445066345)明确指向 `ray-sticker-shop`，补充了 ChatGPT 网页端上传 Skill 文档的用法。这是作者使用报告，不是本库重现实验。
- [不叫韦恩原帖](https://x.com/VaneAILab/status/2118367371643719978)关联 `VaneAi888/vane-portrait-gif-stickers`。原帖所说上传微信和市场报价，与源码支持范围分开看。

上述 X 正文已通过公开阅读器读到，未据文字摘要核验视频、截图中的上传状态或金额。其余种子中的教程、提示词库和经营观点归入对应资料页；`Punk-IP` 是静态文章配图 Skill，`Evolink` 是提示词/API 资料库，均不冒充 GIF Skill。安装成功、生成文件、技术检查和平台审核是四件不同的事。
