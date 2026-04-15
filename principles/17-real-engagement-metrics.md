# 17 · Core Metric Bound to Real Engagement

> **Whether the product is working should be answerable by one question. Finding that one question is worth more than stacking a hundred metrics.**

## Core idea

Most products stare at the wrong numbers: registrations, DAU, PV, UV. Those only show that the product has been **opened** — not that it **held** the user.

The metric that reflects real product health is typically **a behavior the user had to pay a cost to perform**.

For example:
- Content product → what chapter did the user reach / what minute did they listen to
- Tool product → did the user open it a 3rd time / make their first payment
- Community product → did the user post their first content / reply to someone

That metric must directly answer: **"is my product actually working?"**

Find it → the admin dashboard becomes meaningful. Don't find it → no amount of data is signal.

## In real projects

**Spybook** — The core metric is **last_read_chapter** (which chapter each user reached). One field directly answers "is the content gripping?"

Further: **arc_done** (reached chapter 15) as the threshold for "real engagement," **distinct from "opened."**

> *"比如我希望能看到每个用户到了第几章，这样我才知道我的产品是否真的受欢迎。"*

**Xianxia** — Same logic:

> *"我才知道我的产品是否真的受欢迎。"*

Not "user count" / "PV/UV" style generic metrics — **which chapter each user reached** directly reflects whether the content is gripping, whether the user is truly engaged.

**Supporting principle** — When existing data is enough, don't add new tools. The data is in SQLite, all metrics are SQL queries away. No need to bring in Metabase / PostHog. An `/admin` page in the app reads the DB directly.

**Supporting principle** — Minimalism for admin tools. Internal tools don't need to be "product-ized" — audience is just you. Hidden URL + single admin account + 404 for everyone else. Put the effort into data accuracy and metric clarity.

## Anti-patterns

- **Tracking registrations / DAU:** doesn't reflect real usage depth. A user opening for 30 seconds vs. 30 minutes a day is worlds apart.
- **Integrating analytics SDK before launch:** data model isn't stable, events pile up messy.
- **No "real engagement" threshold:** count "ever opened" as success.
- **Product-izing the admin panel:** spend days building login / permissions / menus / design — for a tool you alone will use.

## Thinking formula

> **Can one number tell me whether my product is succeeding?**  
> Is that number about "opens," or "real engagement"?

**One test:** if you could only see *one* number to judge whether the product is working, what would it be? Can't name it → product positioning isn't clear yet.

## Related

- [01 · Scenario-first](01-scenario-first.md)
- [04 · Subtitle as promise](04-subtitle-as-promise.md)
- [18 · Persistence is trust](18-persistence-is-trust.md)

## Case studies

[Spybook](../case-studies/spybook.md) · [Xianxia](../case-studies/xianxia.md)

---

# 17 · 核心指标绑定真实投入

> **知道产品是否成功，只需要一个问题的答案。找到那个问题，比堆一百个指标都重要。**

## 核心思想

大多数产品盯着错的指标看：注册数、DAU、PV、UV。这些指标**只能说明产品被打开过**，不能说明产品**抓住了用户**。

真正反映产品健康的指标，通常是一个**需要用户付出成本才会发生的行为**。

比如：
- 内容产品 → 用户读到第几章 / 听到第几分钟
- 工具产品 → 用户第 3 次打开 / 第一次付费
- 社区产品 → 用户发出第一条内容 / 回复某人

这个指标要**足够直接地回答**："**我的产品有没有真的在起作用？**"

找到这个指标，管理后台才有意义；找不到，再多的数据都是噪音。

## 在真实项目里长什么样

**Spybook** · 核心指标是 **last_read_chapter**（每个用户读到第几章）。一个字段直接回答"内容是否抓人"。

进一步定义 **arc_done**（读到第 15 章）作为"真正投入"的门槛，**区别于"打开过"**。

> *"比如我希望能看到每个用户到了第几章，这样我才知道我的产品是否真的受欢迎。"*

**Xianxia** · 同样的思路：

> *"我才知道我的产品是否真的受欢迎。"*

需要的不是"用户量"、"PV/UV"这类通用指标，而是"每个用户读到了第几章"——直接反映内容是否抓人、用户是否真的投入。

**配套原则** · 存量数据够用时，不引入新工具。数据已经在 SQLite 里，所有指标都能用 SQL 查出来。没有必要接 Metabase / PostHog —— 在 app 里加 /admin 页面，直接查数据库。

**配套原则** · 管理工具极简主义。内部工具不需要"产品化"，它的受众只有你一个人。隐藏 URL + 唯一账号可见 + 404 给其他人。把精力花在让数据准确、指标清晰上。

## 反模式

- **盯着注册数 / DAU**：不反映真实使用深度。一个用户每天打开 30 秒和打开 30 分钟是天差地别的。
- **一上线就接埋点 SDK**：数据结构还没定，就开始堆埋点，数据越来越乱。
- **没有"真投入"门槛**：把"打开过"当成功，把所有曾经点过的用户都计入活跃。
- **管理后台先做产品化**：内部工具花时间做登录、权限、菜单、设计—— 自己一个人用，根本不需要。

## 思考公式

> **我的产品有没有成功，能不能用一个指标回答？**  
> 这个指标反映的是"打开过"，还是"真投入"？

**一测**：如果只能看到一个数字来判断产品好不好，那个数字是什么？找不出来，说明产品定位还没想清楚。

## 延伸

- [01 · 场景先于功能](01-scenario-first.md)
- [04 · 副标题是承诺](04-subtitle-as-promise.md)
- [18 · 持久化 = 信任基础](18-persistence-is-trust.md)

## 相关案例

[Spybook](../case-studies/spybook.md) · [Xianxia](../case-studies/xianxia.md)
