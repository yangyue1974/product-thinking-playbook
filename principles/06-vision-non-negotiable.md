# 06 · Vision Non-Negotiable, Implementation Flexible

> **Implementation can be renegotiated. The product vision cannot be downgraded.**

## Core idea

When working with AI or engineering, the most dangerous pattern is: **"Technically hard to do" → "Then let's simplify" → the product's core value quietly dilutes.**

This is the deadliest trap, because every step sounds reasonable:
- Engineer says "can't be done" → drop one level → still works → seems OK

But "still works" ≠ "hit the target." Once the vision is downgraded, there's no coming back — you've started compounding on a wrong direction.

**The correct posture:**
- Vision is the **non-negotiable floor**
- Implementation is **fully open to negotiation** — stack, architecture, approach
- If current tools can't do it, ask "how long until they can," not "should we give up"

## In real projects

**Contra Code** — I shipped the game as a standalone Tab. User pushback:

> *"这和我想的不一样，跟他们在旁边开一个挖地雷有什么区别。"*

The weight of this line:
- They knew the original intent was "don't interrupt coding"
- Tab mode let them play, but lost the core value proposition
- They didn't accept a downgrade just because "tech said so"

Result: kept pushing on DOM injection → landed on bottom panel (compromised on implementation, but **kept "doesn't occupy the editor" as the core intent**).

**Xianxia** — On the mechanic "Chapter 15 writes straight through, no mid-way prompt," engineering wanted a "friendly prompt," but that would shatter the "immersive reading" vision. So engineering was paused until vision was confirmed.

## Anti-patterns

- **Technical difficulty used to kill vision:** "Can't do this, let's skip it" — "can't" is an implementation issue, not a reason to cancel vision.
- **"Users won't notice anyway"** — what users don't perceive is detail difference, not value difference.
- **Serial concessions:** give an inch here, an inch there, and by the end this isn't the product you wanted.

## Thinking formula

> When hearing "we can't do it," don't ask **"can we skip it."**  
> Ask **"can we do it a different way."**

**Three layers:**
- **Vision layer** (value proposition) → no compromise
- **Feature layer** (product form) → compromise carefully
- **Implementation layer** (technical approach) → compromise freely

## Related

- [02 · Spec before code](02-spec-before-code.md) — spec anchors the vision
- [11 · Commander posture](11-commander-posture.md)
- [14 · Design error vs execution error](14-design-vs-execution-error.md)

## Case studies

[Contra Code](../case-studies/contra-code.md) · [Xianxia](../case-studies/xianxia.md) · [Tarot](../case-studies/tarot.md)

---

# 06 · 愿景不妥协，实现可妥协

> **实现方案可以谈判，产品愿景不能让步。**

## 核心思想

和 AI / 工程团队协作时，最容易发生的退让是：**"技术上不好做"→"那就简化一下"→ 产品核心价值被悄悄稀释**。

这是最致命的陷阱。因为每一步都"合理"：
- 技术说实现不了 → 降一级实现 → 还能跑 → 好像也能接受

但"能跑"和"达到目标"是两回事。愿景一旦被降级，就再也回不去了——因为已经在错的方向上持续累积。

**正确姿态**：
- 愿景是**议价底线**，不在协商范围内
- 实现方式**完全可以谈**，可以换技术栈、换架构、换思路
- 如果现有工具做不到，问"要多久能做到"，而不是"要不要放弃"

## 在真实项目里长什么样

**Contra Code**：我把游戏做成了一个独立 Tab，用户直接反击：

> *"这和我想的不一样，跟他们在旁边开一个挖地雷有什么区别。"*

这句话分量很足：
- 他清楚原始意图是"不打断编程"
- Tab 模式让他能玩，但损失了核心价值主张
- 他没有因"技术上做不到"接受降级

结果：驱动继续研究 DOM 注入 → 最后落地在底部面板（技术上有妥协，但**保留了"不占用编辑器区域"的核心意图**）。

**Xianxia**：在「第 15 章直写到底、不设中途提示」这个机制上，工程更想做"友好提示"，但这会打碎"沉浸式阅读"的核心愿景。结果是先叫停讨论，确认愿景后再动手。

## 反模式

- **技术难度当愿景理由**："这个暂时做不到，先不做了" —— 做不到是实现问题，不是取消愿景的理由。
- **"反正用户也不会注意"** —— 用户感受不到的是细节差异，不是价值差异。
- **一路退让**：第一次让一点，第二次让一点，走到最后已经不是原来那个产品了。

## 思考公式

> 遇到"技术上做不到"，不问**"那我们能不能不做"**，  
> 问**"那我们能不能换个实现方式做到"**。

**三层结构**：
- **愿景层**（价值主张）→ 不妥协
- **功能层**（产品形态）→ 谨慎妥协
- **实现层**（技术方案）→ 可以随意妥协

## 延伸

- [02 · 先定性，再动手](02-spec-before-code.md) —— Spec 是愿景的锚
- [11 · 指挥者姿态](11-commander-posture.md)
- [14 · 设计错误 vs 执行错误](14-design-vs-execution-error.md)

## 相关案例

[Contra Code](../case-studies/contra-code.md) · [Xianxia](../case-studies/xianxia.md) · [Tarot](../case-studies/tarot.md)
