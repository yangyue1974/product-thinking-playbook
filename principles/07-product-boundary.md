# 07 · Product Boundary = User's Decision Path

> **Every feature should do one thing, clearly. Features with fuzzy boundaries force users to guess.**

## Core idea

A product's boundary isn't drawn in the user manual. It's drawn **before every click** a user makes. Each feature should answer one question cleanly in the user's head: **"what will pressing this do?"**

- "Draw again" = continue the current reading / or switch topics?
- "Back" = back to previous page / or exit session?
- "Delete" = soft delete / or permanent?

Once a boundary is fuzzy, every action carries uncertainty — and trust erodes quietly.

**Clear boundaries come from clear understanding of the user's decision path**, not from "what this button can technically do."

## In real projects

**Tarot** — The AI suggested "draw again" in conversation; the next reading completely ignored prior context. Engineering read this as an implementation problem. Product defined it as a **design error**:

> *"'再次抽牌' is for going deeper into the current reading, not for switching to a new topic. If the user wants to consult something else, they should start a new session. That's the product boundary."*

Once clarified, "draw again" had a crisp boundary: **deeper, not sideways**.

**Xianxia** — Auto-starting Arc 2 is a good mechanism, but it shouldn't be the only exit. Different users have different intent, so a third option — *"Return to shelf · start a new saga"* — was added. But **auto-continue remained the default path**; user choice is the "escape hatch," not a replacement for the main road. Primary vs. secondary is clear → boundary is clear.

## Anti-patterns

- **Fuzzy semantics:** one button doing several things, context-dependent.
- **No escape hatch:** user went wrong, can't get back.
- **Unclear defaults:** no explicit action, but system did something "for them" without telling.
- **Over-confirming:** every node pops "are you sure?" — this isn't respecting choice, it's dodging decisions.

## Thinking formula

> Before a user clicks — **what question is in their head?**  
> Does my feature **answer exactly that question**?

**Two checks:**
1. Same button, different users — do they expect different things? If yes, split it.
2. For a feature: which is the "default path" and which is the "escape hatch"? Any conflict between them?

## Related

- [05 · Subtract, don't add](05-subtraction-over-addition.md)
- [14 · Design error vs execution error](14-design-vs-execution-error.md)
- [19 · Cross-platform parity + honest permissions](19-honest-parity.md)

## Case studies

[Tarot](../case-studies/tarot.md) · [Xianxia](../case-studies/xianxia.md)

---

# 07 · 产品边界 = 用户决策路径

> **每个功能都应该只做一件事，做清楚。边界模糊的功能，用户就要靠猜来使用。**

## 核心思想

产品边界不是在用户手册里画的，是在**用户每一次点击前**画的。每个功能在用户头脑里都应该回答一个明确的问题："**我点了这个会怎样**？"

- "再抽一次" = 延续当前咨询 / 还是切换话题？
- "返回" = 返回上一页 / 还是退出会话？
- "删除" = 软删除 / 还是永久删除？

边界一旦模糊，用户的每一次操作都带着不确定感，信任会慢慢损耗。

**边界的清晰，来自对用户决策路径的清晰理解**。不是"这个按钮能做的事"，而是"用户在这一步到底想做什么"。

## 在真实项目里长什么样

**Tarot**：AI 在对话中建议"再次抽牌"，然后新一轮解读完全忽略了此前的对话。工程侧把这理解为"实现问题"，产品侧定义为"**设计错误**"。

> *"再次抽牌是为了深入当前咨询话题，不是为了切换到其他话题。用户如果想咨询别的事，应该开一个新的推演——这是产品边界。"*

澄清之后，"再次抽牌"的边界明确了：**深入，不是切换**。

**Xianxia**：Arc 2 的自动开启是好机制，但不能是唯一出口。不同用户有不同意图，于是增加第三个选项"返回书架·另起新传"——但**自动推进仍然是默认路径**，用户选择是"逃生口"，不是替代主路径。主次清晰，边界就清晰。

## 反模式

- **功能语义模糊**：一个按钮做多件事，靠上下文判断。
- **没有"逃生口"**：用户走错路想退回来，找不到路径。
- **默认行为不明**：用户没明确操作时，系统替用户做了决定，但没告诉用户。
- **把用户选择变成干扰**：每个节点都弹窗问"你确定吗" —— 这不是尊重选择，是推卸决策。

## 思考公式

> 用户点击之前，**脑子里在问什么问题**？  
> 我这个功能，**能精确回答这个问题吗**？

**两条检查**：
1. 同一个按钮，不同用户是否有不同预期？如果有，就需要拆分。
2. 功能的"默认路径"和"逃生口"，哪个是主，哪个是辅？两者有没有冲突？

## 延伸

- [05 · 做减法而非加法](05-subtraction-over-addition.md)
- [14 · 设计错误 vs 执行错误](14-design-vs-execution-error.md)
- [19 · 跨端一致 + 权限诚实](19-honest-parity.md)

## 相关案例

[Tarot](../case-studies/tarot.md) · [Xianxia](../case-studies/xianxia.md)
