# 12 · Content Standards > Technical Standards (for AI Products)

> **The moat of an AI product isn't "which model you use." It's your judgment about content quality.**

## Core idea

When everyone can call the same model APIs, **there's no technical differentiation** between AI products. The real gap opens up from:

1. How fine-grained your content-quality standards are
2. How much of that standard you can encode into prompt / system message / output constraints

"Content standards" are much harder to define than "technical standards" — technical standards are quantifiable (response < 200ms), content standards can only be felt ("no summary sentences," "must have a sense of process").

**People who can articulate content standards clearly are the ones who build AI products with actual quality.** It's a scarce kind of intuition — not an engineering skill, but a literary / aesthetic / narrative skill.

This doesn't only apply to text generation:
- Image generation: composition / lighting / texture constraints in prompts
- Audio generation: style / mood / density constraints
- Conversational AI: **what role does the AI play** — advisor? judge? teacher? companion?

## In real projects

**Xianxia** — Style constraints far more precise than technical requirements:

> *"仿照《凡人修仙传》早期叙事风格…… 禁止总结句，禁止抽象评价，要求过程感，字数控制在 1800–3000 字。"*

These standards directly determine the quality ceiling of the core experience. Same model, different standards, vastly different output.

**Tarot** — Role definition decides everything:

> *"Users come to Tarot because they're facing a question they haven't thought through. If the AI rushes to conclusions, it's interrupting their thinking, not helping."*

Changing the AI from "judge" to "guide" is one line in the prompt — but it changes the soul of the product:
- If the situation isn't clear, ask questions first — understand before advising
- When the cards point to difficulty, focus on "what can be done next," don't linger on the problem itself
- Acknowledge the user's judgment and feelings — understand first, then discuss; don't negate, don't overturn

## Anti-patterns

- **"Built on GPT-4 / Claude 4 / latest model" as a selling point:** users don't care about model versions, they care about content quality.
- **Prompts written like manuals:** *"Please help me generate…"* — generic prompt, average output.
- **Tuning prompts after user feedback:** launched, users said "it's boring," now you go tune. Too late.
- **Engineers writing prompts:** get "competent but lifeless" content.

## Thinking formula

> AI product competitiveness = **model capability** × **your content standard**.  
> Model capability is the same for everyone, so it's all in the second factor.

**Two self-checks:**
1. Can I list **10 clear content don'ts** (must not appear) and **10 clear content musts** (must appear)?
2. What role is my AI playing? Can I describe that role's speech style, thinking mode, and value leanings in one paragraph?

## Related

- [03 · Aesthetic as stance](03-aesthetic-as-stance.md)
- [04 · Subtitle as promise](04-subtitle-as-promise.md)
- [11 · Commander posture](11-commander-posture.md)

## Case studies

[Xianxia](../case-studies/xianxia.md) · [Tarot](../case-studies/tarot.md)

---

# 12 · 内容标准 > 技术标准（AI 产品）

> **AI 产品的护城河不在于"用了什么模型"，而在于"对内容品质的判断力"。**

## 核心思想

当所有人都能调用同样的模型 API，AI 产品之间**技术栈没有差异**。真正拉开差距的是：

1. **你对内容品质的标准有多细**
2. **你能把这个标准写进 Prompt / 系统提示 / 内容约束里多少**

"内容标准"比"技术标准"难定义得多——技术标准可以量化（响应时间 < 200ms），内容标准只能感受（"不要有总结句"、"要有过程感"）。

**能把内容标准写清楚的人，才能做出有品质的 AI 内容产品。** 这是一种稀缺的内容直觉，它不是工程能力，是文学/审美/叙事的能力。

这条原则不只适用于文本生成类产品：
- 图像生成：prompt 里的构图、光线、质感约束
- 音频生成：风格、情绪、密度约束
- 对话类 AI：**AI 扮演什么角色**（顾问？判官？老师？陪伴？）

## 在真实项目里长什么样

**Xianxia**：对 AI 写作风格的要求远比技术需求精细。

> *"仿照《凡人修仙传》早期叙事风格…… 禁止总结句、禁止抽象评价、要求过程感，字数控制在 1800–3000 字。"*

这些标准直接决定了产品核心体验的质量上限。同样的模型，标准不同，产出天差地别。

**Tarot**：角色定位决定一切。

> *"用户来做塔罗咨询，是因为他们面对一个还没想清楚的问题。AI 如果急着下结论，实际上是在打断用户的思考过程，而不是帮助他们。"*

把 AI 从"判官"改成"引导者"，改的是 Prompt 里一句话，但改的是产品的灵魂：
- 处境不清楚，先问问题，搞清楚再给建议
- 当牌面指向困难，重心放在"接下来可以怎么做"，不停在问题本身
- 认可用户的判断和感受，先理解再探讨，不否定不推翻

## 反模式

- **"用了 GPT-4 / Claude 4 / 最新模型"当卖点**：对用户来说，模型型号没意义，内容质量才有意义。
- **Prompt 写得像说明书**："请帮我生成……"—— 这种 Prompt 只会得到平均水平的输出。
- **内容标准靠用户反馈倒推**：上线后用户说"没意思"，你才回头调 Prompt —— 太晚了。
- **技术团队负责内容**：工程师写 Prompt，结果生成的是"合格但无趣"的内容。

## 思考公式

> AI 产品的竞争力 = **模型能力** × **你的内容标准**。  
> 模型能力大家都一样，所以全部看后半段。

**两问自检**：
1. 我能列出 **10 条明确的内容禁忌**（不能出现什么）和 **10 条明确的内容要求**（必须出现什么）吗？
2. 我的 AI 在扮演一个什么角色？这个角色的说话腔调、思考方式、价值倾向，我能不能用一段话描述？

## 延伸

- [03 · 气质即立场](03-aesthetic-as-stance.md)
- [04 · 副标题是承诺](04-subtitle-as-promise.md)
- [11 · 指挥者姿态](11-commander-posture.md)

## 相关案例

[Xianxia](../case-studies/xianxia.md) · [Tarot](../case-studies/tarot.md)
