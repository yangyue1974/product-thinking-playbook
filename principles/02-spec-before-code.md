# 02 · Spec Before Code

> **The product doc is upstream of engineering, not an artifact you write after shipping.**

## Core idea

Whether you're writing code yourself or letting an AI do it, **before the first line of code, put the product in writing**. Two documents pay off more than any other artifact:

- **A product logic doc** — core value, user path, key junctions, and an explicit *"what we will NOT do"* list
- **A technical boundary doc** — stack, data shape, module split, initial data

Documents aren't valuable because they predict the future correctly. They're valuable because **they give every step an unambiguous finish line**. With a spec in hand, watching an AI write code is editing; without one, you're doing product design live in comment threads.

**"Discuss first, then do"** is the corollary: before engineering (or an AI) touches anything that affects the user path, put it in words. Code can be rewritten; architectural direction, once off, is expensive to undo.

## In real projects

**AudioLib** — The project started with two documents: one defining product logic (*what this is NOT* + *what this IS*), one defining technical boundaries. Spec came before the repo was even created.

**Xianxia** —

> *"你先不要改，我们来讨论一下。"*

Before confirming the core mechanic ("Chapter 15 writes straight through, no mid-way prompt"), engineering was paused. Lock the logic in language, then ship code.

**Spybook** — When presented with 14 audit bugs, the response wasn't per-item debate. It was: draft the full fix plan first, then execute.

> *"你按计划步骤做吧。"*

Planning first lets execution be "mindless" — cognitive bandwidth goes into judgment, not real-time decisions.

## Anti-patterns

- **Build-then-fix:** ship a version and see, realize on day 3 the direction is wrong, start over.
- **Doc-as-deliverable:** write docs after shipping, as compliance, never read them again.
- **Feature list masquerading as spec:** 20 features listed, but "what we won't do", "who for", "what counts as success" — all missing.

## Thinking formula

> Can a complete stranger read your spec and understand:  
> **Who this solves a problem for? The next 3 things we'll do? The things we're explicitly not doing?**

**Minimum spec skeleton:**
1. One-sentence scenario
2. Core value (what this is NOT / what this IS)
3. The three key junctions on the user path
4. *"Not in v1"* list
5. Success criterion (the minimum loop that has to work)

## Related

- [01 · Scenario-first](01-scenario-first.md) — spec starts from scenario
- [06 · Vision non-negotiable](06-vision-non-negotiable.md) — the spec anchors the vision
- [11 · Commander posture](11-commander-posture.md)

## Case studies

[AudioLib](../case-studies/audiolib.md) · [Xianxia](../case-studies/xianxia.md) · [Spybook](../case-studies/spybook.md) · [Gospel Hub](../case-studies/gospel-hub.md)

---

# 02 · 先定性，再动手

> **产品文档是工程的上游，不是工程完成后的附属品。**

## 核心思想

不论是自己写代码，还是让 AI 写代码，**写第一行代码之前，先用文字把产品想清楚**。两份文档的价值最大：

- **一份定义产品逻辑**：核心价值、用户路径、关键节点、"不做什么"清单
- **一份定义技术边界**：技术栈、数据结构、模块划分、初始数据

文档的价值不是"对未来预测正确"，而是**让执行过程中的每一步都有明确的完成标准**。有了文档，AI 写代码时你是在审稿，不是在实时设计。没有文档，你每一步都在用嘴做产品。

**"先讨论，再动手"** 是这条原则的副产物：工程（或 AI）开始写代码之前，凡是影响用户路径的决策，都值得先用语言说清楚。代码可以反复改，架构方向一旦跑偏，重构成本极高。

## 在真实项目里长什么样

**AudioLib**：起点是两份文档，一份定义产品逻辑（这不是什么 + 这是什么），一份定义技术边界。项目建仓之前，Spec 先成。

**Xianxia**：

> *"你先不要改，我们来讨论一下。"*

在确认「第 15 章直写到底、不设中途提示」这个核心机制前，主动叫停工程实现，要先把逻辑想清楚再落地。

**Spybook**：拿到 14 个 bug 后没有逐条讨论，而是要求先出完整修复计划再开始执行。

> *"你按计划步骤做吧。"*

计划先行之后，执行时就能"无脑执行"——认知资源放在判断上，不是实时决策上。

## 反模式

- **边做边改**：先让 AI 写一版跑起来再说，结果第三天发现方向错了，全推翻。
- **文档当交付物**：做完才补文档，交差用，自己都不读。
- **功能列表当 Spec**：列了 20 个功能，但没说"不做什么"、"为谁做"、"怎么算成功"。

## 思考公式

> 能不能让一个完全不认识你的人，看完你的 Spec 就明白：  
> **这个产品为谁解决什么问题？下一步要做哪 3 件事？哪些事明确不做？**

**Spec 最小骨架**：
1. 一句话场景
2. 核心价值（这不是什么 / 这是什么）
3. 用户路径的关键 3 个节点
4. "第一阶段不做"清单
5. 成功标准（V1 跑通的最小闭环）

## 延伸

- [01 · 场景先于功能](01-scenario-first.md) —— Spec 从场景开始
- [06 · 愿景不妥协](06-vision-non-negotiable.md) —— Spec 是愿景的锚点
- [11 · 指挥者姿态](11-commander-posture.md)

## 相关案例

[AudioLib](../case-studies/audiolib.md) · [Xianxia](../case-studies/xianxia.md) · [Spybook](../case-studies/spybook.md) · [Gospel Hub](../case-studies/gospel-hub.md)
