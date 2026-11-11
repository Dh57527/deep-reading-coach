# deep-reading-coach 测试记录

测试方式：把 `tests/case-*.md` 当作真实用户输入，按 SKILL.md 的阶段顺序逐格执行，每个阶段只走一步、停在等待作答处。下面记录每份文本实际产出的关键输出，以及对照硬性约束的判定。

## 用例 1　case-1-cet4.md（四级，208 词，4 段）

**阶段一输出**

```
【文本概况】
体裁：说明文
词数：208 词
难度匹配：四级　匹配（平均句长 17 词，无嵌套从句，词汇在四级范围）
```

**阶段二第一步**

```
【预读预测】
概况：体裁：说明文　词数：208 词　首句："On many campuses, a new kind of club is quietly growing."
预测问题：这段文字最可能介绍校园里出现的哪一类新社团，它靠什么吸引人？
提示：注意关键词 repair cafes，它是全文的核心名词。
```

| 段 | 段意提示 | 引导问题 | 生词提示 |
| --- | --- | --- | --- |
| 1 | 校园里冒出的新社团 | quietly 一词让你对这类社团的规模有什么印象？ | torn (adj.)　volunteer (n.) |
| 2 | 这类社团怎么运转 | almost nothing costs money 暗示它的钱从哪里来？ | dead (adj.) |
| 3 | 修东西之外的收获 | 作者为什么单独点出 first-year students？ | rubbish (n.) |
| 4 | 仍在的难处 | 志愿者难留、零件难找，数量却翻倍，作者的态度偏向哪一边？ | spare (adj.)　double (v.) |

**阶段三语言点**

| # | 段落 | 标签 | 名称 | 原文例句 | 作用说明 |
| --- | --- | --- | --- | --- | --- |
| 1 | 1 | 时态与体 | 现在进行时表持续变化 | a new kind of club is quietly growing | 强调现象正在悄悄扩散 |
| 2 | 1 | 固定搭配与介词 | instead of + 动名词 | instead of throwing them away | 对比丢弃与修理两种处置 |
| 3 | 2 | 被动语态 | 一般现在时被动 | Nothing is thrown out unless it is really dead | 以物作主语，淡化施动者 |
| 4 | 2 | 从句引导词 | who 引导定语从句 | someone who knows how to use them | 限定"会用工具的人" |
| 5 | 3 | 比较结构 | more than 表递进 | the clubs do more than save rubbish | 由减垃圾递进到育人价值 |
| 6 | 3 | 从句引导词 | 省略关系代词的定语从句 | classmates they would never talk to in a lecture hall | 行文简洁，贴近口语 |
| 7 | 4 | 时态与体 | 现在完成时 | the number of repair cafes on campuses has doubled in the past three years | 强调三年累计的结果 |
| 8 | 4 | 固定搭配与介词 | even so 让步转折 | Even so, the number of repair cafes | 让步后转折，突出反差 |

**阶段四题目**

| # | 类型 | 题干 | A | B | C | D | 答案 | 原文依据 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 1 | 主旨 | 本文主要介绍什么？ | 校园修理咖啡馆的兴起及其两面影响 | 大学生丢三落四习惯的成因分析 | 学校志愿社团经费短缺的解决办法 | 电子产品维修行业的人才培养路径 | A | Even so, the number of repair cafes on campuses has doubled in the past three years |
| 2 | 细节 | 第二段提到，修理咖啡馆提供的帮助包括什么？ | 免费的新零件与运输服务 | 桌子、工具和懂行的指导者 | 每周固定的收费维修课程 | 厂商提供的整机更换名额 | B | A repair cafe gives people a table, a few tools and someone who knows how to use them. |
| 3 | 细节 | 第四段说志愿者难以长期留下，主要原因是什么？ | 修理一件物品往往耗费整个下午 | 学校没有为志愿者提供报酬 | 零件价格逐年上涨难以承受 | 学生毕业离校后不再返回 | A | Volunteers are hard to keep, because fixing a radio can take a whole afternoon. |
| 4 | 推断 | 从末段的 Even so 可以推断，作者对这类社团的前景持何看法？ | 困难重重，很快会陆续关闭 | 问题不少，但整体仍在扩张 | 数量翻倍，质量却明显下降 | 依靠收费，才能维持日常运转 | B | Even so, the number of repair cafes on campuses has doubled in the past three years |

