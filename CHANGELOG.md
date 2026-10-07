# Changelog

本项目遵循 [语义化版本](https://semver.org/lang/zh-CN/)。

## v1.0.0 — 2026-10-08

首个公开版本。

**能力卡（12 张，RIA++ 结构）**

- 01 `mom-test-three-rules` — 三条铁律
- 02 `bad-data-triage` — 坏数据化解
- 03 `question-quality-gate` — 好问题判定与改写
- 04 `important-questions` — 关键问题（能推翻自己生意的问题）
- 05 `zoom-control` — 先广后深
- 06 `product-market-risk` — 产品风险 vs 市场风险
- 07 `keeping-casual` — 保持随意
- 08 `commitment-advancement` — 承诺与推进
- 09 `meeting-outcome` — 会议成败
- 10 `segmentation-slicing` — 客户切片
- 11 `finding-conversations` — 找到对话（含 VFWPA 邀约框架）
- 12 `conversation-process` — 流程与笔记

**陪练模式**

- 大模型扮演具体客户，4–6 轮对话后出戏点评
- **五档起始态度**（非常不感兴趣 → 非常感兴趣），不同起点诱发不同错误类型
- **14 分制评分表**（7 维度 × 2 分）
- 每个失分点强制引用原著英文原句 + 中译 + 章节号
- 助教职责：概念四步讲透、给下一步读卡建议、给真实工作可用的最小动作
- 首轮标准开场引导语

**辅助资料**

- `capability-index.md` 完整意图与关键词索引
- `cheatsheet.md` 决策规则速查
- `glossary.md` 术语表
- `overview.md` 全书概览

**其他**

- 9:16 包豪斯风格宣传海报（`assets/poster.png` + HTML 源码）
- MIT 许可 + `NOTICE.md` 引用范围说明
- 发布前安全自检：0 脚本 / 0 网络请求 / 0 凭据

**构建链**

- 使用 [cangjie-skill](https://github.com/kangarooking/cangjie-skill) v2.5.0 流水线蒸馏：《The Mom Test》全书 → 阶段 0 整书理解 → 阶段 1 五类候选提取 → 阶段 1.5 三重验证 → 阶段 1.6 晋级门 → 阶段 2 RIA++ 构造 → 阶段 3 链接与术语 → 阶段 4 压力测试 → 阶段 5 编译
- 编译产物通过 `validate_skill_pack.py` 校验：**0 errors / 0 warnings**
