# Quick Reference · 一页速查表

> Read it when stuck. Find the line that hurts most.  
> 卡住的时候念一遍，找"最刺痛自己"那一条。

## Symptom → Principle · 症状 → 原则对照表

| You're feeling / 你正在感觉到 | Read / 该翻 |
|---|---|
| "Don't know what to do first" / "不知道先做什么" | [01 Scenario-first · 场景先于功能](principles/01-scenario-first.md) · [02 Spec before code · 先定性再动手](principles/02-spec-before-code.md) |
| "Features keep piling up, can't stop" / "功能越加越多，收不住" | [05 Subtract, don't add · 做减法而非加法](principles/05-subtraction-over-addition.md) · [08 Infrastructure mindset · Infrastructure 心智](principles/08-infrastructure-mindset.md) |
| "Looks the same as competitors" / "和同类产品看起来差不多" | [03 Aesthetic as stance · 气质即立场](principles/03-aesthetic-as-stance.md) · [10 Borrow cognition · 借力已有认知](principles/10-borrowed-cognition.md) |
| "Just using whatever AI gives me" / "AI 给什么我用什么" | [11 Commander posture · 指挥者姿态](principles/11-commander-posture.md) · [15 Experience before review · 先用再评](principles/15-experience-before-review.md) |
| "Tech says it can't be done, thinking of downgrading" / "技术说做不到，想降级" | [06 Vision non-negotiable · 愿景不妥协](principles/06-vision-non-negotiable.md) |
| "Bugs keep resurfacing" / "bug 修了又出" | [13 End-to-end fixes · 端到端修复](principles/13-end-to-end-fixes.md) · [14 Design vs execution error · 设计错误 vs 执行错误](principles/14-design-vs-execution-error.md) |
| "Content quality is just off" / "内容质量总差一口气" | [12 Content standards > technical standards · 内容标准 > 技术标准](principles/12-content-standards-first.md) |
| "Don't know if the product is any good" / "不知道产品好不好" | [17 Real engagement metrics · 核心指标绑定真实投入](principles/17-real-engagement-metrics.md) |
| "Shipped, what's next?" / "上线了，不知道下一步" | [20 Distribution is product · 分发是产品的一部分](principles/20-distribution-is-product.md) |
| "Users complain, can't pin it down" / "用户反馈不对劲说不清" | [07 Product boundary · 产品边界](principles/07-product-boundary.md) · [18 Persistence = trust · 持久化=信任](principles/18-persistence-is-trust.md) |

## 5 dimensions × 4 principles · 5 个维度 × 4 条原则

### I. Intent 立意 · Why build it

1. **Scenario-first · 场景先于功能** — start from real context, not feature list
2. **Spec before code · 先定性，再动手** — product doc is upstream of engineering
3. **Aesthetic as stance · 气质即立场** — color, type, voice are the first filter
4. **Subtitle as promise · 副标题是承诺** — "what you become," not "what you get"

### II. Boundary 边界 · What NOT to do

5. **Subtract, don't add · 做减法而非加法** — ask: in this scenario, does the user have patience
6. **Vision non-negotiable · 愿景不妥协，实现可妥协** — the floor is the vision, what's negotiable is the approach
7. **Product boundary = user's decision path · 产品边界 = 用户决策路径** — each feature does one thing, clearly
8. **Infrastructure mindset · Infrastructure 心智** — "can do" ≠ "should do"

### III. Execution 执行 · How to ship

9. **Decisive on direction, meticulous on detail · 决策果断，细节挑剔** — lock direction fast, never let details slide
10. **Borrow existing cognition · 借力已有认知** — borrow the memory, save innovation for what's felt, not seen
11. **Commander posture · 指挥者姿态** — AI is the executor, you set the direction
12. **Content standards > technical standards · 内容标准 > 技术标准** — the AI moat is your content judgment

### IV. Quality 品质 · How to make it stick

13. **End-to-end fixes · 端到端修复** — fix the whole path, not the symptom
14. **Design vs execution error · 设计错误 vs 执行错误** — diagnose the layer before choosing the fix
15. **Experience before review · 先用再评** — live use before listing problems, sample before trusting data
16. **Security = product quality · 安全 = 产品品质** — same queue as feature bugs, audit proactively

### V. Closed Loop 闭环 · When is it done

17. **Core metric bound to real engagement · 核心指标绑定真实投入** — one number that tells you if the product is working
18. **Persistence = trust · 持久化 = 信任基础** — what users invested, the product must remember
19. **Cross-platform parity + honest permissions · 跨端一致 + 权限诚实** — feature parity across platforms, clear boundaries
20. **Distribution is part of the product · 分发是产品的一部分** — done ≠ good, good ≠ reached

## Three-line compression · 三句话浓缩

**English:**
> **Intent holds firm:** scenario, aesthetic, vision — each articulable.  
> **Execution holds up:** decisive direction × meticulous detail.  
> **Loop closes:** it works → stands up to scrutiny → users can actually reach it.

**中文：**
> **立意定得住**：场景、气质、愿景都能说清楚。  
> **执行扛得住**：果断拍板 × 细节不放过。  
> **闭环做得到**：能跑起来 → 经得起推敲 → 用户真的能用到。

## Five questions to ask yourself every day · 五个每天该问自己的问题

1. Is the **scenario** for what I'm doing right now articulable? / 我现在做的这件事，**场景**说得清楚吗？
2. Can the features I recently added be **reverse-derived** from the scenario? / 我最近加的功能，**反推得出来**吗？
3. Working with AI — **am I commanding or being commanded**? / 和 AI 协作时，**我在指挥还是在被指挥**？
4. What is my product's **core metric**? What's the number today? / 我产品的**核心指标**是什么？现在数字是多少？
5. Can a **stranger actually reach** this product? Or do only I know it exists? / 这个产品**能被陌生人用到**吗？还是只有我知道它存在？
