# 01 · Scenario-First

> **Good products start from observing a real scenario — not from a feature list.**

## Core idea

Most products don't fail because they lacked features. They fail because the features didn't fit a real scenario. Describe — in one concrete sentence — **the situation the user is in, the posture they use your product in, and the emotion they carry** when they open it. The feature set will then fall out naturally, and most of it will be cut.

A scenario isn't a vague persona ("young urban professionals"). It's a sentence specific enough to picture:

> *"Programmers have a lot of dead time while waiting on builds, and it's boring."*

From that one line, these all drop out:
- Players won't invest long stretches → **no levels, no weapon upgrades**
- Players get yanked back to work any second → **respawn in place**
- Visuals must not intrude on the editor → **bottom overlay**
- Keys can't collide with the IDE → **focus-switching mechanism**

## In real projects

**Contra Code** — The entire project started from one scenario sentence, and every downstream decision was re-checked against it:

> *"我们在 Coding 的时候都有大量的等待时间非常无聊，这个场景是一个真实的需求。"*

When someone else made a Super Mario overlay, the reaction wasn't "cool" — it was "this is a real, under-served scenario."

**Gospel Hub** — The core value was nailed down first: *"Information centralization — take wildly scattered information and bring it to one place."* The scenario is "a Gospel music fan bouncing between YouTube, Spotify, Apple Music, and tour sites." The product form — an aggregator — falls out of the scenario.

## Anti-patterns

- **Feature-driven:** "I want to build an XX with AI + social + gamification." Each noun is a feature, none is a scenario.
- **Audience-driven:** "I want to build for Gen Z." An audience isn't a scenario — the same person is a different user at different moments.
- **Tech-driven:** "AI is hot, let me build something with AI." Tools-first, not needs-first.

## Thinking formula

> Don't ask "is this feature good?" — ask "what does this scenario actually look like?"

**Three self-checks:**
1. Can I describe, in one sentence, the scenario my user is in?
2. Is that scenario real? Am I someone who lives in it?
3. Can every feature be derived from that scenario? The ones that can't — can they be cut?

## Related

- [05 · Subtract, don't add](05-subtraction-over-addition.md) — scenario is the yardstick
- [07 · Product boundary = user's decision path](07-product-boundary.md)
- [12 · Content standards > technical standards](12-content-standards-first.md)

## Case studies

[Contra Code](../case-studies/contra-code.md) · [Gospel Hub](../case-studies/gospel-hub.md)

---

# 01 · 场景先于功能

> **好产品从观察真实场景开始，不是从功能列表开始。**

## 核心思想

大多数产品失败，不是因为功能不够多，而是功能**不够贴合场景**。先把"用户在什么情况下、用什么姿势、带着什么情绪用这个产品"描述清楚，功能自然就定下来了——而且大部分会被砍掉。

场景不是"目标用户是谁"那种空泛的画像，是一句具体到能想象画面的陈述：
> "程序员在 Coding 的时候有大量的等待时间非常无聊。"

这一句就能推导出：
- 玩家不会长时间投入 → 不要关卡/武器升级
- 玩家随时被拉回工作 → 死了就地重生
- 画面不能干扰编程 → 底部浮层
- 按键不能和 IDE 冲突 → 焦点切换机制

## 在真实项目里长什么样

**Contra Code**：起点就是一句场景描述，之后每一个功能取舍都回到这句话来判断。

> *"我们在 Coding 的时候都有大量的等待时间非常无聊，这个场景是一个真实的需求。"*

看到别人做超级玛丽浮层，没停留在"好酷"，而是立刻意识到这是个被普遍低估的真实场景。

**Gospel Hub**：核心价值先写死——"信息集中化，把极度分散的信息统一汇聚到一个地方"。场景是"福音乐迷现在要在 YouTube/Spotify/Apple Music/Tour 网站之间反复跳"，于是产品形态自然指向聚合。

## 反模式

- **功能驱动**："我想做一个带 AI、带社交、带签到的 XXX" —— 每个名词都是功能，没有一个是场景。
- **人群驱动**："我要做给 Z 世代的 XXX" —— 人群不是场景，同一个人在不同时刻是不同用户。
- **技术驱动**："现在 AI 这么火，我用 AI 做个……" —— 工具先行，不是需求先行。

## 思考公式

> 不问"这个功能好不好"，问"这个场景到底是什么样的"。

**三问自检**：
1. 我能用一句话说清楚"用户在什么场景下用这个产品"吗？
2. 这个场景真实存在吗？我自己是不是这个场景里的人？
3. 每个功能都能从这句场景反推出来吗？反推不出来的功能是不是都可以先砍？

## 延伸

- [05 · 做减法而非加法](05-subtraction-over-addition.md) —— 场景是减法的标尺
- [07 · 产品边界 = 用户决策路径](07-product-boundary.md)
- [12 · 内容标准 > 技术标准](12-content-standards-first.md)

## 相关案例

[Contra Code](../case-studies/contra-code.md) · [Gospel Hub](../case-studies/gospel-hub.md)
