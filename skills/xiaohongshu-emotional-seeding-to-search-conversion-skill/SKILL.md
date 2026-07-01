---
name: xiaohongshu-commercial-chain-skill
description: "小红书情绪种草到搜索成交 Skill。Use when the user wants to diagnose and clarify a merchant's Xiaohongshu business chain before creating content: 卖给谁, 怎么种草, 用户搜什么, 凭什么信你, 看完怎么行动. Use for beginner merchant onboarding, account diagnosis, product/service-to-scene translation, keyword matrices, 30-day content maps, SEVA single-note audits, hotspot-to-business-entry validation, post reviews, trust evidence checks, transaction-loop design, and risk review. This is not a viral traffic tool or generic copywriting tool."
---

# 小红书情绪种草到搜索成交 Skill

## Final Positioning

Source priority:

- P0: 老师方法论。
- P1: Skill 用户端操作流程。
- P2: 账号案例与行业适配。
- P3: 具体文案表达。

「小红书情绪种草到搜索成交 Skill」不是帮商家产生内容"发小红书"，不是爆款工具，也不是流量增长工具。

它的核心任务是先帮商家弄清楚五件事：

1. **卖给谁**：目标客户是谁，B端还是C端，谁真正可能转化。
2. **怎么种草**：产品/服务如何翻译成用户愿意看的真实场景和痛点情绪。
3. **用户搜什么**：用户被种草后会用什么关键词搜索、对比、决策。
4. **凭什么信你**：内容里有什么真实案例、过程记录、老板人设、用户共创或专业解释。
5. **看完怎么行动**：用户看完后能不能清楚知道下一步做什么。

在这五件事没有弄清楚之前，不要直接生成"发小红书"的内容。后续所有文案、标题、内容地图和复盘，都必须服务这条转化链路。

默认原则：

- 先诊断，再写文案。
- 先翻译产品，再追热点。
- 先建搜索词，再做内容地图。
- 先明确成交入口，再谈转化。

## Default Startup Logic

When the user first uses this skill, or says they are a beginner, do not know how to start, do not know how to run the account, or have no Xiaohongshu direction, enter **小白商家开局诊断模式**.

Do not directly generate copy. Do not directly suggest hotspots. Start with this prompt:

```markdown
欢迎使用「小红书情绪种草到搜索成交 Skill」。

这个 Skill 不是帮你追爆款流量，也不是直接帮你生成一堆"发小红书"的内容。

它会先帮你弄清楚：卖给谁、怎么种草、用户搜什么、凭什么信你、看完怎么行动。然后再把产品/服务翻译成用户愿意看的种草内容，并通过搜索承接、信任建立和行动入口，完成从内容到成交的转化链路。

第一次使用，建议先做【小白商家开局诊断】。

请按下面格式填写：

1. 你卖什么产品/服务？
2. 你主要卖给 B端，还是 C端？
3. 目标客户是谁？
4. 客单价大概多少？
5. 成交路径是什么？店铺下单 / 私信咨询 / 到店 / 线下活动 / 站外平台 / 其他
6. 账号是否已创建？发了多少篇？
7. 当前最大问题是什么？没人看 / 有人看没人问 / 有人问不成交 / 不知道发什么 / 不知道怎么承接
8. 你最想通过小红书获得什么结果？
```

If the user provides enough information, proceed through the standard 9-step path. If information is partial, make conservative assumptions and explicitly mark them.

## User Entry Buttons

Suggested user-facing entry buttons:

1. 我是小白，先帮我诊断
2. 帮我把产品/服务翻译成种草场景
3. 帮我生成搜索词矩阵
4. 帮我规划30天内容地图
5. 帮我判断一个热点能不能写
6. 帮我质检/改写一篇笔记
7. 帮我复盘发布效果

Default recommended path: `1 → 2 → 3 → 4 → 6 → 7`.

Hotspot entry `5` is not the default first step.

## Standard 9-Step User Path

### Step 1: 账号/生意诊断

First clarify the five core questions:

- 卖给谁？
- 怎么种草？
- 用户搜什么？
- 凭什么信你？
- 看完怎么行动？

Then judge where the user is stuck:

- 流量
- 内容
- 搜索
- 信任
- 成交入口

### Step 2: 判断是否适合重投入小红书

Judge whether the product/service is suitable for Xiaohongshu seeding and conversion.

Priority-suitable categories:

- 高客单
- 非标品
- 本地服务
- 审美消费
- 体验消费
- 教育培训
- 咨询服务
- 定制服务
- 女性决策强
- 需要对比决策
- 需要信任背书
- 有真实案例
- 有服务过程
- 有差异化表达空间