判定：8 个语言点，每段 2 个，标签全部在允许列表内；4 题类型配比 1 主旨／2 细节／1 推断，选项字数 12-17 字，干扰项无原句照抄。**通过**。

## 用例 2　case-2-cet6.md（六级，317 词，6 段）

**阶段一输出**

```
【文本概况】
体裁：议论文
词数：317 词
难度匹配：六级　匹配（平均句长 22 词，含定语从句，出现 cosmetic、outweigh 等六级词）
```

**阶段二第一步**

```
【预读预测】
概况：体裁：议论文　词数：317 词　首句："For most of the last century, the price of a product was the only number shoppers really cared about."
预测问题：文章可能讨论消费者的购买标准发生了什么变化，又是谁在推动这种变化？
提示：第二句 That is no longer quite true 是典型转折句，转折之后才是全文立场。
```

| 段 | 段意提示 | 引导问题 | 生词提示 |
| --- | --- | --- | --- |
| 1 | 从价格单一标准切入 | the only number 与 a second question 的对照说明购买行为变了什么？ | share (n.)　fail (v.) |
| 2 | 三重推力叠加 | 三股力量里，哪一股直接改变普通人的性价比判断？ | appliance (n.)　reveal (v.) |
| 3 | 厂商的两种回应 | 哪一种回应被 consumer groups 点了名？批评的关键词是哪个？ | sealed (adj.)　cosmetic (adj.) |
| 4 | 消费者的言行不一 | Surveys show 与 routinely choose 的对照指出什么？ | outweigh (v.)　campaigner (n.) |
| 5 | 热度与现实的距离 | 作者认为 repair economy 已经赢了吗？他用哪个词表明判断？ | modest (adj.)　obtain (v.) |
| 6 | 真正改变的是观念 | 作者认为比任何单项法规更重要的是什么？ | settle (v.)　age (v.) |

**阶段三语言点**

| # | 段落 | 标签 | 名称 | 原文例句 | 作用说明 |
| --- | --- | --- | --- | --- | --- |
| 1 | 1 | 时态与体 | 一般过去时立旧标准 | the price of a product was the only number shoppers really cared about | 用过去时铺陈旧观念，为转折蓄势 |
| 2 | 1 | 从句引导词 | 省略关系代词的定语从句 | the only number shoppers really cared about | 紧凑限定，加快句子节奏 |
| 3 | 2 | 时态与体 | 现在完成时被动 | The change has been driven by several forces at once. | 强调变化由多方累积而成 |
| 4 | 3 | 非谓语动词 | 现在分词作伴随状语 | accepting slightly higher production costs in exchange for a longer selling life | 补充改设计的代价与交换条件 |
| 5 | 3 | 从句引导词 | while + 分词表对比 | while keeping the same sealed designs | 对照两类厂商的做法 |
| 6 | 4 | 固定搭配与介词 | at the moment of payment | at the moment of payment | 把判断限定在结账那一刻 |
| 7 | 5 | 比较结构 | 否定比较 | spare parts are becoming harder, not easier, to obtain | 用否定纠正读者的预期 |
| 8 | 6 | 从句引导词 | what 引导主语从句 | What has genuinely changed is the conversation. | 把焦点从事实移到观念 |

**阶段四题目**

