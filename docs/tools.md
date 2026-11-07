# 生成入口与 GIF 后处理工具

[返回首页](../README.md) · [原词与作者案例](prompts.md)

需要安装现成工作流时，直接查看[Skills 专区](skills.md)；作者发布与实操说明见[X 原帖目录](x-tutorials.md)。

精选与“原生 GIF → 微信适配”直接相关的入口或项目。原入口核查日期：2026-11-06；X案例库与Skills补充于2026-11-07。

## 先取得原生 GIF

| 入口 | 用在什么地方 | 取用前看什么 |
|---|---|---|
| [ChatGPT Images](https://help.openai.com/en/articles/11084440-images-in-chatgpt) | 上传静态参考图，要求生成会循环的 GIF；在对话中修改，打开后调速或保存 | 官方帮助注明 GIF 功能逐步推出，当前账号可用性仍需确认。不能编辑用户上传的已有动画 GIF |
| [OpenAI Image API](https://developers.openai.com/api/docs/guides/image-generation#generate-animated-gif-output) | 需要 API 的读者参考官方原生 GIF 请求；可使用静态参考图指导动画 | 当前官方正文支持 generations 与 edits 的 GIF 输出，参考图走 edits。与只输出静态图再切帧的代码区分；权限和计费另行确认 |

ChatGPT 订阅与 API 是不同入口。这里不推荐为复现某篇教程而购买中转服务，也不把工具名称、模型自述或文件扩展名当作动画已经成功的证据。

## 已有 GIF，再做适配

### Ezgif：浏览器里调整尺寸、速度与体积

[GIF 优化页面](https://ezgif.com/optimize)提供压缩、减色及调整速度，并链接缩放、裁切等操作。适合已有原生 GIF 后做适配，再回手机检查细节和循环。

当前页面有本地处理选项，注明部分功能受限；未在浏览器本地提供的工具会把文件发送到服务器。处理真人或客户素材前，应按实际模式判断是否上传。它是文件处理网站，不是 Image 2.6 生成入口，也不会自动证明微信规格或内容审核合格。

### Gifsicle：本地检查和优化 GIF

[作者官网与手册](https://www.lcdf.org/gifsicle/) · [GitHub：kohler/gifsicle](https://github.com/kohler/gifsicle)

作者 Eddie Kohler 的项目可读取 GIF 信息、调整循环与调色板、优化动画体积；适合希望在本地处理已有文件的读者。其 [README](https://github.com/kohler/gifsicle/blob/master/README.md)说明了处理功能，源代码中的 [gifsicle.c](https://github.com/kohler/gifsicle/blob/master/src/gifsicle.c)是命令行处理入口。它不调用图像生成模型；项目虽也能合并帧，本路线只取其对已有 GIF 的检查、编辑与优化用途。

代码采用 GPL-2.0，README 另给可选许可条款，具体见[作者许可说明](https://github.com/kohler/gifsicle/blob/master/README.md#copyrightlicense)和 [COPYING](https://github.com/kohler/gifsicle/blob/master/COPYING)。使用程序处理图片，与再分发或修改其代码，应分别阅读相应条件。本页不提供未经验证的安装命令或微信参数预设。

## 找原词：保留来源的 GitHub 提示词库

### Awesome-GPT-Image-2.6-API-Prompts

[Anil-matcha 的仓库](https://github.com/Anil-matcha/Awesome-GPT-Image-2.6-API-Prompts) · [本库已署名摘录的 5 条原词](prompts.md#可直接复制5-条开放许可模板)

核查版本 `426032b613a85eef2936a226db2b0698ad698782` 的内容是 README 与 LICENSE，适合查阅提示词，不是可执行生成工具。GIF 区有 5 条模板，未附对应 GIF 成品或生成日志。其 [CC BY 4.0 声明](https://github.com/Anil-matcha/Awesome-GPT-Image-2.6-API-Prompts/blob/426032b613a85eef2936a226db2b0698ad698782/LICENSE)允许按署名等条件转载和改编。

仓库含 MuAPI 商业导流。所核 README 的“GIF 仅支持 generations”和“2–64 帧”与当前[官方 GIF 指南](https://developers.openai.com/api/docs/guides/image-generation#generate-animated-gif-output)不一致；本库只摘录提示词，不沿用它的 API 参数表。

### Awesome AI GIF Prompts

[ailingqu 的仓库](https://github.com/ailingqu/awesome-ai-gif-prompts) · [41 条分类原词入口](prompts.md#来源跳转41-条带示例的-gif-原提示)

固定版本 `2672b8fe04e75275de70a8d5d2992da6271ce8f5` 收录聊天贴纸、快闪、氛围循环与像素/UI四类，附英文原词、来源中文标题和作者生成的示例。采用 CC BY 4.0；本库整理目录并链接原文，没有逐项运行或复现。生成脚本使用第三方服务，代码配置不作为所有 Image 2.6 入口的通用设置。

## 其他资料库与 Skill 路线

另可参考已有的中英案例仓库 [zhuyansen/awesome-chatgpt-images-2.6](https://github.com/zhuyansen/awesome-chatgpt-images-2.6)及其[浏览页面](https://jasonzhu.ai/en/prompts/chatgpt-images-2-6)。它按原帖、作者、类别和提示词出处组织，未公开原词的作品留空。仓库未检测到通用开放许可，本库只提供链接，不复制其媒体和数据。

两个常见仓库的源码可以帮助辨认路线，但不符合本页的原生生成入口条件：

- **[ray-sticker-shop](https://github.com/imraywang/ray-sticker-shop)**：固定版本 [sticker.py](https://github.com/imraywang/ray-sticker-shop/blob/d274a8831b73a9f41504c66d330ca90119582119/scripts/sticker.py)中的 `_prompt_sheet` 要求 4×4 静态精灵图，随后切片并编码 GIF。README 提及 2.6，不能改变这段代码的实际路径。
- **[kim-sticker-pack](https://github.com/KimYx0207/Kim_Service/tree/main/skills/kim-sticker-pack)**：固定版本 [finish_frames.py](https://github.com/KimYx0207/Kim_Service/blob/aceed1895f61cc4681cabb41b1afe6911c9d8a58/skills/kim-sticker-pack/scripts/finish_frames.py)接收已有静态 PNG 动作帧，文件开头明确说明不生成运动。它是动作帧收尾工具，不能替代原生图转 GIF。

这两项不作为原生生成入口推荐。它们的流程、默认阈值和许可都不能替代当前微信官方规范。工具能导出动图、投稿技术检查通过、平台内容审核通过，是不同结果。
