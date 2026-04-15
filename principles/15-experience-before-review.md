# 15 · Experience Before Review, Don't Trust Defaults

> **Lived experience is more valuable than an imagined list of problems. AI defaults must be actively verified.**

## Core idea

Two ideas folded into one, because they share the same underlying logic:
- **Experience before review:** don't worry about problems in the abstract — go use the thing, then list problems.
- **Don't trust defaults:** AI / tool default outputs must be verified, don't assume "should be correct."

**Shared logic:** don't over-simulate in your head. Ship fast and get real feedback.

- No matter how good a feature sounds, you don't know where it jams until you use it
- AI-generated links / data look real, one click might be a 404
- "Close enough" and "actually works" are gaps only real usage reveals

## In real projects

**Contra Code** — Every iteration follows this rhythm:

1. Ship new version
2. Actually play for a while
3. Report **specific** problems (often several at once)

> *"人物和物品没抠图，必须抠图，火苗都抠图了，是正常的，枪械包似乎是半透明，有个透明框。"*

Only playing surfaces three distinct problems at once.

**Gospel Hub** — Skeptical of AI-generated content:

> *"苹果、Spotify 和 YouTube 的链接都是错的和假的。"*  
> *"我手动检查了一遍，这么多歌手的苹果和 Spotify 链接是假的。"*

Required **HTTP-level verification of every link**, didn't trust search results. Stay alert to what users will actually see — one 404 destroys trust.

## Anti-patterns

- **Imagined problem list:** worry about "what if X happens" for hours, then ship and find the real problems were elsewhere.
- **"If AI said so":** accept AI-given content / links as-is, no sampling.
- **Only testing happy path:** you only click through the perfect path, skip edge cases, ship, first user goes off-path, crashes.
- **"Works in dev" = done:** never used it in real environment / on a real device, called it done.

## Thinking formula

> **Have you actually used it?** → if not, don't say "should be fine."  
> **Have you sampled and verified?** → if not, don't say "AI-generated should be correct."

**Two habits:**
1. After every "done," **act as a real user for 5 minutes**. List concrete problems, not "possible problems."
2. For every batch of AI-generated data / content, **randomly sample 3–5 items for verification**. One wrong → re-verify the batch.

## Related

- [09 · Decisive & meticulous](09-decisive-and-meticulous.md)
- [11 · Commander posture](11-commander-posture.md)
- [13 · End-to-end fixes](13-end-to-end-fixes.md)

## Case studies

[Contra Code](../case-studies/contra-code.md) · [Gospel Hub](../case-studies/gospel-hub.md)

---

# 15 · 先用再评，不信任默认

> **真实体验比想象中的问题清单更有价值。AI 的默认输出必须主动验证。**

## 核心思想

两件事合并在一起：
- **先用再评**：不担心可能的问题，真玩一会儿再列问题。
- **不信任默认**：AI / 工具的默认输出要主动验证，不相信"应该是对的"。

这两件事的共同逻辑是：**别在脑子里过度推演，上线最快反馈**。

- 功能再好，自己没玩过就不知道卡在哪里
- AI 生成的链接/数据看着像真的，随手点一下可能就是 404
- "差不多能用"和"真能用"之间的差距，只有亲自走一遍才知道

## 在真实项目里长什么样

**Contra Code** · 每轮迭代都是这个节奏：

1. 上线新版本
2. 真玩一会儿
3. 反馈**具体**问题（经常一次好几个）

> *"人物和物品没抠图，必须抠图，火苗都抠图了，是正常的，枪械包似乎是半透明，有个透明框。"*

玩过才能同时发现三个不同的问题。

**Gospel Hub** · 对 AI 生成的内容保持怀疑：

> *"苹果、Spotify 和 YouTube 的链接都是错的和假的。"*
> *"我手动检查了一遍，这么多歌手的苹果和 Spotify 链接是假的。"*

要求用 HTTP 请求**逐个验证**，而不是相信搜索结果。对用户会看到的东西保持警觉——用户点进去发现是 404 就毁了信任。

## 反模式

- **想象中的问题清单**：在脑子里担心"会不会出 xx 问题"，折腾好久，结果上线后真正的问题根本不在那里。
- **AI 说好就是好**：AI 给了一份内容/一串链接，直接用上，不抽查。
- **Demo 阶段只做 happy path**：自己只点完美路径，没试边界情况，上线后用户一走歪就崩。
- **"开发环境能跑"就算完**：没在真实环境/真机上用过，就当做完。

## 思考公式

> **真用过没有？** → 没用过就不要说"应该没问题"。  
> **抽样验证过没有？** → 没验证过就不要说"AI 生成的应该对"。

**两步习惯**：
1. 每次"做完"之后，**自己当 5 分钟真实用户**。列具体问题，不列"可能问题"。
2. 每批 AI 生成的数据/内容，**随机抽 3-5 条验证**。一条错，全部重新校验。

## 延伸

- [09 · 决策果断，细节挑剔](09-decisive-and-meticulous.md)
- [11 · 指挥者姿态](11-commander-posture.md)
- [13 · 端到端修复](13-end-to-end-fixes.md)

## 相关案例

[Contra Code](../case-studies/contra-code.md) · [Gospel Hub](../case-studies/gospel-hub.md)