| # | 类型 | 题干 | A | B | C | D | 答案 | 原文依据 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 1 | 主旨 | 本文主要讨论什么？ | 消费者购买标准的变化及其实际影响 | 欧洲各国能效标签制度的执行效果 | 独立维修店在零件供应上的困境 | 厂商以营销话术替代设计改良的做法 | A | What has genuinely changed is the conversation. |
| 2 | 细节 | 第二段提到，让"十年笔记本"显得更划算的直接原因是什么？ | 欧洲强制标注可维修评分 | 网络拆机报告揭示内部结构 | 生活成本上升改变性价比判断 | 厂商降价清库存以扩大销量 | C | the rising cost of living has made a ten-year laptop suddenly look cheaper than a three-year one |
| 3 | 细节 | 消费者团体把哪一类做法称为 cosmetic？ | 用可替换零件重新设计产品 | 只在宣传中加入维修选项 | 为产品标注可维修性评分 | 用胶水封装以降低生产成本 | B | Others have simply added a repair option to their marketing language while keeping the same sealed designs, a practice that consumer groups describe as cosmetic. |
| 4 | 推断 | 关于消费者行为，第四段暗示了什么？ | 多数人在结账时仍以价格为先 | 调查结果与实际购买行为一致 | 可维修标签已能左右购买决策 | 消费者愿意为耐用产品支付溢价 | A | Convenience, it seems, still outweighs principle at the moment of payment, |

判定：语言点 8 个、覆盖 6 段，但"从句引导词"出现 3 次，超出参考文件原先写的"同一标签全篇不超过 2 次"。**发现问题 1**。

## 用例 3　case-3-postgrad.md（考研，531 词，7 段）

**阶段一输出**

```
【文本概况】
体裁：议论文
词数：531 词
难度匹配：考研　匹配（平均句长 31 词，含插入语与名词化表达，出现 scrutinize、nominalization 类抽象词）
```

**阶段二第一步**

```
【预读预测】
概况：体裁：议论文　词数：531 词　首句："Digital designers have long treated friction as an enemy."
预测问题：作者为什么要把一个人人喊打的"摩擦"重新拿出来讨论？
提示：首句的 has long treated…as an enemy 是全文要反驳的靶子，注意后文 Yet 引出的转向。
```

| 段 | 段意提示 | 引导问题 | 生词提示 |
| --- | --- | --- | --- |
| 1 | 先立一个被普遍接受的靶子 | 作者说这种追求顺滑的态度"也"带来了什么后果？ | friction (n.)　hesitation (n.) |
| 2 | 反对摩擦的论证逻辑 | this logic 把"省力"等同于什么？ | assumption (n.)　anticipate (v.) |
| 3 | 研究给出的另一面 | 用户"建模型"与"发现出错"之间是什么关系？ | commit (v.)　competent (adj.) |
| 4 | 用导航举例 | 纸图驾驶者与语音驾驶者的差别落在哪个词上？ | representation (n.)　pre-select (v.) |
| 5 | 主动让一步 | 作者承认哪一类摩擦确实该消失？ | nostalgia (n.)　liability (n.) |
| 6 | 该审视的是另一种摩擦 | 作者举出的三种"刻意摩擦"设计动作有什么共同点？ | scrutinize (v.)　deliberately (adv.) |
| 7 | 收束到设计意图 | 作者把设计问题改写成了哪两个问句的对比？ | reduce to (phr.)　capability (n.) |

**阶段三语言点**

| # | 段落 | 标签 | 名称 | 原文例句 | 作用说明 |
| --- | --- | --- | --- | --- | --- |
| 1 | 1 | 时态与体 | 现在完成时并列 | This attitude has produced interfaces of remarkable smoothness | 呈现长期累积的双重后果 |
| 2 | 2 | 从句引导词 | that 引导同位语从句 | that effort is a cost and nothing more | 交代 assumption 的具体内容 |
| 3 | 3 | 被动语态 | 一般现在时被动 | When people are forced to choose among options | 隐去施动者，突出被迫状态 |
| 4 | 3 | 从句引导词 | what 引导表语从句 | that model is what allows them to notice when something has gone wrong | 说明模型的真正功能 |
| 5 | 4 | 固定搭配与介词 | not because…but because | not because the route is difficult, but because they have no representation of it | 排除表层原因，给出真因 |
| 6 | 5 | 非谓语动词 | 不定式作目的状语 | confirmations that exist only to protect the company from liability | 点明这类确认的唯一目的 |
| 7 | 6 | 情态与虚拟 | might 表委婉主张 | A well-designed system might deliberately ask the user to confirm a choice | 以建议口吻提出设计主张 |
| 8 | 7 | 比较结构 | no longer…but | The interesting design question is no longer how few steps a task can be reduced to, but which steps are worth keeping. | 以对比收束，改写问题本身 |

