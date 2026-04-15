# 13 · End-to-End Fixes, Not Surface Patches

> **Fixing a bug isn't "making the symptom disappear." It's "making the path correct."**

## Core idea

Most bugs are not standalone events — they're **the visible symptom of several places on the same path being broken simultaneously**. Fixing only the visible one pushes the rest onto the next round.

Take "wrong redirect after login" as an example — on the surface, one file issue. Trace it, and you may find:
- `requireUser` drops the param
- auth page hardcodes the redirect
- `/api/login` hardcodes the redirect
- `/api/register` hardcodes the same
- No open-redirect protection

**Fix only the auth page → symptom gone.** But the rest of the path stays broken — it'll re-emerge as a different symptom next time.

**End-to-end fix:**
1. Trace the bug to its **root cause**, don't stop at the surface
2. Fix the **entire path**, not just the symptom location
3. While you're there, add **the protections that should have been there** (e.g., open-redirect guard)

## In real projects

**Spybook** — callbackUrl loss: surface was the wrong post-login redirect; root cause was the entire path — `requireUser`, `auth/page.tsx`, `api/login`, `register/page.tsx`, `api/register` — **none passed the param correctly**.

The fix didn't touch only one file — **all 5 files were fixed, plus open-redirect protection added.**

**Tarot** — AI replies kept truncating mid-sentence. Users thought the AI was being curt; the actual cause was `max_tokens` set too low.

> **The UI surface sits on top of a logic constraint, which sits on top of an infrastructure parameter.**

Diagnose experience problems down to the root, don't just patch the surface.

## Anti-patterns

- **Symptom → fix → done:** if the symptom goes away, you call it fixed.
- **Afraid of bigger changes:** you know the path has more issues, but "this time let's leave it, next time" — next time never comes.
- **No protection added:** only fix the specific bug, skip the related guardrails.
- **No regression sweep:** fix this bug, don't check if the same root cause triggers other bugs.

## Thinking formula

> Before fixing, ask:  
> **Are there other broken points upstream? Will the same root cause surface again downstream?**

**Three steps:**
1. Symptom → trace to root cause
2. Sweep the **entire path** from root to symptom for the same class of issue
3. Fix it all at once + add related protections

## Related

- [14 · Design error vs execution error](14-design-vs-execution-error.md)
- [15 · Experience before review](15-experience-before-review.md)
- [16 · Security = product quality](16-security-as-quality.md)

## Case studies

[Spybook](../case-studies/spybook.md) · [Tarot](../case-studies/tarot.md)

---

# 13 · 端到端修复，不修表面

> **修 bug 不是"让症状消失"，是"让这条链路正确"。**

## 核心思想

大多数 bug 不是独立事件，是某条**链路上多个点同时出错的外显**。只修最显眼的那个点，等于把其他错误推到下一次。

以"登录后跳转错误"为例——表面看是一个文件问题，追进去可能是：
- `requireUser` 丢失参数
- auth 页硬编码了回跳地址
- `/api/login` 硬编码了回跳地址
- `/api/register` 同样硬编码
- 没有 open redirect 防护

**只修 auth 页，症状消失了**。但链路上其他点依然是错的，下一次会以别的症状再冒出来。

**端到端修复**：
1. 追溯问题到**根因**，不停在表面
2. 修**整条链路**，不只修症状位置
3. 顺便补上应该有的**保护**（如 open redirect 防护）

## 在真实项目里长什么样

**Spybook** · callbackUrl 丢失：问题表面是 login 后跳错页，根因是整条链路——`requireUser`、`auth/page.tsx`、`api/login`、`register/page.tsx`、`api/register`——**都没有正确传递这个参数**。

修复时没有只改一个文件，而是**把 5 个文件全部修完，同时加上 open redirect 防护**。

**Tarot** · AI 对话总是中途截断。用户以为是 AI 在敷衍，实际上是 `max_tokens` 设置太低。

> **UI 层的表现背后是逻辑层的约束，逻辑层的约束背后是基础设施层的参数。**

诊断体验问题要追到根因，不要只修表面现象。

## 反模式

- **头痛医头**：症状消失就算修好。
- **怕改动大**：明知链路上还有问题，但"这次先不动了，下次再说"——下次永远不会来。
- **不补防护**：只修当前 bug，不顺手加上相关的边界保护。
- **不做回归**：修了这个 bug，没有检查"同一个根因会不会引发别的 bug"。

## 思考公式

> 修 bug 之前问一句：  
> **这个 bug 的上游还有没有出错的点？下游会不会因为同样原因再出一次？**

**三步**：
1. 定位症状 → 追到根因
2. 在根因到症状的**整条链路**上找同类问题
3. 一次性修完 + 补相关防护

## 延伸

- [14 · 设计错误 vs 执行错误](14-design-vs-execution-error.md)
- [15 · 先用再评](15-experience-before-review.md)
- [16 · 安全 = 产品品质](16-security-as-quality.md)

## 相关案例

[Spybook](../case-studies/spybook.md) · [Tarot](../case-studies/tarot.md)
