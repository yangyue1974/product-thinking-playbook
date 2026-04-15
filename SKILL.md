---
name: product-thinking-playbook
description: A decision-making playbook for solo product builders. 20 principles across 5 dimensions — Intent, Boundary, Execution, Quality, Closed Loop — extracted from 6 shipped products. Use when starting a new product, stuck on a product decision, reviewing your own work, or collaborating with an AI coder who can write anything but doesn't know what to build.
---

# Product Thinking Playbook

> 一套给独立开发者 / 产品人的判断框架。  
> 不是"产品经理手册"，是把"做决策的那一刻在想什么"写下来。

## 什么时候用这个 skill

在以下时刻主动打开对应的原则文件阅读再做决定：

- **新产品立项** → 读 `principles/01-scenario-first.md` → `principles/02-spec-before-code.md`
- **功能蔓延、收不住手** → 读 `principles/05-subtraction-over-addition.md`
- **和 AI 协作写代码，感觉产品在跑偏** → 读 `principles/11-commander-posture.md`
- **拿到一批 bug，不知道从哪下手** → 读 `principles/13-end-to-end-fixes.md` + `14-design-vs-execution-error.md`
- **产品"能跑了"，下一步该做什么** → 读 `principles/17-real-engagement-metrics.md` + `20-distribution-is-product.md`
- **快速查阅** → `quick-reference.md`

## 五个维度

| 维度 | 回答的问题 | 对应原则 |
|---|---|---|
| **I. 立意 Intent** | 为什么存在？为谁做？ | 01–04 |
| **II. 边界 Boundary** | 不做什么？边界在哪？ | 05–08 |
| **III. 执行 Execution** | 怎么把判断落地？ | 09–12 |
| **IV. 品质 Quality** | 怎么让它站得住？ | 13–16 |
| **V. 闭环 Closed Loop** | 什么时候算做完？ | 17–20 |

## 20 条原则索引

**I. 立意**
1. [场景先于功能](principles/01-scenario-first.md)
2. [先定性，再动手](principles/02-spec-before-code.md)
3. [气质即立场](principles/03-aesthetic-as-stance.md)
4. [副标题是承诺，不是描述](principles/04-subtitle-as-promise.md)

**II. 边界**
5. [做减法而非加法](principles/05-subtraction-over-addition.md)
6. [愿景不妥协，实现可妥协](principles/06-vision-non-negotiable.md)
7. [产品边界 = 用户决策路径](principles/07-product-boundary.md)
8. [克制：不是基础设施该做的，别做](principles/08-infrastructure-mindset.md)

**III. 执行**
9. [决策果断，细节挑剔](principles/09-decisive-and-meticulous.md)
10. [借力已有认知](principles/10-borrowed-cognition.md)
11. [指挥者姿态，不做被动执行](principles/11-commander-posture.md)
12. [内容标准 > 技术标准（AI 产品）](principles/12-content-standards-first.md)

**IV. 品质**
13. [端到端修复，不修表面](principles/13-end-to-end-fixes.md)
14. [设计错误 vs 执行错误](principles/14-design-vs-execution-error.md)
15. [先用再评，不信任默认](principles/15-experience-before-review.md)
16. [安全 = 产品品质](principles/16-security-as-quality.md)

**V. 闭环**
17. [核心指标绑定真实投入](principles/17-real-engagement-metrics.md)
18. [持久化 = 信任基础](principles/18-persistence-is-trust.md)
19. [跨端一致 + 权限诚实](principles/19-honest-parity.md)
20. [分发是产品的一部分](principles/20-distribution-is-product.md)

## 案例底座

这 20 条不是凭空写的。每一条都能在下面 6 个真实项目里找到原始对话和决策时刻：

- [Contra Code](case-studies/contra-code.md) · VS Code 内嵌游戏浮层
- [AudioLib](case-studies/audiolib.md) · 开发者用的音频库服务
- [Gospel Hub](case-studies/gospel-hub.md) · 福音音乐聚合站
- [Spybook](case-studies/spybook.md) · 互动侦探叙事小说
- [Tarot](case-studies/tarot.md) · AI 塔罗咨询
- [Xianxia](case-studies/xianxia.md) · AI 仙侠小说生成

## 使用方式

```
在 Claude Code 里：
> 用 product-thinking-playbook 帮我判断一下：
> 现在这个功能要不要加？

在人自己脑子里：
> 对着 quick-reference 念一遍，找"最刺痛自己"那条。
```

---

## 三个核心姿态

把 20 条再压成 3 句话：

> **1. 立意定得住：场景、气质、愿景都能说清楚，别人改一字都不舒服。**  
> **2. 执行扛得住：果断拍板 × 细节不放过，自己是指挥者不是乙方。**  
> **3. 闭环做得到：能跑起来 → 经得起推敲 → 用户真的能用到。**

---

*基于 6 个已上线产品的全过程对话提炼 · 2026.04*  
*作者 [@yangyue1974](https://github.com/yangyue1974) · [43.group](https://43.group)*