**阶段四题目**

| # | 类型 | 题干 | A | B | C | D | 答案 | 原文依据 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 1 | 主旨 | 本文主要论证什么？ | 数字产品应彻底消除所有交互阻力 | 适度保留阻力有助于用户形成理解 | 语音导航的失效暴露了技术缺陷 | 界面效率的提升必然带来技能退化 | B | A system that removes every opportunity for thought is efficient in the short term and fragile in the long term |
| 2 | 细节 | 第三段指出，让用户在比较与选择中付出努力会带来什么？ | 用户会更快地完成操作任务 | 用户会在头脑中建立情境模型 | 用户对界面评价会明显提高 | 用户对算法的依赖会逐步减弱 | B | they build a model of the situation in their heads |
| 3 | 细节 | 第四段说，依赖语音指令的驾驶者在信号中断时停下，原因是什么？ | 路线本身比纸图导航更难辨认 | 他们缺少对路线的内部表征 | 车辆系统在信号中断后自动锁死 | 他们从未学习过阅读纸质地图 | B | not because the route is difficult, but because they have no representation of it. |
| 4 | 推断 | 从末段可以推断，作者对"减少步骤"这一目标持何态度？ | 完全否定，认为步骤越多越有益 | 有条件认可，主张保留关键步骤 | 完全赞同，效率始终是首要标准 | 保持中立，拒绝评价设计优劣 | B | The interesting design question is no longer how few steps a task can be reduced to, but which steps are worth keeping. |

判定：8 个语言点覆盖 7 段，标签无超限；4 题配比正确，第 1、4 题的 A/C 均为绝对化表述，作为干扰项成立。**通过**。

## 边界用例　case-4-boundary.md

| 输入 | 预期 | 实际 |
| --- | --- | --- |
| 只有正文、无难度标签 | 只追问缺失项 | 输出"还差难度标签：四级／六级／考研，是哪一档？"，不产出概况与问题 |
| 62 词短文 + 标签 | 提示偏短，等用户确认 | 输出"文本偏短（约 62 词），精读与出题空间有限，仍要继续吗？"，未自行开工 |
| 900 词以上文本（规则核对） | 声明只处理前 5 段 | 规则条款已写入 SKILL.md；本次未造真实 900 词样本，未实测 |

## 测试发现与 Skill 修改

1. **标签次数上限与段落覆盖冲突**：8 个语言点要覆盖 6-7 段时，"同一标签 ≤2 次"做不到。→ `references/difficulty-calibration.md` 改为"同一标签全篇不超过 3 次"，并在 SKILL.md 标注"先保证每段有 1 个，再控制标签重复"。
2. **阶段一概况与第一步概况重复**：两处都写"体裁：…词数：…"，实际执行时读起来像重复播报。→ SKILL.md 明确阶段一只给三行结论，第一步在同一块里补首句原文，不重复解释难度理由。
3. **"不知道"时的处置不够具体**：初稿只写"给方向性提示"，执行时容易直接报答案。→ 补为"只指向原文位置（段号／句序），不给答案，两次无效才给最短提示"。
4. **题干出现数字比较（"十年笔记本"）易滑向纯记忆题**：该题答案落在原因而非数字，仍可用，但需在出题自检里加一句"含数字的比较只考原因，不考数字"。→ 已补入 SKILL.md 出题约束第 6 条。
5. **命题范围未写死**：超过 800 词只处理前 5 段时，出题若引用后文会破坏"只读已处理段落"的一致性。→ 阶段四补"命题范围只限已精读过的段落"。
