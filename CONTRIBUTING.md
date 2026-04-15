# CONTRIBUTING · 如何扩充这本 Playbook

这不是传统的开源贡献指南。这是**给未来的自己**——每做一个新产品，怎么把它变成这本 playbook 的新一页。

---

## 新增一个案例（做完一个产品之后）

### Step 1 · 写 case study

在 `case-studies/` 下新建 `<product-slug>.md`，用**统一模版**：

```markdown
# [Product Name] · 产品思维案例

> 一句话产品描述（产品形态 + 解决的问题）
> 从 [Project Name] 项目全过程对话提炼 · YYYY-MM

---

## 一、[决策片段简称]

> *"原话引用（如有）"*

[2-3 段叙述：当时在什么场景下做了什么决策，为什么这么判断]

**原则：** [浓缩成一句可迁移的原则]

---

## 二、[决策片段简称]

...重复上面的结构...

---

*提炼自 [Project Name] 项目全过程对话 · YYYY-MM*
```

**写作要点：**
- 每一节聚焦**一个具体的决策时刻**，不是"我学到了什么"的反思
- 尽量引用当时的**原话**（自己的 / 对方的），原话比总结更有分量
- `**原则：**` 必须能脱离这个项目独立成立——如果必须带项目名才能理解，说明还没提炼到位
- 章节数不限，但每一节都应该是"无它不可"的——可删则删

### Step 2 · 和已有原则对照

打开 `principles/` 下的 20 条，对照新 case study 里的决策：

- **已经被覆盖？** → 只在 case study 里记录，不改 principles
- **是现有原则的新佐证？** → 在对应 principle 文件的"相关案例"段落里加上新项目
- **确实是一条新原则？** → 进 Step 3

### Step 3 · 提炼新原则（仅在确实必要时）

保守一点——**至少 3 个以上项目**都出现过同一种判断，才值得升级为新的 principle。否则放在 case study 里就好。

新原则加入时：
1. 在 `principles/` 新建 `NN-kebab-name.md`（编号续上）
2. 用统一模版（见下方"Principle 模版"）
3. 更新 `SKILL.md` 的索引
4. 更新 `README.md` 的 20 条速览
5. 更新 `quick-reference.md` 的症状→原则对照表
6. 更新 `case-studies/README.md` 的原则反查表

### Step 4 · 更新 case-studies/README.md

在表格里加一行：

```markdown
| [Product Name](product-slug.md) | 产品形态 | 核心提炼出的原则 |
```

并在"原则索引 → 案例"里把新项目加到相关原则下。

### Step 5 · 提交

```bash
git add .
git commit -m "Add case study: [Product Name]"
git push
```

---

## Principle 模版

如果真的要新增一条原则，这是标准模版：

```markdown
# NN · [原则名]

> **[一句话版本]**

## 核心思想

[2-3 段阐述这条原则的内涵，以及为什么重要]

## 在真实项目里长什么样

**[Project A]**：...

> *"原话引用"*

[展开说明]

**[Project B]**：...

## 反模式

- **[错误做法 1]**：...
- **[错误做法 2]**：...

## 思考公式

> [一句可内化的判断句]

**[N 问自检 / N 步习惯]**：
1. ...
2. ...

## 延伸

- [关联原则 1](NN-xxx.md)
- [关联原则 2](NN-xxx.md)

## 相关案例

[Project A](../case-studies/project-a.md) · [Project B](../case-studies/project-b.md)
```

---

## 命名约定

- **Case study 文件**：`case-studies/<product-slug>.md`（小写、短横线）
- **Principle 文件**：`principles/NN-kebab-name.md`（两位编号 + 短横线）
- **章节标题**：中文数字（一、二、三、……），保持整篇 playbook 一致

---

## 什么时候不要改

- **心血来潮想加一条原则**：先放在 case study 里，观察 3 个以上项目再决定
- **想改已有原则的措辞**：原则越用越稳定比越改越"好"更重要。确有必要时，改，但保留原始语感
- **想加"最佳实践" / "常见错误"**：这本 playbook 的定位是**判断原则**，不是操作手册。操作性的东西写 blog / writeup 更合适

---

## 给 fork 这本 playbook 的人

随便改、随便删、随便加你自己的产品。**你的 playbook 应该看起来和我的不一样**——因为你做的产品不一样、你的判断也不一样。

把它当作一个模版，不是一本圣经。

---

*Built for one person deciding alone · [@yangyue1974](https://github.com/yangyue1974)*
