# 20 · Distribution Is Part of the Product

> **"Works" isn't the end. "Users can actually use it" is. Done ≠ good. Good ≠ reached.**

## Core idea

Many indie builders split the process into **"build the product"** + **"figure out distribution later."** This bifurcation leaves the product in a vacuum post-launch — no domain, no channel, no onboarding, no brand.

**Distribution is part of the product.** Reserve its place at design time, execute at the right moment.

Sub-principles:

### 20.1 · Timing of distribution awareness

**Not at the start — not at the end. At the moment MVP is stable and you're ready to promote.**

> *"现在我们来解决如何让用户最简单安装的问题。"* (Contra Code)

### 20.2 · Manual → automated rhythm

**Ship first, polish later.** The manual process itself is **defining the rules and boundaries for automation**. Don't waste energy on immature tools — wait for them to mature, then adopt.

> *"别折腾了，定时任务以后再搞。"* (Gospel Hub)

Meanwhile, **leave hooks for future automation** — optional fields in DB schema, a manual-entry admin UI, etc.

### 20.3 · Brand domain is the anchor of product identity

Buy and configure the brand domain at the validation stage, not at "official launch":

> *"我为这个产品在 godaddy 买了一个域名 xianxia.cc。"* (Xianxia)

The domain itself is a product decision — **short, precise, category-resonant**. `xianxia.cc` and `myapp-v2-final.vercel.app` represent different identities from day one.

### 20.4 · Cost & dependency prudence

**Every paid feature: is there a free equivalent?** Use existing assets where you can, but don't force an ill-fitting tool just because you've paid for it. Willing to pay for "peace of mind," not for "coolness."

### 20.5 · The folder is the first layer of product portfolio

Desktop is temporary storage. `Products/` is a portfolio. Managing your product folders coherently reflects treating each product as an independent entity — not "whatever I'm busy with."

> *"请把本地文件夹整体迁移到 /Users/.../Documents/Products"* (Xianxia / Spybook)

### 20.6 · Infrastructure added on a "useful-then-add" cadence

Donation button only after users feel the site is valuable. Analytics only after domain + some traffic. PWA-ization / desktop icon after the product is "formalized." **Each stage cares about different things.**

## In real projects

**Gospel Hub** distribution cadence:
1. Core 3 modules first (artists / releases / tours)
2. Data populated → design polish
3. Content present → custom domain
4. Domain present → Analytics
5. Trust built → donation entry
6. Finally → PWA + desktop icon

**Contra Code** — Proactively raised "how to make install easiest" once the feature was stable. Timing: not too early (no MVP yet), not too late (already launched).

## Anti-patterns

- **Launch and immediately chase traffic:** no domain, no brand — the traffic you pull in doesn't stick.
- **Obsess over distribution before MVP:** no product yet, but you're already asking "how to promote" — misplaced energy.
- **Non-prudent paid features:** pay for everything you see, no thought about alternatives.
- **Desktop chaos:** all projects on the desktop, no portfolio sense.

## Thinking formula

> **Done ≠ good. Good ≠ reached.**  
> What stage am I in? Is distribution the right next move?

**Rhythm:**
1. Spec done → buy domain ("give the product an identity")
2. MVP works → think distribution ("how do strangers see it, use it")
3. Users retaining → add analytics (where from, how long they stay)
4. Trust built → add paid / donation / subscription
5. Steady state → manual becomes automated

## Related

- [02 · Spec before code](02-spec-before-code.md)
- [08 · Infrastructure mindset](08-infrastructure-mindset.md)
- [17 · Core metric bound to real engagement](17-real-engagement-metrics.md)

## Case studies

[Contra Code](../case-studies/contra-code.md) · [Gospel Hub](../case-studies/gospel-hub.md) · [Xianxia](../case-studies/xianxia.md) · [Spybook](../case-studies/spybook.md)

---

# 20 · 分发是产品的一部分

> **产品不是"能运行"就结束，"用户能用上"才是完成。做完 ≠ 做好，做好 ≠ 用得到。**

## 核心思想