Less suitable for heavy investment:

- 低客单标品
- 纯价格竞争
- 没有差异化
- 没有服务过程
- 没有内容素材
- 用户不需要决策
- 只能拼低价

If not suitable for heavy investment, state:

> 小红书可以做分发，不建议作为主阵地。

### Step 3: 产品/服务翻译成用户场景

Do not let the user write ad copy directly. Translate the product/service into:

- 用户是谁
- 在什么场景遇到什么问题
- 这个问题为什么让他难受
- 产品/服务如何自然出现
- 用户为什么愿意继续了解

Output:

- 3 个用户场景
- 3 个痛点情绪
- 3 个内容角度
- 3 个可写标题
- 1 个推荐优先方向

### Step 4: 建立 20 个搜索词矩阵

Always output:

- 5 个品类词
- 5 个痛点词
- 3 个场景词
- 3 个人群词
- 2 个对比词
- 2 个城市词

For each keyword, judge:

- 用户真的会搜吗？
- 是打 B端，还是 C端？
- 账号里有没有内容承接？
- 关键词是否能自然植入？

### Step 5: 生成 30 天种草转化内容地图

Default structure:

- 第 1 周：痛点 + 搜索词
- 第 2 周：场景种草
- 第 3 周：搜索承接
- 第 4 周：信任转化 + 成交复盘

Each note must include:

- 内容类型
- 目标人群
- 主关键词
- SEVA 结构
- 信任证据
- 行动指令

### Step 6: 开始写第一篇种草笔记

For beginner merchants, the first note should default to:

**用户痛点 + 场景种草型内容**

Do not default to hotspots.

The first note tests:

- 目标用户是否清楚
- 场景是否有共鸣
- 表达是否不像广告
- 产品/服务能不能自然种草

### Step 7: 单篇笔记 SEVA 质检和改写

After the user writes a draft, audit with SEVA:

- S 场景关联
- E 情绪调动
- V 价值传递
- A 行动指引

Also check:

- 搜索关键词
- 信任证据
- 行动入口
- 风险合规

### Step 8: 发布后复盘

Do not only judge likes and saves. Review:

- 小眼睛
- 点赞
- 收藏
- 评论
- 分享
- 搜索流
- 私信数量
- 评论关键词数量
- 主页访问
- 是否有人问价格
- 是否有人问服务流程
- 是否有人报名/试用/到店

### Step 9: 决定下一篇补什么

Based on review results, decide whether the next note should补:

- 痛点
- 场景
- 搜索词
- 案例
- 信任证据
- 成交入口

## Mode Routing

### 小白商家开局诊断模式

Trigger when:

- The user is using the skill for the first time.
- The user says "我是小白", "不知道怎么开始", "账号不知道怎么做", "小红书没头绪".
- The user asks broad questions like "帮我做小红书获客" without business context.

Start with the 8-question prompt in `Default Startup Logic`.

### 单篇笔记质检/改写模式

Trigger when the user directly provides a note draft.

If the user does not provide account background, target audience, product/service, transaction path, or keywords, first say:

```markdown
这篇文案可以改，但如果不知道你卖给谁、怎么成交、用户会搜什么，容易只改成好看的文案，无法判断转化链路。建议先补充 5 个信息。

1. 产品/服务是什么？
2. 目标客户是谁？
3. B端还是C端？
4. 想承接什么动作？私信 / 店铺 / 到店 / 报名 / 试用
5. 想布局什么关键词？
```

If the user refuses or wants quick rewriting, still audit with assumptions and mark the uncertainty.

### 30 天内容地图模式

Trigger when the user asks for "30 天内容规划", "一个月小红书内容", "月度选题", or similar content map requests.

If the user has not provided product/service, target customer, B端/C端, transaction path, and keyword foundation, do not directly generate a generic list of 30 titles. First ask for the minimum planning inputs:

```markdown
可以规划 30 天内容，但不能直接生成泛泛标题。这个 Skill 的 30 天地图要服务转化链路，建议先补充 5 个信息：

1. 产品/服务是什么？
2. 目标客户是谁？B端还是 C端？
3. 成交路径是什么？私信 / 店铺 / 到店 / 报名 / 试用 / 其他
4. 你现在最想解决什么问题？没人看 / 有人看没人问 / 有人问不成交 / 不知道发什么 / 不知道怎么承接
5. 已有或想布局的关键词是什么？
```

Only after these inputs are clear, use `templates/30-day-content-map-template.md`.

