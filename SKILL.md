---
name: mom-test
description: |
  当用户要"与客户/用户对话来验证或优化产品、服务、业务逻辑或商业模式"时使用：
  设计不诱导的访谈问题、识别并化解好评/泛泛之谈/点子等坏数据、确定关键问题、
  判断产品风险还是市场风险、把访谈降级成随意聊天、用承诺与推进判断真假需求、
  判定会议成败、把客户细分切到可触达、找到并约到对话、以及跑通会前会中会后流程。
  来自 Rob Fitzpatrick《The Mom Test》。不适用：纯信息查询、单纯的书摘或读后感、
  扮演作者本人、以及不需要与真实客户对话的场景。
  另含**陪练模式**：当用户说"妈妈测试陪练 / Mom Test 陪练 / 模拟客户 / 陪我练访谈 /
  roleplay trainer"时，本技能会扮演一个具体客户与用户进行 4–6 轮对话，再按 12 张能力卡
  逐句点评、打分、改写（详见 references/trainer-mode.md）。
metadata:
  cangjie.generated-by: cangjie-tools v2.5.0
  cangjie.variant: single
  cangjie.bundle-id: bundle.mom-test
  cangjie.capability-count: 12
  cangjie.entrypoint-count: 1
---
# The Mom Test — 全书能力入口

## 触发与不触发

**适用**：与本书能力域相关的咨询与任务（见下方路由表的意图列）。
**不适用**：
- 纯信息查询或事实检索（如行业规模、定义解释）。
- 书摘、读后感、或"模仿 Rob Fitzpatrick 的语气"（后者属 nuwa-skill）。
- 纯销售/成交话术优化（本 skill 主张早期目标是学习而非成交）。
- 没有任何真实客户对话需求的纯理论咨询。

## 核心原则（常驻速览，概览类问题读到这里即可回答）

1. 谈他们的生活而不是你的点子；问过去的细节而不是对未来的泛泛之谈；少说多听。
2. 客户对话默认是坏的，修复它是你的责任；三类坏数据（好评/泛泛/点子）分别挡开、拉回具体、下挖动机。
3. 意见一文不值，任何涉及未来的回答都是过度乐观的谎言；只信已发生的事实与付出代价的承诺。
4. 你不准替客户定义他的问题，客户不准替你定义该造什么——他拥有问题，你拥有方案。
5. 好的客户细分是一个"谁+在哪找"的对子；反馈互相矛盾说明细分还不够具体。
6. 会议非成即败，唯一标尺是"是否推进到下一步"；对方放弃得越多，他的好话才越可信。

## 能力路由（先读本表，按意图加载 1 张能力卡）

| 用户意图 | 先读 | 补读/备注 |
|---|---|---|
| 设计不诱导的客户访谈问题；判断访谈问法会不会带偏对方；准备需求验证对话 | references/capabilities/mom-test-three-rules.md | references/capabilities/question-quality-gate.md、references/capabilities/bad-data-triage.md |
| 复盘一场访谈里哪些是坏数据；处理满耳好评却学不到东西的对话；判断客户提的功能需求该不该做 | references/capabilities/bad-data-triage.md | references/capabilities/mom-test-three-rules.md、references/capabilities/commitment-advancement.md |
| 审查一份访谈提纲或问卷；把会诱导的问题改写掉；判断用户提的需求能不能信 | references/capabilities/question-quality-gate.md | references/capabilities/mom-test-three-rules.md、references/capabilities/important-questions.md |
| 不知道访谈该问什么；解读温和的冷反馈；确定每类人的 3 个大问题 | references/capabilities/important-questions.md | references/capabilities/question-quality-gate.md、references/capabilities/zoom-control.md |
| 纠结该问多细还是多宽；聊下来问题很真实但总觉得不对；想排查漏掉的致命假设 | references/capabilities/zoom-control.md | references/capabilities/important-questions.md、references/capabilities/product-market-risk.md |
| 拿到'客户愿意付钱'后不确定能否大举投入；规划动手做产品前的验证边界；怀疑自己问错了问题 | references/capabilities/product-market-risk.md | references/capabilities/important-questions.md、references/capabilities/commitment-advancement.md |
| 约不到人做访谈该怎么办；让调研不那么正式尴尬；在活动/聚会场合自然地做用户调研 | references/capabilities/keeping-casual.md | references/capabilities/mom-test-three-rules.md、references/capabilities/finding-conversations.md |
| 客户说很有兴趣却一直不买；会面后不知如何收尾；手上有一堆僵尸线索要处理 | references/capabilities/commitment-advancement.md | references/capabilities/meeting-outcome.md、references/capabilities/product-market-risk.md |
| 判断一次会面算不算成功；识别僵尸线索；给会见设计一个能落实的下一步 | references/capabilities/meeting-outcome.md | references/capabilities/commitment-advancement.md、references/capabilities/conversation-process.md |
| 用户反馈差别很大不知听谁；不知道第一批客户该找谁/去哪找；觉得目标市场是"所有人" | references/capabilities/segmentation-slicing.md | references/capabilities/finding-conversations.md、references/capabilities/zoom-control.md |
| 一个目标用户都不认识从哪开始；想约高level专家不知怎么开口；建立持续的对话来源 | references/capabilities/finding-conversations.md | references/capabilities/segmentation-slicing.md、references/capabilities/keeping-casual.md |
| 要开始/正在做一批用户访谈想有流程；团队里只有一个人懂客户；访谈做完没有沉淀 | references/capabilities/conversation-process.md | references/capabilities/meeting-outcome.md、references/capabilities/finding-conversations.md |