很多独立开发者把产品分成两段：**"做产品"** + **"之后再想怎么分发"**。这种切分会让产品上线后陷入真空——没有域名、没有分发通道、没有 onboarding、没有品牌。

**分发是产品的一部分**，要在设计阶段就预留位置，在合适的时机动手。

这条原则下有几个子原则：

### 20.1 · 分发意识的时机

**不是做完才想，也不是一开始就纠结。而是在 MVP 稳定、准备推广时主动思考分发。**

> *"现在我们来解决如何让用户最简单安装的问题。"*（Contra Code）

### 20.2 · 手动 → 自动化的节奏

**先能跑起来，再谈精致。** 手动做的过程其实是**为自动化定义规则和边界**。不在未成熟的工具上浪费精力，等它成熟了再接入。

> *"别折腾了，定时任务以后再搞。"*（Gospel Hub）

同时**留 hook 为将来自动化铺路**（数据库 schema 加可选字段、后台加手工录入界面）。

### 20.3 · 品牌域名是产品身份的锚点

产品验证阶段就绑定品牌域名，而不是等"正式上线"才考虑。

> *"我为这个产品在 godaddy 买了一个域名 xianxia.cc。"*（Xianxia）

域名本身就是一种选品判断——**短、精准、品类感强**。`xianxia.cc` 比 `myapp-v2-final.vercel.app` 从第一天就是不同的身份。

### 20.4 · 审慎的成本与依赖判断

**每一个付费功能都要问"有没有免费的替代"**。已有资产要想办法用上，但不因为付过钱就强行用不合适的工具。愿意为"省心"付出复杂度成本，但不为"酷炫"买单。

### 20.5 · 文件夹就是产品组合的第一层架构

桌面是临时区，`Products/` 是产品组合。能对自己的产品文件夹做统一管理，说明把每个产品当独立个体经营，而不是"当前在忙的项目"。

> *"请把本地文件夹整体迁移到 /Users/.../Documents/Products"*（Xianxia / Spybook）

### 20.6 · 基础设施按"有用才加"的顺序铺开

捐赠按钮放在用户开始觉得"这网站真的有价值"之后才加。Analytics 在有域名和流量之后才加。PWA 化 / 桌面图标在产品"正式化"之后才加。**每个阶段该关心的事情不一样**。

## 在真实项目里长什么样

**Gospel Hub** 的分发节奏：
1. 先做核心三个模块（艺人/发行/演出）
2. 数据填充后才做设计美化
3. 有内容后才考虑自定义域名
4. 有了域名才想到 Analytics
5. 最后才加捐赠入口（信任建立后）
6. 最后才做 PWA 桌面图标

**Contra Code**：功能稳定后主动提出 "如何让用户最简单安装" —— 时机不是太早（没 MVP 不想），不是太晚（上线才想）。

## 反模式

- **上线即开始找流量**：没绑域名没定品牌，开始推广 —— 推来的流量留不住。
- **一开始就纠结分发**：还没有 MVP 就想着"怎么推"，精力错配。
- **付费功能不审慎**：看到就加，不想替代方案。
- **桌面混乱**：所有项目都在桌面，没有产品组合意识。

## 思考公式

> **做完了 ≠ 做好了。做好了 ≠ 用得到。**  
> 到哪一步了？下一步该不该做分发？

**阶段节拍**：
1. Spec 完成 → 买域名（"给产品一个身份"）
2. MVP 跑通 → 想分发（"怎么让陌生人看到、用到"）
3. 有用户留存 → 加 Analytics（知道从哪来、留多久）
4. 信任建立 → 加付费/捐赠/订阅
5. 常规运营 → 手动变自动化

## 延伸

- [02 · 先定性，再动手](02-spec-before-code.md)
- [08 · Infrastructure 心智](08-infrastructure-mindset.md)
- [17 · 核心指标绑定真实投入](17-real-engagement-metrics.md)

## 相关案例

[Contra Code](../case-studies/contra-code.md) · [Gospel Hub](../case-studies/gospel-hub.md) · [Xianxia](../case-studies/xianxia.md) · [Spybook](../case-studies/spybook.md)
