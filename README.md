# The Mom Test — 客户访谈技能（含陪练模式）

> 把 Rob Fitzpatrick《The Mom Test》蒸馏成一个可直接安装的 Agent 技能：
> **12 张能力卡**（含原文依据、案例、可执行步骤、边界）＋ 一个**客户访谈陪练模式**。

---

## 它解决什么问题

绝大多数"客户访谈"都在浪费时间——对方出于礼貌对你说谎，而你把谎话当数据，一路做错到钱花完。

这个技能把书里的判定标准变成**可以随时调用、可以反复练习**的能力。

## 包含什么

**① 12 张能力卡**（`references/capabilities/`）

| 卡 | 一句话规则 |
|---|---|
| `mom-test-three-rules` | 三条铁律：谈他们的生活、问过去的细节、少说多听 |
| `bad-data-triage` | 好评挡开、泛泛拉回具体、点子下挖动机 |
| `question-quality-gate` | 把"你觉得/你会不会/愿付多少"改写成"你现在怎么做/上次何时/代价多少" |
| `important-questions` | 每场对话至少问一个能推翻你当前生意的问题 |
| `zoom-control` | 先广后深；把产品/市场/预算等所有失败点摊开 |
| `product-market-risk` | 先分清风险在产品还是在市场 |
| `keeping-casual` | 把访谈降级成随意的聊天，越晚提到你的想法越好 |
| `commitment-advancement` | 用时间/声誉/金钱三大货币索取承诺 |
| `meeting-outcome` | 会议非成即败，唯一标尺是"是否推进到下一步" |
| `segmentation-slicing` | 好细分是"谁 + 在哪找"，反馈矛盾说明切得不够细 |
| `finding-conversations` | 把"你去找人"变成"人来找你"（含 VFWPA 邀约框架） |
| `conversation-process` | 会前 3 个大问题、会中两人分工、会后团队复盘 |

每张卡都是 **RIA++ 结构**：`R 原文（英文原句+中译+章节）→ I 方法论骨架 → A1 应用示例 → A2 触发场景 → E 可执行步骤 → B 边界`。

**② 陪练模式**（`references/trainer-mode.md`）

大模型扮演一个**具体客户**与你对话 4–6 轮，结束后摘下面具，按 12 张能力卡逐句打分、**引原著原文**、给你改写，并判定这场会议是成是败。

---

## 安装

把本仓库的内容放到你的 Agent 技能目录下，命名为 `mom-test`。

### WorkBuddy

```bash
# macOS / Linux
git clone https://github.com/Atange2023/mom-test-skill.git ~/.workbuddy/skills/mom-test
```

```powershell
# Windows (PowerShell)
git clone https://github.com/Atange2023/mom-test-skill.git "$env:USERPROFILE\.workbuddy\skills\mom-test"
```

不想用 git？点仓库右上角 **Code → Download ZIP**，解压后把整个文件夹重命名为 `mom-test`，放到：

- macOS / Linux：`~/.workbuddy/skills/`
- Windows：`C:\Users\<你的用户名>\.workbuddy\skills\`

最终目录长这样：

```
.workbuddy/skills/mom-test/
├── SKILL.md
└── references/
```

### 其他 Agent

任何支持 `SKILL.md` 规范的 Agent（CodeBuddy 等）同理——放进它的 skills 目录、文件夹名为 `mom-test` 即可。本技能**纯 Markdown，无脚本、无网络请求、无外部依赖**。

---

## 怎么用

### 用法一：直接提问（能力卡）

说这些话就会自动触发：

- 「我要去见一批客户，帮我设计不诱导的访谈问题」
- 「我做了一轮访谈，客户都说不错，我能信吗」
- 「客户说很有兴趣但一直不买，怎么办」
- 「我不知道该先切哪个细分市场」
- 「帮我看看这份访谈提纲，哪些问题会带偏对方」

### 用法二：陪练模式

说 **「妈妈测试陪练」** 或 **「模拟客户」**，然后给出 3 个输入：

1. **你是谁**（你的身份 / 角色）
2. **你想卖什么**（产品、服务，或任何想验证的东西）
3. **客户开局是什么态度**（① 非常不感兴趣　② 比较冷漠　③ 中性　④ 感兴趣　⑤ 非常感兴趣）

**起点态度决定了你会犯哪类错**：

| 起点 | 我开局什么样 | 你最容易犯的错 |
|---|---|---|
| ① 非常不感兴趣 | 冷淡、想结束 | **推销**：为证明自己有价值而猛讲产品 |
| ② 比较冷漠 | 礼貌但平，"嗯""还行" | **推销 / 过早放弃** |
| ③ 中性 | 就事论事，一问一答 | **坏数据**：把普通回答当信号，不挖细节 |
| ④ 感兴趣 | 主动发问、顺手给好评 | **坏数据**：被好评带走，忘了追事实 |
| ⑤ 非常感兴趣 | 热情、"我现在就想报" | **草率成交**：直接报价/承诺，跳过学习 |

> 书里说：*"There's more reliable information in a 'meh' than a 'Wow!'"* —— 一个"嗯"比一个"哇"更有信息量。**起点越高，你越容易短路。**

陪练结束后你会拿到：逐句点评 + **14 分制评分表** + 每处失分对应的原著原文 + 改写话术 + 会议成败判定 + 起始态度复盘。

> ⚠️ **边界**：陪练是**飞行模拟器**，不是市场调研。模拟客户是编的，**不能**用来判断你的生意好不好——只用来练你的**提问手艺**。

---

## 文件结构

```
mom-test-skill/
├── SKILL.md                          # 技能主入口：触发条件、能力路由表、核心原则
├── references/
│   ├── capabilities/                 # 12 张 RIA++ 能力卡
│   ├── capability-index.md           # 完整意图与关键词索引
│   ├── cheatsheet.md                 # 决策规则速查（一句话版）
│   ├── glossary.md                   # 术语表
│   ├── overview.md                   # 全书概览
│   └── trainer-mode.md               # 陪练模式（演练流程 + 评分表 + 助教职责）
└── BUILD_MANIFEST.json               # 构建元数据
```

---

## 来源与许可

本书方法论来自 **Rob Fitzpatrick, _The Mom Test_ (2013)**。本技能是**方法论的再组织与教学化改写**，为标注出处保留了少量英文原句与章节号，并非原书内容的复制。强烈建议读原书——它很短，两小时能读完。

详见 [`NOTICE.md`](NOTICE.md)。

---

## 改进它

发现某张卡不准确、或陪练体验有问题，欢迎提 Issue / PR。

主要可改进方向：
- 陪练的客户角色库（更多行业 / 更多细分）
- 能力卡的中文案例（补本土场景）
- 评分表权重的校准
