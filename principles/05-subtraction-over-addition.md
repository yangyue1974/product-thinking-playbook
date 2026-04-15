# 05 · Subtract, Don't Add

> **Features aren't better because there are more of them. They're better because they fit the scenario more tightly.**

## Core idea

Most feature creep isn't because you "wanted to add" — it's because you didn't have **a yardstick for cutting**. With a scenario as the yardstick, subtraction becomes natural:

| Cut | Reason |
|---|---|
| Weapon upgrades | Programmers won't play long enough |
| Level progression | Doesn't fit the scenario |
| User registration | Adds friction to first use |
| Recommendation algorithm | This isn't a recommendation product |
| Comments / social | Not in v1 |

**Every time you're about to add a feature, ask:** does the user — in this scenario — have the patience for this? Are they willing to spend one extra step?

This applies beyond MVP. At every stage, before adding, ask: am I serving the scenario, or escaping boredom?

## In real projects

**Contra Code** — When defining gameplay, subtraction came first: cut weapon upgrades, levels, complex plot, registration; keep score-based challenges, in-place respawn, anonymous leaderboards.

**AudioLib** —

> *"This is not a music product. This is not a recommendation product. This is a library-based audio service."*

This **restrained self-definition** prevented feature bloat. Every new idea had to pass one question: is this what an infrastructure product should do?

**Gospel Hub** — Phase 1 explicit exclusions: user accounts / comments / donations / agent-based scraping. **The "not doing" list is as important as the "doing" list.**

## Anti-patterns

- **"Do a little of everything"**: afraid of missing a need, you add a bit of each — and none of it is great.
- **Cargo-cult additions**: the competitor added search, you add search. Their scenario isn't yours.
- **Monetization and social before MVP**: core flow isn't proven yet, but you've already stacked on payment walls / social / points.

## Thinking formula

> **Use scenario to reverse-derive what NOT to do, not a feature list to forward-enumerate what to do.**

**Three questions before adding:**
1. In my scenario, does the user have patience for this?
2. Without this feature, does the core value suffer? If not, don't add yet.
3. If this feature is to be done well, what else comes with it? (Login usually drags in user management, password reset, email service…)

## Related

- [01 · Scenario-first](01-scenario-first.md) — scenario is the yardstick
- [07 · Product boundary](07-product-boundary.md)
- [08 · Infrastructure mindset](08-infrastructure-mindset.md)

## Case studies

[Contra Code](../case-studies/contra-code.md) · [AudioLib](../case-studies/audiolib.md) · [Gospel Hub](../case-studies/gospel-hub.md)

---

# 05 · 做减法而非加法

> **功能不是加得越多越好，而是越贴合场景越好。**

## 核心思想

大部分功能蔓延不是因为"想加"，而是因为**没有一个减法的标尺**。有了场景做标尺，减法是自然的：

| 去掉 | 原因 |
|---|---|
| 武器升级 | 码农不可能超时间玩 |
| 关卡通关 | 场景不适合 |
| 用户注册 | 增加使用门槛 |
| 推荐算法 | 这不是推荐产品 |
| 评论/社交 | 第一阶段不做 |

**每加一个功能，先问一句**：这个场景下，用户有这个耐心吗？愿意为这个功能多花一步吗？

不只是 MVP 阶段要做减法。产品任何阶段，加功能之前都该问：是在贴合场景，还是在摆脱无聊？

## 在真实项目里长什么样

**Contra Code**：定义玩法时主动做减法——砍掉武器升级、关卡通关、复杂剧情、用户注册；保留积分挑战、就地重生、匿名排行。

**AudioLib**：

> *"This is not a music product. This is not a recommendation product.  
> This is a library-based audio service."*

这种**对产品本质的克制定义**，防止了功能蔓延。每次有新想法时先问：这是基础设施该做的事吗？

**Gospel Hub**：第一阶段明确不做——用户注册 / 评论 / 捐赠 / Agent 抓取。"**不做"清单和"要做"清单同等重要**。

## 反模式

- **"都做一点"**：怕漏掉需求，每样都做点，最后每样都不好用。
- **因为别人有所以我也得有**：竞品加了搜索你也加，竞品加了 AI 你也加。别人的场景不是你的场景。
- **MVP 阶段就加付费墙/社交/积分系统**：核心路径还没跑通，先堆外围。

## 思考公式

> **用"场景"反推"哪些功能不要"，而不是用"功能列表"正推"做什么"。**

**加功能之前三问**：
1. 我的场景里，用户有这个耐心吗？
2. 这个功能不加，产品核心价值受影响吗？不受影响，暂时不加。
3. 如果这个功能要做好，要多少后续投入？（登录通常连着用户管理、密码找回、邮件服务……）

## 延伸

- [01 · 场景先于功能](01-scenario-first.md) —— 场景是减法的标尺
- [07 · 产品边界 = 用户决策路径](07-product-boundary.md)
- [08 · Infrastructure 心智](08-infrastructure-mindset.md)

## 相关案例

[Contra Code](../case-studies/contra-code.md) · [AudioLib](../case-studies/audiolib.md) · [Gospel Hub](../case-studies/gospel-hub.md)
