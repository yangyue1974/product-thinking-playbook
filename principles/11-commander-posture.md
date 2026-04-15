# 11 · Commander Posture — Don't Be the Passive Executor

> **AI is the executor. You are the direction-setter. Reviewing AI output is your job — not something the AI picks up on its own.**

## Core idea

When collaborating with AI on code, the trap is **passive execution**:
- AI says it can → OK, do it
- AI writes a version → OK, that's it

This is handing over product decision authority. AI doesn't have your judgment about the product; it will default to what seems "most generic, most reasonable" — and "generic" is exactly why products end up bland.

**Four traits of commander posture:**
1. **Give explicit output specs**, not vague directives. *"Write 50 of the most influential US contemporary Gospel artists,"* not *"help me list some artists."*
2. **Review and correct** — I edit the list AI gives me, I don't accept it wholesale.
3. **Challenge AI suggestions** — don't be convinced by "the AI said so," counter-question: *"Really? Evidence?"*
4. **Bluntly call out errors** — clear feedback is what lets AI course-correct quickly.

**Commander ≠ dictator.** AI is sometimes better than you (at writing code, handling details). Let that part go. But **direction and quality standards don't get delegated.**

## In real projects

**Gospel Hub** —
- Explicit output spec: *"Write 50 of the most influential US contemporary Gospel artists and bands"*
- Review and correct (cut Vertical Worship, Todd Dulaney, Koryn Hawthorne, Sinach; added NF; later added Hope Darst)
- Challenge AI suggestions: *"Vercel seems to need a deployment first to monitor data"*, *"this port is occupied"*
- Direct when AI errs: *"You didn't give me code"*

**Spybook** — Facing 14 bugs, no debate about "which are worth fixing." Straight:

> *"全部都要修，你按计划步骤做吧。"*

Classic commander posture: **direction is set, execution doesn't need discussion.**

## Anti-patterns

- **"Whatever AI gives, I'll use":** no review habit, trusting "AI should know what's right."
- **Talked into it by AI confidence:** AI says *"this is usually how it's done,"* you accept. You didn't ask *"but does that really fit my scenario?"*
- **Polite when AI is wrong:** *"Hmm, maybe I didn't phrase it clearly..."* — saying plainly *"you're wrong"* is what lets AI correct.
- **No spec in the question:** *"help me optimize this"* — optimize in what direction? what's better? AI can only guess.

## Thinking formula

> **I set direction. You write details.**  
> **I review output. You fix errors.**

**One test:** look at the AI's last output and **find at least 3 things you'd change**. Can't find any? Either you didn't read carefully, or your product standards aren't clear enough yet.

## Related

- [02 · Spec before code](02-spec-before-code.md) — spec is the commander's baton
- [06 · Vision non-negotiable](06-vision-non-negotiable.md)
- [15 · Experience before review](15-experience-before-review.md)

## Case studies

[Gospel Hub](../case-studies/gospel-hub.md) · [Spybook](../case-studies/spybook.md) · [Contra Code](../case-studies/contra-code.md)

---

# 11 · 指挥者姿态，不做被动执行

> **AI 是执行者，你是方向指挥者。审查 AI 输出是你的责任，不是 AI 自己会担起来的。**

## 核心思想

和 AI 协作写代码，最容易陷入的状态是**被动执行**：
- AI 说可以做 → 好，那就做
- AI 写完一版 → 好，那就这样

这是把"产品决策权"拱手让出。AI 没有你对产品的判断力，它只会按照自己认为"最通用、最合理"的方式做——而"通用"恰好是产品没有特点的原因。

**指挥者姿态** 的四个特征：
1. **明确给产出规格**，不是模糊描述（"写 50 位最重要的美国当代福音歌手"，不是"帮我列一些歌手"）
2. **审阅并修正**，AI 给的清单我自己删改，不是照单全收
3. **挑战 AI 的建议**，不被"它说的"说服，会反问"真的吗？有依据吗？"
4. **不客气地指出错误**，明确反馈才能让 AI 迅速纠正

**指挥者不等于独裁者**。AI 有时候比你强（比如写代码、处理细节），那部分要放手。但**方向和品质标准不能放手**。

## 在真实项目里长什么样

**Gospel Hub**：
- 明确产出规格："写 50 位最重要的美国当代福音歌手和乐队"
- 审阅并修正（删掉 Vertical Worship、Todd Dulaney、Koryn Hawthorne、Sinach，加了 NF，后来又加 Hope Darst）
- 挑战 AI 建议："Vercel 好像需要部署才能监测数据"、"这个端口被占用了"
- 在 AI 做错时直接指出："你没给我代码啊"

**Spybook**：面对 14 个 bug，没有讨论"哪些值得修"，直接：**全部修**。

> *"全部都要修，你按计划步骤做吧。"*

这是典型的指挥者姿态：**方向已定，执行无需讨论**。

## 反模式

- **"AI 给什么我用什么"**：对 AI 输出缺少审查习惯，相信"AI 应该知道对的做法"。
- **被 AI 的自信说服**：AI 说"这个功能通常是这么做的"，你就接受了，没问"我们的场景里真的该这么做吗"。
- **AI 出错时客气**："好像不太对哦，可能是我说的不清楚"——明确说"你错了"才能让 AI 纠正。
- **没有规格的提问**："帮我优化一下这个" —— 优化方向是什么？好在哪？AI 只能瞎猜。

## 思考公式

> **方向我定，细节你写。**  
> **产出我审，错了你改。**

**一测**：看 AI 给的最后一版输出，**至少找出 3 个你认为可以改得更好的点**。找不出来，要么你没认真看，要么你对产品标准还不够清晰。

## 延伸

- [02 · 先定性，再动手](02-spec-before-code.md) —— Spec 是给 AI 的指挥棒
- [06 · 愿景不妥协](06-vision-non-negotiable.md)
- [15 · 先用再评](15-experience-before-review.md)

## 相关案例

[Gospel Hub](../case-studies/gospel-hub.md) · [Spybook](../case-studies/spybook.md) · [Contra Code](../case-studies/contra-code.md)
