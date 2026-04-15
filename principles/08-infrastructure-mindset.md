# 08 · Infrastructure Mindset — Restraint

> **Infrastructure-class products earn their value through reliability, simplicity, and being embeddable. Don't do end-user-product things just because "you can."**

## Core idea

Every tool / infrastructure product faces the same temptation: **reach down into more "user-friendly" surface area, reach up into more "complete" features**. Most products die walking this path.

Infrastructure quality comes from restraint:
- An audio library service doesn't do recommendations (that's an end-user product's job)
- A developer API doesn't do community (that's a forum's job)
- A content aggregator doesn't do comments (that's a social product's job)

**Benefits of restraint:**
1. Focus → core quality is high
2. Clear boundary → users know what to come here for and what not to
3. Reusability → you can be embedded by other products

**Restraint isn't laziness.** It's **continually answering "is this mine to do?"** and being willing to accept "no — we stop here."

## In real projects

**AudioLib** —

> *"This is not a music product. This is not a recommendation product.  
> This is a library-based audio service."*

Every new idea had to answer one question first: **is this what an infrastructure product should do?** If not — don't build it, even though you "could."

**Gospel Hub** — An aggregator, but no comments, no donations (phase 1), no user registration. Single job: "information centralization."

## Anti-patterns

- **"We could also do a…"** — every competitor feature gets copied in, and positioning blurs.
- **Half-built user-product features:** an infrastructure adds a comment section but no moderation, no notifications — it becomes spam.
- **Adding because it's simple:** a feature takes one line of code, but it doesn't belong. *Easy* is not a reason to build.

## Thinking formula

> **Is this mine to do?**  
> No? Don't do it. Even if it's "easy."

**Three self-checks:**
1. Does this feature belong to my product's positioning? Or to an upstream / downstream product?
2. If another product does this well already, what value does my crude version add?
3. With this feature added, does my core function get diluted?

## Related

- [05 · Subtract, don't add](05-subtraction-over-addition.md)
- [07 · Product boundary](07-product-boundary.md)
- [20 · Distribution is part of the product](20-distribution-is-product.md)

## Case studies

[AudioLib](../case-studies/audiolib.md) · [Gospel Hub](../case-studies/gospel-hub.md)

---

# 08 · 克制：不是基础设施该做的，别做

> **基础设施产品的价值在于可靠、简洁、可接入。不要因为"可以做"就去做用户产品的事。**

## 核心思想

每一个工具类 / 基础设施类产品，都会有一个诱惑：**往下做"更用户友好"的界面，往上做"更完整"的功能**。大部分产品就死在这条路上。

基础设施的品质感来自克制：
- 音频库服务不做推荐（推荐是用户产品的事）
- 开发者 API 不做社区（社区是论坛的事）
- 内容聚合站不做评论（评论是社交产品的事）

**克制的好处**：
1. 专注 → 核心功能质量高
2. 边界清晰 → 用户知道该来你这里做什么、不该来做什么
3. 复用 → 作为基础设施被别的产品集成

**克制不是偷懒**。它是**持续回答"这是不是我该做的"这个问题**，并接受"我就做这么多"作为答案。

## 在真实项目里长什么样

**AudioLib**：

> *"This is not a music product. This is not a recommendation product.  
> This is a library-based audio service."*

每次有新想法时，先问一句：**这是基础设施该做的事吗？** 不是，就不做——即使"可以做"。

**Gospel Hub**：聚合型产品，但不做评论、不做捐赠（第一阶段）、不做用户注册。保持"信息集中化"这个单一职能。

## 反模式

- **"我们也可以做个……"**：看到竞品有什么功能就加，产品定位越来越模糊。
- **做一半的用户产品**：基础设施加了个评论区，但没做审核、没做通知，变成一堆垃圾数据。
- **因为简单就做**：某个功能只要一行代码就能加，但它不属于这个产品——简单不是做的理由。

## 思考公式

> **这件事，是不是我该做的？**  
> 不是？不做。即使"很简单"。

**三问自检**：
1. 这个功能属于我的产品定位吗？还是属于下游/上游产品？
2. 如果别的产品已经做得很好了，我加一个粗糙版本，对用户有什么价值？
3. 加了这个功能，我的核心功能会被稀释吗？

## 延伸

- [05 · 做减法而非加法](05-subtraction-over-addition.md)
- [07 · 产品边界 = 用户决策路径](07-product-boundary.md)
- [20 · 分发是产品的一部分](20-distribution-is-product.md)

## 相关案例

[AudioLib](../case-studies/audiolib.md) · [Gospel Hub](../case-studies/gospel-hub.md)
