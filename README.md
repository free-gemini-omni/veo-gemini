[Official Website](https://freegeminiomni.com) · [Live Demo on Hugging Face](https://huggingface.co/spaces/gemini-omni/veo-gemini)

---

<div align="center">

<img src="https://freegeminiomni.com/og.png" alt="Free Gemini Omni — multimodal AI video and image creation platform" width="100%" />

# Free Gemini Omni

**Create, remix, and refine AI videos and images with text, image, audio, and video references.**

An all-in-one, browser-based creative workspace for creators, marketers, educators, developers, and teams.

[Website](https://freegeminiomni.com/) · [Start Creating](https://freegeminiomni.com/generator) · [Documentation](https://freegeminiomni.com/docs) · [Prompt Gallery](https://freegeminiomni.com/prompts) · [Pricing](https://freegeminiomni.com/pricing)

[English](#english) · [简体中文](#中文)

</div>

<a id="english"></a>

## About Free Gemini Omni

Free Gemini Omni, also known as **Free Omni**, is a multimodal AI creation platform built to turn ideas and reference assets into publishable videos and images. It brings text prompts, images, audio cues, existing video clips, generation models, task tracking, and iterative editing together in one browser workflow—without requiring a heavyweight desktop editing suite.

Traditional generators often start and end with a text box. Free Gemini Omni is designed around a broader, reference-driven workflow:

- **Text** defines the subject, action, setting, composition, camera language, lighting, mood, and pacing.
- **Images** help establish characters, products, environments, keyframes, and visual direction.
- **Audio** can provide dialogue, music, rhythm, atmosphere, or emotional guidance when supported by the selected model.
- **Video** can communicate movement, performance, camera behavior, timing, or an existing scene to remix.

From a first prompt to a finished clip, users can select a model, configure supported inputs, review estimated credit usage, submit a task, follow its progress, and manage previous generations from the same online studio.

> **Independent product notice:** Free Gemini Omni is an independent product and is not affiliated with, endorsed by, or sponsored by Google or any model provider. Product names and model names are used only to describe supported or documented workflows. Model availability, features, pricing, and output capabilities may change and should be confirmed on the live website.

## What You Can Create

| Creative goal | Example outputs |
| --- | --- |
| Product marketing | Motion ads, launch videos, product demonstrations, campaign variants, and social hooks |
| Social content | TikTok videos, YouTube Shorts, Instagram Reels, vertical stories, and reusable content concepts |
| Cinematic storytelling | Short scenes, mood films, story remixes, character moments, and pre-production concepts |
| Education and onboarding | Explainers, visual lessons, product walkthroughs, and training content |
| Brand content | Consistent product visuals, character-led series, seasonal campaigns, and style explorations |
| Music and performance | Rhythm-led clips, performance references, dance concepts, and music-video ideas |
| Product development | AI media features for apps, automated generation pipelines, and SaaS integrations |

## Core Capabilities

### Multimodal generation

- Generate short-form video from natural-language prompts.
- Animate product photos, character artwork, concept frames, and other still images.
- Combine multiple reference types when the selected model supports them.
- Create supporting images for characters, products, environments, storyboards, and later video generation.
- Choose from multiple video and image workflows through a unified model catalog.

### Video remixing and conversational editing

- Bring an existing clip into the workflow and describe the desired change in plain language.
- Adjust a scene's pacing, background, subject, composition, camera direction, or visual style.
- Use reference motion to communicate camera moves, choreography, performance, or timing.
- Iterate through prompt changes instead of rebuilding an edit from scratch.

### A unified online studio

- Browse video and image models by category and capability.
- See model-specific fields only when they are relevant to the selected workflow.
- Review estimated credit usage before submitting supported jobs.
- Track queued, running, succeeded, and failed tasks.
- Revisit prompts, settings, visibility, generated media, and downloadable results in generation history.
- Create from a responsive browser interface without installing professional editing software.

### Prompt and learning resources

The [Prompt Gallery](https://freegeminiomni.com/prompts) provides reusable examples across text-to-video, image-to-video, video-to-video, storyboarding, camera direction, action, text rendering, cross-modal generation, visual effects, and other creative patterns. Product guides and documentation help users move from experimentation to repeatable workflows.

### Developer API

Developers can bring the same generation workflow into an application or automation. After creating an API key in the dashboard, clients can submit a generation request, poll task status, read generation history, and manage usage through the same account and credit system used by the web studio.

```bash
curl -X POST "https://freegeminiomni.com/api/ai-studio/execute" \
  -H "Authorization: Bearer YOUR_API_KEY" \
  -H "Content-Type: application/json" \
  -d '{
    "modelId": "YOUR_MODEL_ID",
    "isPublic": false,
    "payload": {
      "prompt": "A cinematic product launch video",
      "duration": 5,
      "resolution": "720p"
    }
  }'
```

When the request returns a task ID, query the task endpoint until the job reaches a terminal state:

```bash
curl "https://freegeminiomni.com/api/ai-studio/tasks/YOUR_TASK_ID" \
  -H "Authorization: Bearer YOUR_API_KEY"
```

The exact `modelId`, payload fields, accepted media types, duration, resolution, and credit cost depend on the selected model. See the [API documentation](https://freegeminiomni.com/docs/api) for the current contract.

## How the Workflow Fits Together

1. **Choose a workflow** — Start with text-to-video, image-to-video, remixing, image generation, or another available model flow.
2. **Prepare the references** — Write a structured prompt and add the images, audio, or video required by the selected model.
3. **Configure the output** — Select supported settings such as aspect ratio, duration, resolution, or visibility.
4. **Review usage** — Check the estimated credit cost and available account balance before submission.
5. **Generate and track** — Submit the task and follow it through queued, running, succeeded, or failed states.
6. **Review and iterate** — Preview or download the result, reuse the prompt, and refine motion, framing, style, timing, or narrative direction.

## Built for Different Teams

### Creators

Move from an idea, script, or reference image to short-form video concepts quickly. Explore multiple directions without switching between separate tools for generation, prompting, and result management.

### Marketing and brand teams

Prototype product ads, campaign hooks, visual variations, and social assets before committing to a full production cycle. Reference-driven workflows make it easier to communicate a specific product, character, composition, or visual language.

### Educators and product teams

Turn lessons, onboarding flows, product messages, and abstract concepts into visual explanations. Use iteration to test different levels of detail, pacing, and tone.

### Developers and SaaS teams

Use documented endpoints, API-key authentication, asynchronous task tracking, and generation history to integrate AI video and image creation into applications and automated workflows.

## Product Ecosystem

Free Gemini Omni combines the creative workspace with the supporting systems needed for ongoing production:

- **Accounts and access** — Authentication, user settings, API keys, and account management.
- **Credits and plans** — Credit-based rendering, subscriptions, one-time credit packages, orders, and usage records.
- **Generation history** — Centralized task status, prompts, configurations, outputs, and downloads.
- **Content resources** — Prompt examples, model guides, comparisons, use cases, and articles.
- **Developer tooling** — Model discovery, generation requests, task-status queries, history, and API documentation.
- **International experience** — Product content and interfaces for English, Simplified Chinese, and Japanese users.

## What This GitHub Organization Represents

This organization is the engineering and open collaboration home for the Free Gemini Omni ecosystem. Repositories may include product applications, shared components, developer examples, documentation, integrations, operational tooling, and experiments that make multimodal creation more accessible.

Our focus is practical: reduce the distance between a creative idea and a usable result, provide one consistent workflow across models, and give both creators and developers enough control to build repeatable AI media processes.

## Quick Links

- [Free Gemini Omni website](https://freegeminiomni.com/)
- [AI creation studio](https://freegeminiomni.com/generator)
- [Prompt gallery](https://freegeminiomni.com/prompts)
- [Product and API documentation](https://freegeminiomni.com/docs)
- [API overview](https://freegeminiomni.com/docs/api)
- [Plans and credits](https://freegeminiomni.com/pricing)
- [Contact support](mailto:support@freegeminiomni.com)

---

<a id="中文"></a>

## 关于 Free Gemini Omni

Free Gemini Omni，也称 **Free Omni**，是一个多模态 AI 视频与图像创作平台，帮助用户把创意和参考素材快速转化为可发布的视觉内容。平台将文字提示词、图片、音频、现有视频、生成模型、任务跟踪与多轮迭代整合到同一个浏览器工作流中，无需安装大型专业剪辑软件。

与只提供文本输入框的传统生成器不同，Free Gemini Omni 更强调“参考素材驱动”的创作方式：

- **文字**用于描述主体、动作、环境、构图、镜头语言、光线、情绪与节奏。
- **图片**用于确定角色、商品、环境、关键帧与整体视觉方向。
- **音频**可在模型支持时提供对白、音乐、节拍、氛围或情绪参考。
- **视频**可用于表达运动、表演、运镜、时间节奏，或作为需要混剪和改编的原始场景。

从第一条提示词到最终成片，用户可以在同一个在线工作台中选择模型、配置输入、查看预计积分、提交生成任务、跟踪运行状态并管理历史结果。

> **独立产品声明：** Free Gemini Omni 是独立产品，与 Google 或任何模型提供商不存在隶属、授权、背书或赞助关系。产品名称和模型名称仅用于说明平台所支持或介绍的工作流。模型可用性、功能、价格与输出能力可能变化，请以线上页面为准。

## 可以创作什么

| 创作目标 | 示例内容 |
| --- | --- |
| 产品营销 | 商品动态广告、发布视频、产品演示、Campaign 变体与社媒开场钩子 |
| 社交内容 | TikTok、YouTube Shorts、Instagram Reels、竖屏故事与系列内容创意 |
| 电影感叙事 | 剧情短片、氛围视频、故事混剪、角色片段与前期概念预演 |
| 教育与入门 | 教学解说、知识可视化、产品教程与培训内容 |
| 品牌内容 | 风格统一的商品视觉、角色系列、节日活动与视觉方向探索 |
| 音乐与表演 | 节奏驱动短片、表演参考、舞蹈概念与音乐视频创意 |
| 产品开发 | 应用内 AI 媒体功能、自动化生成流程与 SaaS 集成 |

## 核心能力

### 多模态内容生成

- 使用自然语言提示词生成短视频。
- 让商品照片、角色设定、概念图和其他静态画面产生运动。
- 在所选模型支持时组合多种参考素材。
- 生成角色、商品、环境、分镜等图片，为后续视频创作准备素材。
- 通过统一的模型目录选择不同的视频与图像工作流。

### 视频混剪与对话式编辑

- 上传现有视频，并用自然语言描述希望做出的改变。
- 调整场景节奏、背景、主体、构图、运镜或视觉风格。
- 使用参考运动表达镜头移动、舞蹈动作、人物表演或时间节奏。
- 通过持续修改提示词完成迭代，无需每次从零开始制作。

### 统一的在线工作台

- 按类别和能力浏览视频或图像模型。
- 根据当前模型动态显示真正需要的输入字段。
- 在提交支持的任务前查看预计积分消耗。
- 跟踪排队、运行、成功和失败等任务状态。
- 在生成历史中查看提示词、参数、公开范围、生成内容与下载结果。
- 直接在响应式网页中完成创作，无需安装专业剪辑软件。

### 提示词与学习资源

[提示词库](https://freegeminiomni.com/zh/prompts)提供文本生成视频、图片生成视频、视频改编、故事板、镜头控制、动作、文字渲染、跨模态生成、视觉特效等不同方向的可复用示例。产品指南与文档帮助用户把单次尝试沉淀成可重复的创作流程。

### 开发者 API

开发者可以把与网页工作台一致的生成能力接入应用或自动化流程。在仪表盘创建 API Key 后，即可提交生成任务、轮询任务状态、读取生成历史，并使用与网页端统一的账号和积分体系管理用量。

```bash
curl -X POST "https://freegeminiomni.com/api/ai-studio/execute" \
  -H "Authorization: Bearer YOUR_API_KEY" \
  -H "Content-Type: application/json" \
  -d '{
    "modelId": "YOUR_MODEL_ID",
    "isPublic": false,
    "payload": {
      "prompt": "A cinematic product launch video",
      "duration": 5,
      "resolution": "720p"
    }
  }'
```

接口返回任务 ID 后，可通过任务查询接口持续读取状态：

```bash
curl "https://freegeminiomni.com/api/ai-studio/tasks/YOUR_TASK_ID" \
  -H "Authorization: Bearer YOUR_API_KEY"
```

实际使用的 `modelId`、`payload` 字段、素材类型、时长、分辨率和积分消耗取决于所选模型，请以最新的 [API 文档](https://freegeminiomni.com/docs/api)为准。

## 完整创作流程

1. **选择工作流** — 从文本生成视频、图片生成视频、视频混剪、图片生成或其他可用模型流程开始。
2. **准备参考素材** — 编写结构化提示词，并按模型要求添加图片、音频或视频。
3. **配置输出** — 选择模型支持的画幅、时长、分辨率和公开范围等参数。
4. **确认用量** — 提交前查看预计积分消耗和当前账户余额。
5. **生成并跟踪** — 提交任务，持续查看排队、运行、成功或失败状态。
6. **查看并迭代** — 预览或下载结果，复用提示词，继续优化运动、取景、风格、节奏或叙事方向。

## 为不同用户和团队而设计

### 内容创作者

快速把想法、脚本或参考图片变成短视频概念，在同一个平台中完成生成、提示词迭代和结果管理，无需频繁切换工具。

### 营销与品牌团队

在进入完整制作周期前验证产品广告、营销钩子、视觉变体与社媒素材。参考素材驱动的工作流能够更准确地表达商品、角色、构图和视觉语言。

### 教育与产品团队

把课程、入门流程、产品信息和抽象概念转化为视觉解说，并通过多次迭代测试内容的细节程度、节奏与表达语气。

### 开发者与 SaaS 团队

通过文档化接口、API Key 认证、异步任务跟踪与生成历史，将 AI 视频和图像能力集成到应用及自动化工作流中。

## 产品生态

Free Gemini Omni 将创作工作台与持续生产所需的配套系统整合在一起：

- **账号与访问** — 身份验证、用户设置、API Key 与账号管理。
- **积分与套餐** — 积分制渲染、订阅、一次性积分包、订单与用量记录。
- **生成历史** — 集中管理任务状态、提示词、参数、生成结果与下载。
- **内容资源** — 提示词示例、模型指南、对比内容、使用场景与文章。
- **开发者能力** — 模型发现、生成请求、任务查询、历史记录与 API 文档。
- **国际化体验** — 面向英文、简体中文和日文用户的界面与内容。

## GitHub Organization 定位

这个 GitHub Organization 是 Free Gemini Omni 生态的工程与开放协作空间。相关仓库可用于承载产品应用、共享组件、开发示例、文档、集成、运营工具，以及让多模态创作更易用的实验项目。

我们的重点始终是实用性：缩短创意与可用成品之间的距离，以一致的体验连接不同模型，并为创作者和开发者提供足够的控制能力，帮助他们建立可重复的 AI 媒体工作流。

## 快速链接

- [Free Gemini Omni 官网](https://freegeminiomni.com/zh)
- [AI 创作工作台](https://freegeminiomni.com/zh/generator)
- [提示词库](https://freegeminiomni.com/zh/prompts)
- [产品与 API 文档](https://freegeminiomni.com/docs)
- [API 概览](https://freegeminiomni.com/docs/api)
- [套餐与积分](https://freegeminiomni.com/zh/pricing)
- [联系支持](mailto:support@freegeminiomni.com)

![Analytics](https://ga.smnzb.com/p/9zZ0eLD42)
