# IP Picture Workshop — Agent Skill for Photo-Based IP Carousels

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE) [![GitHub stars](https://img.shields.io/github/stars/masonmosen/ip-picture-workshop.svg)](https://github.com/masonmosen/ip-picture-workshop/stargazers)

**Photo to character. Text to illustrated carousel.** Create a recognizable personal character and turn articles, notes, stories, or scripts into cohesive social-media image cards.

**一张照片，一段文字，变成有你专属角色的多页图文。**

An AI Skill for Codex: it builds a personal IP character in different styles from a photo, reads an article, note, story, or script, and generates a series of illustrated image cards with text. Works for Xiaohongshu carousels, WeChat article art, knowledge cards, and personal-brand content.

## Demo

> **Demo uses a fictional character, no photo input.** The demo below was generated from a text-only description of a fictional creator “小满” (Xiao Man) — round glasses, freckles, beige sweater — not from any real person's photo. With a real photo, the same skill builds the character from that photo instead.
>
> **Demo 说明：虚拟角色，无照片输入。** 下面的 Demo 用纯文字描述的虚拟博主“小满”（圆框眼镜、雀斑、米白毛衣）生成，没有用任何真人照片；有照片时，技能会按照片定制角色。

![Demo collage: 3-page carousel of fictional creator Xiao Man](docs/demo/05-collage-3pages.jpg)

Demo: 1 style sheet + 3 pages, 3:4, Codex built-in imagegen. [Style sheet](docs/demo/01-style-sheet.png) · [Page 1](docs/demo/02-page1.png) · [Page 2](docs/demo/03-page2.png) · [Page 3](docs/demo/04-page3.png)

## Install

```bash
npx skills add https://github.com/masonmosen/ip-picture-workshop --skill ip-picture-workshop
```

## What you get

- **Custom character**: build one recognizable IP character in several styles and expressions, then pick your favorite.
- **One input, many pages**: the skill plans cover, highlights, visuals, and reading order from your text.
- **Complete illustrated pages**: character, scene, and text generated together — no layout or prompt craft needed.
- **Single-page redo**: point at a page and say what to change; the rest stays.
- **Reuse across posts**: save the chosen character reference and keep the same look in the next piece.

## 它能帮你做什么？

- **定制专属角色**：基于人物形象生成多个风格和表情，让你选择喜欢的一种。
- **一次输入，多页表达**：AI 分析文字，自行规划封面、重点、画面和阅读顺序。
- **直接生成完整图片**：角色、场景和文字一起生成；无需自己设计版式或写复杂提示词。
- **不满意就重做单页**：指出页码和修改方向，其他页面保留。
- **跨内容复用**：保存选定的角色参考图，下一篇继续使用，逐步形成统一视觉形象。

无论你想把**文章转小红书图文**、把**公众号长文变成漫画配图**，还是把一段想法做成**个人 IP 知识卡片**，都可以从这里开始。

## 三步开始

1. 提供一张照片，或直接描述你想要的角色形象。
2. 选择喜欢的 IP 风格；如果已有角色参考图，可以直接提供。
3. 提供文章、文字、文件或可访问的链接。AI 会拆解内容并生成多页图片。

> 人物长相和辨识度优先。照片里的包、包带等偶然配件默认不会被当作人物特征；服装可以明确指定。

## 使用示例

```text
用 $ip-picture-workshop 把我这张照片做成三种 IP 角色风格。
```

```text
用我选好的角色，把下面这篇关于培养阅读习惯的文章做成小红书多页图文。
```

```text
第 4 页标题太小，请只重新生成这一页，其他页面保持不变。
```

无需提前准备长篇提示词；你可以直接用自己的语言说明想法。

## 安装与使用

把仓库完整的 Skill 文件夹安装到 Codex 可发现的 skills 目录，或在支持 Agent Skills 的环境中按其安装方式使用。使用时调用 `$ip-picture-workshop`，并确保当前环境提供可用的图像生成工具；在 Codex 中优先使用内置 imagegen。具体工具可用性、账号额度及生成时间由运行环境决定。

```bash
npx skills add https://github.com/masonmosen/ip-picture-workshop --skill ip-picture-workshop
```

安装完成后，如当前会话未发现新 Skill，请重新打开会话并确认其已加载。命令来自 skills CLI 生态；不同客户端的安装目录与发现规则可能不同，首次使用请核对本机配置。

## 适合谁？

- 希望用统一人物形象经营个人品牌的创作者
- 希望把公众号、长文或知识笔记变成系列配图的作者
- 想为小红书、社交媒体制作漫画图文的个人或 OPC 团队
- 想用同一角色讲解知识、观点、故事和教程的内容团队

## 使用边界

- 它是 **Skill 工作流程**，不是独立网站、插件托管服务或自动发布工具。运行它需要支持相应 Skill 和生图能力的 Agent 环境。
- 支持粘贴的文字、可读取文件和可访问链接；遇到无法读取的链接，会请你粘贴正文或提供文件。
- 生成结果需要人工检查人物、文字和原文含义；跨页一致性、生成速度、文字准确率与费用取决于工具和任务，无法保证每次完全一致或零错误。
- 角色图、文章和输出默认用于当前任务；复用时请保留自己的角色参考图。不要将他人照片或没有权限公开的材料上传至公开仓库。
- 本项目公开的是工作流程，不附带示例中的真实人物照片、角色、文章或成品，也不会自动发布你的内容。

## 本次验证状态

在一次实际创作中，先用用户提供的照片生成三个角色风格，用户选择后移除偶然配件，再将一篇文章制作成 8 张带文字的 3:4 图文。图片完成了文件和视觉检查，创作者给予正面反馈。该记录证明一次实际工作流体验，不代表封装后的 Skill 已在其他机器、其他 Agent 或所有文章中独立验证。

## 来源与许可

本项目由 Mason OPC 根据真实创作需求独立编写；工作流程研究时参考了 [YouMind 公众号长文一键转漫画贴图](https://youmind.com/~skills/01a18d41-91d8-7f81-8b15-44bae30f496e) 的公开说明及可见交互，也参考了公开图文工作流思路。未复制其私有提示词或服务端代码。本项目以 MIT License 发布；第三方服务和生图工具各自的条款与费用另行适用。

---

## More from MOSEN

- [muse-video-prompt-skill](https://github.com/masonmosen/muse-video-prompt-skill) — Prompt engineering workflow for Muse built-in video generation.
- [mason-opc-motion-video](https://github.com/masonmosen/mason-opc-motion-video) — Talking-head video + script → editable motion-graphics video.
- [mosen-ad-studio](https://github.com/masonmosen/mosen-ad-studio) — Brand ads & product promos made entirely as code.
- [remake-depth-breakdown](https://github.com/masonmosen/remake-depth-breakdown) — Reference video → depth video + Seedance-ready prompts.
- [cueshot-starter-skills](https://github.com/masonmosen/cueshot-starter-skills) — Free starter skills for AI video shot planning & review.
- [reference-video-blueprint](https://github.com/masonmosen/reference-video-blueprint) — Authorized reference video → original Prompt Contract.