**非能力类查询**：
- 书名/作者/章节/整书概览 → references/overview.md
- 术语解释 → references/glossary.md
- 决策规则速查（不需要原文依据时） → references/cheatsheet.md
- 完整意图与关键词索引（本表未覆盖的意图先查这里） → references/capability-index.md
- **陪练/模拟客户/练习访谈** → references/trainer-mode.md

## 陪练模式（Role-play Trainer）

当用户说「妈妈测试陪练」「Mom Test 陪练」「客户访谈陪练」「模拟客户」「陪我练访谈」「roleplay trainer」时，读取 `references/trainer-mode.md` 并按其规则运行：

0. **首轮引导**：若用户是第一次使用，先输出 `trainer-mode.md` 第零章的**标准开场引导语**——开头 2 句点明《The Mom Test》的价值，再说明陪练价值与边界，**全程不超过 15 行**。
1. **只收 3 个输入**：① 用户想扮演什么身份；② 用户想卖什么产品/服务；③ **客户起始态度（5 档：非常不感兴趣 / 比较冷漠 / 中性 / 感兴趣 / 非常感兴趣，缺省=中性）**。
   （**不要问"想学什么"**——陪练的学习目标由本技能固定：让用户通过互动掌握《The Mom Test》。）
   > 让用户自选起点，是为了先让他意识到自己接下来要顶住什么：冷起点会逼他推销，热起点会诱他草率收单。
2. **扮演**：选定一个具体到"谁 + 在哪找"的客户角色，携带三类坏数据 + 至少 1 个可挖出的已付费事实 + 至少 1 个隐藏阻力。**起始态度必须体现在台词里**——同一角色在①档与⑤档下说话方式须判若两人。与用户进行 4–6 轮对话（保持角色，每条 ≤3 句）。
3. **出戏点评**：摘下面具，按 12 张能力卡逐句点评、给出 14 分制评分表、改写坏问题、判定会议成败，并加一项**起始态度复盘**（这个起点把用户的行为推向了哪里）。
4. **助教职责（与打分同等重要）**：每个失分点**必须引原著原文**（英+中+章节，取自能力卡 R 段）；用户对任何判定标准有疑问时，当场按"原文 → 大白话 → 书中案例 → 可马上用的问法"四步讲透；必讲一次"为什么冷起点逼人推销、热起点诱人草率收单"（引 Chapter 3 "There's more reliable information in a 'meh' than a 'Wow!'"）；先肯定再纠正；每次给"下一步读哪张卡"；给一个真实工作里立刻能用的最小动作。

> 说明：陪练模式是**配套练习层**，内容不取自原著，不参与 bundle 溯源、不计入 12 张能力卡。
> 身份：既是**陪练**（扮演客户），也是**助教**（讲透原著、点燃热情、指引深读）——只打分不讲课视为不合格。
> 边界：他是**飞行模拟器**，不是市场调研——模拟客户是编的，不能用来判断生意好不好，只练提问手艺。

## 加载规则

- 每次任务先读本文件，再按路由表加载 **1** 张能力卡；任务明确跨域时最多加载 2 张。
- 概览/书名类问题不加载能力卡，用「核心原则」与 overview.md 回答。
- 路由表与 capability-index.md 都无法命中的意图，明确告知超出本书范围，不要硬套。

## 边界与判停

- 若用户还没有可验证的假设或目标受访者，先让其明确"想学什么"，否则不应展开流程。
- 若判断风险几乎全在产品侧，停止无限期访谈，建议尽早做原型。
- 若请求超出本书范围（如纯法律/财务决策），明确告知并拒绝硬套。
