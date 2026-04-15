# product-thinking-playbook

> A decision-making playbook for solo product builders — **20 principles across 5 dimensions**,  
> extracted from the full development conversations of 6 shipped products.  
> 独立开发者的产品判断手册 · 从 6 个已上线产品的全过程对话中提炼 · 20 条原则 / 5 个维度

[中文](#中文) · [English](#english)

---

## English

### Why this exists

AI coding tools can now write almost anything. The bottleneck has moved from **"can you build it"** to **"do you know what to build, where to stop, and how to tell it's done"**.

Most product writing is written by teams for teams. This playbook is written for **one person** making every call alone: what to build, what to cut, when to ship, what metric actually matters.

### Who it's for

- Indie hackers shipping with AI (Claude Code, Cursor, v0, Lovable, etc.)
- Product people who code, engineers becoming product people
- Anyone who has ever asked: *"AI just built me 10 things — but is any of this the right thing?"*

### How to use it

1. **Read [`SKILL.md`](./SKILL.md)** — the entry point, with a trigger table mapping symptoms to principles.
2. **Read `principles/`** — one file per principle. Each has a real dialogue, anti-pattern, and thinking formula.
3. **Read `case-studies/`** — 6 complete project retrospectives. The principles are derived from these.
4. **Use `quick-reference.md`** — a one-page checklist for when you're stuck.

As a Claude Code / AI agent skill:
```
> Using product-thinking-playbook: should I add this feature now, or wait?
```

### The 20 principles (at a glance)

| # | Principle | Dimension |
|---:|---|---|
| 01 | Scenario before feature | Intent |
| 02 | Spec before code | Intent |
| 03 | Aesthetic as stance | Intent |
| 04 | Subtitle as promise, not description | Intent |
| 05 | Subtract, don't add | Boundary |
| 06 | Vision non-negotiable, implementation flexible | Boundary |
| 07 | Product boundary = user's decision path | Boundary |
| 08 | Infrastructure mindset — restraint | Boundary |
| 09 | Decisive on direction, meticulous on detail | Execution |
| 10 | Borrow existing cognition | Execution |
| 11 | Commander posture with AI | Execution |
| 12 | Content standards > technical standards | Execution |
| 13 | End-to-end fixes, not surface patches | Quality |
| 14 | Design error ≠ execution error | Quality |
| 15 | Experience before review | Quality |
| 16 | Security = product quality | Quality |
| 17 | Core metric bound to real engagement | Closed Loop |
| 18 | Persistence is the foundation of trust | Closed Loop |
| 19 | Cross-platform parity + honest permissions | Closed Loop |
| 20 | Distribution is part of the product | Closed Loop |

### License

MIT — use it, fork it, translate it, turn it into your own playbook. Credit appreciated, not required.

---

## 中文

### 为什么写这个

AI 已经能写几乎所有代码。瓶颈从"**能不能做出来**"转到了"**知不知道该做什么、什么时候停、怎么算做完**"。

市面上的产品文档大多数是团队写给团队的。这个 playbook 是写给**一个人**的 —— 做决定靠自己、代码让 AI 写、判断必须自己下。

### 写给谁看

- 用 AI 工具（Claude Code / Cursor / v0 / Lovable）独立发产品的人
- 会写代码的产品人、想往产品走的工程师
- 任何曾经问过 *"AI 一口气给我写了 10 个功能，可这些是对的吗？"* 的人

### 怎么用

1. **先看 [`SKILL.md`](./SKILL.md)** — 入口文档，有"症状→原则"对照表
2. **读 `principles/`** — 20 条原则各自独立成文，带真实对话 + 反模式 + 思考公式
3. **读 `case-studies/`** — 6 份完整项目复盘，原则就是从这些对话里提炼的
4. **用 `quick-reference.md`** — 卡住的时候一页速查

作为 Claude Code skill 使用：
```
> 用 product-thinking-playbook 判断：这个功能该加吗？
```

### 20 条速览

**I. 立意 Intent**
1. 场景先于功能 · 2. 先定性，再动手 · 3. 气质即立场 · 4. 副标题是承诺

**II. 边界 Boundary**
5. 做减法而非加法 · 6. 愿景不妥协，实现可妥协 · 7. 产品边界=用户决策路径 · 8. 克制：Infrastructure 心智

**III. 执行 Execution**
9. 决策果断，细节挑剔 · 10. 借力已有认知 · 11. 指挥者姿态 · 12. 内容标准 > 技术标准

**IV. 品质 Quality**
13. 端到端修复 · 14. 设计错误 vs 执行错误 · 15. 先用再评 · 16. 安全=产品品质

**V. 闭环 Closed Loop**
17. 核心指标绑定真实投入 · 18. 持久化=信任基础 · 19. 跨端一致+权限诚实 · 20. 分发是产品的一部分

### 案例底座

- [Contra Code](case-studies/contra-code.md) · VS Code 内嵌游戏浮层
- [AudioLib](case-studies/audiolib.md) · 开发者用的音频库服务
- [Gospel Hub](case-studies/gospel-hub.md) · 福音音乐聚合站
- [Spybook](case-studies/spybook.md) · 互动侦探叙事小说
- [Tarot](case-studies/tarot.md) · AI 塔罗咨询
- [Xianxia](case-studies/xianxia.md) · AI 仙侠小说生成

### License

MIT · 随便用、随便 fork、随便翻译、随便改成你自己的 playbook。致谢欢迎，不强求。

---

*作者 [@yangyue1974](https://github.com/yangyue1974) · [43.group](https://43.group)*