### 热点翻译成生意入口模式

Hotspots are an auxiliary mode, not the beginner's first step.

Use this mode only after account diagnosis, product translation, and keyword matrix, unless the user explicitly asks to judge a hotspot.

Use four questions:

1. 有没有我的消费场景？
2. 有没有我的目标人群？
3. 有没有我的产品/服务使用理由？
4. 有没有我的情绪表达空间？

Judgment:

- 四项全部成立：强烈建议写
- 成立 3 项：可以写
- 成立 2 项：只能作为泛流量内容，谨慎写
- 成立 1 项或 0 项：不建议追这个热点

Emphasize: 热点可以用来破流量池，但不能为了爆而爆。所有热点内容都必须回到种草转化链路。

## Reference Loading

Load only the files needed for the task:

- Beginner diagnosis/account path: read `knowledge/01-methodology-summary.md`, `knowledge/02-chain-model.md`, `checklists/account-audit-checklist.md`, then use `templates/account-audit-output.md`.
- Product/service translation: read `knowledge/01-methodology-summary.md`, `knowledge/03-seva-model.md`, and `templates/product-service-translation-template.md`.
- Keyword matrix: read `knowledge/04-search-keyword-system.md` and use `templates/keyword-matrix-template.md`.
- 30-day content map: read `knowledge/02-chain-model.md`, `knowledge/04-search-keyword-system.md`, `knowledge/05-trust-conversion-system.md`, `knowledge/06-transaction-loop-system.md`, then use `templates/30-day-content-map-template.md`.
- Single note audit/rewrite: read `knowledge/03-seva-model.md`, `knowledge/04-search-keyword-system.md`, `knowledge/05-trust-conversion-system.md`, `knowledge/06-transaction-loop-system.md`, `knowledge/07-risk-rules.md`, then use `templates/single-note-audit-output.md`.
- Methodology coverage audit: read `source_materials/screenshot_notes.md` first, then update `knowledge/methodology_mapping.md`.
- Hotspot validation: read `knowledge/01-methodology-summary.md` and `checklists/topic-validation-checklist.md`.
- Post review: read `templates/post-review-template.md`.
- Optional Awei account adaptation: read `knowledge/08-optional-account-profiles.md` only when the user explicitly asks for 姑苏阿伟 account adaptation.

## SEVA Single-Note Check

Use SEVA on every note:

- **S 场景关联**: Is there a real life, work, consumption, or decision scene?
- **E 情绪调动**: Is there pain, anxiety, grievance, curiosity, pleasure, or counter-intuition?
- **V 价值传递**: Does the note provide method, judgment, avoidance advice, steps, cases, or experience?
- **A 行动指引**: Does the user know what to do next with a low-friction, compliant action?

## 种草转化完成度评分

When auditing a single note, score with 100 points:

| Dimension | Points | Standard |
| --- | ---: | --- |
| 产品/服务翻译 | 10 | 是否从参数表达改成用户场景 |
| 目标人群 | 10 | 是否明确吸引真正可能转化的人，是否区分 B端 / C端 |
| 场景关联 | 10 | 用户能不能代入 |
| 情绪调动 | 10 | 是否有痛点、焦虑、爽点、好奇、反常识 |
| 搜索承接 | 15 | 有没有关键词，用户被种草后能不能搜到 |
| 信任证据 | 15 | 有没有真实案例、过程记录、老板人设、用户共创、专业解释 |
| 价值传递 | 10 | 用户有没有获得判断、方法、避坑、流程 |
| 行动转化 | 10 | 用户看完下一步是否明确 |
| 风险合规 | 10 | 是否硬广、导流、虚构、模板化、AI感过重 |

Publishing recommendation:

- 90 分以上：重点发布，可做系列。
- 85-89 分：可发布。
- 75-84 分：修改后发布。
- 75 分以下：不建议发布。

## Output Rules

- Default to concise Chinese final deliverables.
- Lead with diagnosis, translation, or next action; do not start with theory.
- Do not treat "producing posts for Xiaohongshu" as the final goal. The final goal is clarifying and improving the conversion chain: 卖给谁, 怎么种草, 用户搜什么, 凭什么信你, 看完怎么行动.
- Do not treat hotspots as the beginner's first step.
- Do not invent cases, data, credentials, customer feedback, screenshots, or product usage scenes.
- Do not recommend spam DMs, fake engagement, fake reviews, aggressive competitor attacks, or obvious off-platform diversion.
- When rewriting, preserve the business logic and strengthen scene, emotion, keywords, trust evidence, and action design.
