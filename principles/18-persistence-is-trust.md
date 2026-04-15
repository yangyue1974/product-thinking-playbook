# 18 · Persistence Is the Foundation of Trust

> **What a user invested in your product, your product has a duty to remember. Persistence isn't an engineering question — it's a product promise.**

## Core idea

Every user interaction is an **investment**:
- Time invested: 10 minutes walking through a conversation
- Content invested: telling the product their background, context, question
- Emotion invested: revealing something of their state in dialogue

**The product has a duty to remember these investments.** The moment a user realizes "the AI forgot what I just said" or "my last record is gone" — **trust collapses on the spot**. The user will not say it a second time. They simply decide this product isn't worth the investment.

**The granularity of persistence** isn't an engineering question — it's a product promise:
- Promised a "consult" → promise to remember what was said before
- Promised "continue reading" → promise to remember where they stopped
- Promised "my XX" → promise it's theirs, still there when they come back

## In real projects

**Tarot** — Conversation records weren't saved. Reopening a past reading, chat content was gone.

> *"用户把他们思考过的东西告诉了产品，产品忘记了。这不是一个技术 bug，这是信任损耗。用户不会再说第二遍的。"*

**Tarot** — Related principle: **user behavior is continuous, not discrete.**

Engineering defaulted to treating each "draw again" as independent (clear context, start fresh). Wrong. The user came for a **cumulative consultation**, not multiple **discrete queries**. Persistence granularity must serve the "consultation" behavior unit, not the "query" unit.

## Anti-patterns

- **Every session starts fresh context:** AI forgot what the user said.
- **Refresh loses everything:** mid-operation, network hiccup, gone.
- **"Only saved if logged in" as excuse:** many light-interaction products can use localStorage / anonymous ID to save first, bind on signup. Let "try first" and "keep data" coexist.
- **No cross-device sync:** user typed a bunch on phone, switches to laptop, all gone.

## Thinking formula

> What did the user **invest** at this step?  
> Next time they open it, what do they **expect to still be there**?

**Two self-checks:**
1. Of the things users do in my product, which must be remembered? At what granularity?
2. If a piece of information disappeared, would the user react with "no big deal" or "this product is trash"? If the latter — it must be persisted.

## Related

- [17 · Core metric bound to real engagement](17-real-engagement-metrics.md)
- [19 · Cross-platform parity + honest permissions](19-honest-parity.md)
- [07 · Product boundary](07-product-boundary.md)

## Case studies

[Tarot](../case-studies/tarot.md)

---

# 18 · 持久化 = 信任基础

> **用户对产品的投入，产品有义务记住。持久化不是工程问题，是产品承诺问题。**

## 核心思想

用户每一次和产品的交互，都是一次**投入**：
- 投入时间：花 10 分钟走完一轮对话
- 投入内容：告诉产品自己的背景、处境、问题
- 投入情绪：在对话里暴露了某种状态

**产品有义务记住这些投入**。一旦用户发现"我刚刚说的 AI 都忘了"、"我上次的记录没了"——**信任立刻崩塌**。用户不会再说第二遍，他们直接认定这个产品不值得投入。

**持久化到什么粒度**，不是工程问题，是产品承诺问题：
- 承诺了"咨询"，就要承诺"记得之前聊过什么"
- 承诺了"继续阅读"，就要承诺"记住读到哪里"
- 承诺了"我的 XX"，就要承诺"这是你的，关掉再开还在"

## 在真实项目里长什么样

**Tarot** · 对话记录没有保存，用户重新进入历史推演，聊天内容消失了。

> *"用户把他们思考过的东西告诉了产品，产品忘记了。这不是一个技术 bug，这是信任损耗。用户不会再说第二遍的。"*

**Tarot** · 一个相关原则：**用户行为是连续的，不是离散的**。

"再次抽牌"在工程侧默认是每一轮都独立的（清空上下文，重新开始）。但这是错的。用户来的是一次**累积的咨询**，不是多次**离散的查询**。持久化粒度必须服务于"咨询"这个行为单元，不能服务于"查询"。

## 反模式

- **每次会话都开新上下文**：用户说过的话 AI 忘了。
- **刷新就丢失**：操作一半，网络抖一下全没了。
- **"登录才保存"作为借口**：很多轻交互产品可以用 localStorage / 匿名 ID 先存着，等用户注册再绑定。让"先体验"和"保留数据"兼得。
- **跨设备不同步**：用户在手机上输了一堆，换电脑登录都没了。

## 思考公式

> 用户在这一步**投入了什么**？  
> 下一次打开，他期待**还在**的是什么？

**两问自检**：
1. 用户在产品里做的事，哪些必须记住？记住到什么粒度？
2. 如果某个信息丢失了，用户的反应是"没关系"还是"这产品太烂了"？后者就必须持久化。

## 延伸

- [17 · 核心指标绑定真实投入](17-real-engagement-metrics.md)
- [19 · 跨端一致 + 权限诚实](19-honest-parity.md)
- [07 · 产品边界 = 用户决策路径](07-product-boundary.md)

## 相关案例

[Tarot](../case-studies/tarot.md)
