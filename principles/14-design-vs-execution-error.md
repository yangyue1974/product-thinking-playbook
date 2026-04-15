# 14 · Design Error vs Execution Error

> **When you hit a problem, first tell: is this an execution-layer error, or a design-layer error? Execution errors get code fixes. Design errors get direction fixes.**

## Core idea

Not all bugs live on the same layer. Telling them apart is itself a product skill:

| Layer | Symptom | Fix |
|---|---|---|
| **Execution error** | Code is wrong, feature doesn't match the design | Fix the code |
| **Design error** | Feature matches the design, but the design itself is wrong | Fix the direction |

**Treating a design error as an execution error only makes things more complex — the root problem never goes away.** Every fix just piles more onto the wrong direction.

**Signals to look for:**
- Fixed 3 times, still seeing similar issues → likely a design error
- Engineer fixed a bug, but product still feels "off" → likely a design error
- User says "it works, but something's wrong" → likely a design error

## In real projects

**Tarot** — The "draw again" feature:

The AI suggested "draw again" but the next reading completely ignored prior conversation. Engineering read this as an **implementation problem** (context not passed correctly). Product defined it as a **design error**:

> *"这不是某行代码写错了，是对'再次抽牌'这个功能的理解从根本上错了。工程实现了一个不符合产品逻辑的功能，补丁不解决问题，要从设计层重新理解这个功能是什么。"*

Redefined: "draw again" means **deepen the current consult**, not switch topics. Once the design was right, the implementation fell into place.

**Contra Code** — I shipped the game as a standalone Tab. It worked, but user feedback:

> *"这和我想的不一样，跟他们在旁边开一个挖地雷有什么区别。"*

The Tab approach was a **design-layer error** — vision is "don't interrupt coding," but Tab mode interrupts. The Tab implementation wasn't bad; the Tab approach itself was directionally wrong.

## Anti-patterns

- **Treating every issue as a bug:** see an error, fix it, never question why it was designed this way.
- **Piling complexity via patches:** design has a problem, you work around it with if-else, code gets more tangled, new bugs appear.
- **Never revisiting the design:** "the design doc was written, that's final" — no room for direction correction.

## Thinking formula

> Is this bug **"design right, execution wrong"**, or **"execution right, design wrong"**?  
> Former: fix code. Latter: fix direction.

**Identification checklist:**
1. Under the current design, is this bug *inevitable*? → yes = design error
2. After fixing this bug, will similar issues re-emerge in different forms? → yes = design error
3. Fix cost vastly greater than feature value? → consider if the design itself is wrong

## Related

- [06 · Vision non-negotiable](06-vision-non-negotiable.md)
- [07 · Product boundary](07-product-boundary.md)
- [13 · End-to-end fixes](13-end-to-end-fixes.md)

## Case studies

[Tarot](../case-studies/tarot.md) · [Contra Code](../case-studies/contra-code.md)

---

# 14 · 设计错误 vs 执行错误

> **遇到问题，先判断是"执行层错误"还是"设计层错误"。执行错误修代码，设计错误改方向。**

## 核心思想

不是所有 bug 都在一个层面上。分清楚这件事本身就是产品能力：

| 层级 | 表现 | 修复方式 |
|---|---|---|
| **执行层错误** | 代码写错了，功能没按设计跑 | 改代码 |
| **设计层错误** | 功能按设计跑了，但设计本身是错的 | 改方向 |

**把设计层错误当执行层错误修，只会越修越复杂，根本问题不会消失。** 因为每次修都是在错的方向上继续叠加。

**识别信号**：
- 修了 3 次还在出类似问题 → 可能是设计错误
- 工程师修了一个 bug，产品却觉得"不对劲" → 可能是设计错误
- 用户反馈"能用，但总感觉哪里不对" → 可能是设计错误

## 在真实项目里长什么样

**Tarot** · "再次抽牌"功能：

AI 建议用户"再次抽牌"，但新一轮解读完全忽略了此前的对话。工程侧把这理解为**实现问题**（上下文没传好），产品侧定义为**设计错误**：

> *"这不是某行代码写错了，是对"再次抽牌"这个功能的理解从根本上错了。工程实现了一个不符合产品逻辑的功能，补丁不解决问题，要从设计层重新理解这个功能是什么。"*

重新定义之后："再次抽牌"的语义是**深入当前咨询**，不是切换话题。重新设计之后，实现自然就对了。

**Contra Code** · 我把游戏做成独立 Tab。工程上可以工作，但用户反馈：

> *"这和我想的不一样，跟他们在旁边开一个挖地雷有什么区别。"*

Tab 方案是**设计层错误**——愿景是"不打断编程"，Tab 模式打断了。不是 Tab 实现不好，是 Tab 本身方向错了。

## 反模式

- **把所有问题当 bug 修**：看见报错就修，不问为什么会这么设计。
- **用补丁堆出复杂度**：设计层有问题，靠一堆 if-else 绕开，代码越来越复杂，新 bug 越来越多。
- **从不回头看设计**：认为"设计文档已经写了"就是最终答案，不接受方向调整。

## 思考公式

> 这个 bug，**是"设计对但执行错"**，还是**"执行对但设计错"**？  
> 前者修代码，后者改方向。

**识别清单**：
1. 按照当前设计，这个 bug 是不是必然会出现？→ 是 = 设计错误
2. 修完这个 bug，同类问题还会不会以别的形式再出现？→ 是 = 设计错误
3. 修复成本远大于功能价值？→ 考虑是不是设计本身就错了

## 延伸

- [06 · 愿景不妥协](06-vision-non-negotiable.md)
- [07 · 产品边界 = 用户决策路径](07-product-boundary.md)
- [13 · 端到端修复](13-end-to-end-fixes.md)

## 相关案例

[Tarot](../case-studies/tarot.md) · [Contra Code](../case-studies/contra-code.md)
