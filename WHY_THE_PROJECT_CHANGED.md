# Why the Project Changed — and Why It Stops Here

## 一份逐版本研究诊断

这不是一个新的理论版本，也不是对 v1.0–v9.0 的事后改写。它回答三个更具体的问题：

1. **每一版究竟增加了什么？**
2. **这一版后来是怎样被批评、攻击或内部审计击中的？**
3. **下一版具体解决了上一版的什么问题，又留下了什么？**

这里的“攻击”不是都指外部审稿。只有 v5.0 和 v7.0 有明确的 JME 编辑 / Associate Editor 意见；其余版本的“攻击”主要是后续版本暴露出来的内部逻辑问题、可识别性问题、可实施性问题和文献新颖性审计。为了不制造不存在的审稿历史，下面会明确区分这两类来源。

---

## 我们到底在研究什么？

回头看，项目真正持续不变的研究对象并不是“成瘾”、某个新的恢复效用函数、路径加法、补偿比较本身，也不是某一种动态系统。更稳定的问题是：

> **当目标环境中缺少直接的局部反事实比较时，现有选择数据到底识别了什么；还缺什么信息；什么额外、可实施的比较支持能够严格缩小目标响应的识别集？**

最初，这个问题被写成“理性个体为什么会退出、复发、再次退出”；后来被写成恢复价值、路径历史、可加测量、补偿选择和递归延续价值。到最后，问题被剥离到最小形式：参考环境有局部补偿比较，目标环境只有基准选择而缺少邻近比较，我们能否识别目标选择对状态变化的局部响应？

因此，这个项目最深的主题其实是**缺失的反事实信息**，以及如何区分“数据真正揭示的对象”与“模型、记号或维护假设替我们填进去的对象”。

---

# v1.0 — Initial rational-relapse sketch

### 这一版增加了什么？

v1.0 从一个很直接的经济直觉出发：标准 rational-addiction 叙事强调过去消费如何提高当前边际效用，但“减少、退出、恢复”通常没有作为一个内生价值对象进入模型。于是这一版加入了一个与退出 / 恢复有关的当前价值项，并配合二次调整摩擦，把存量动态中的振荡路径解释为“理性复发”。

这一版真正增加的是一个**问题意识**：退出和减少是否可以像强化一样进入理性选择，而不是只能靠外部承诺或冲击解释。

### 它后来怎样被攻击？

**攻击类型：内部结构批评。**

问题很快出现：退出项为什么是这个函数？二次调整摩擦为什么是这个形式？振荡究竟来自经济机制，还是来自人为选择的动态参数和复根条件？短模型能说明一个可能性，但不能说明这个可能性是否稳健。

换句话说，v1.0 最容易被攻击的地方是：**机制存在，但结构太薄；现象可能是特定函数形式和调整项制造出来的。**

### v2.0 解决了什么？

v2.0 把短构造扩展成完整结构模型：动态规划、稳态、比较静态和不同动态区域都被系统写出。它解决了 v1.0 “只有一个机制草图、没有完整经济结构”的问题。

### 但它没有解决什么？

它没有回答更根本的问题：**那个退出 / 恢复项本身凭什么这样写？** 完整模型可以让一个假设工作得更完整，却不能自动证明这个假设不是任意的。

---

# v2.0 — First complete structural model

### 这一版增加了什么？

v2.0 把 v1.0 的直觉升级成一个完整的动态结构：状态变量、Bellman / Euler 逻辑、稳态条件、比较静态和三类动态区域被放进同一个模型。这样可以更认真地问：复发、退出和长期路径是不是模型内部一致的结果，而不只是一个局部线性化现象。

### 它后来怎样被攻击？

**攻击类型：内部稳健性批评。**

模型越完整，反而越容易看见一个问题：大量结论仍然依赖那个特定的“恢复 / 退出函数”。如果换函数，结论会不会消失？如果答案是会，那么我们研究的可能不是一个经济机制，而只是一个参数化案例。

因此 v2.0 的薄弱点不再是“不完整”，而是：**完整性建立在一个可能过于特殊的 primitive 上。**

### v3.0 解决了什么？

v3.0 用函数族和积分形式推广恢复项，并重新整理 Bellman / Euler 条件。它解决了“结论是否只是某一个具体函数的产物”这个问题，至少把研究对象从单一函数推进到一类函数。

### 但它没有解决什么？

函数族再广，仍然默认了一个更深的分解：总价值可以被拆成原有价值加上“恢复价值”。这就引出了下一轮攻击：**这个加法分解从哪里来？会不会重复计算？**

---

# v3.0 — Function-family / adjustment-friction formulation

### 这一版增加了什么？

v3.0 的主要推进是把具体恢复函数推广为一个函数族，并更系统地处理调整摩擦和动态条件。它试图证明：复发 / 恢复机制并不依赖某一个精心挑选的函数。

### 它后来怎样被攻击？

**攻击类型：内部表示与 double-counting 批评。**

这一版暴露出一个比函数形式更深的问题：即使恢复函数属于一个很大的函数族，为什么总效用应该写成“已有成瘾价值 + 一个额外恢复价值”？如果恢复价值其实已经包含在状态依赖效用里，再加一次就可能 double count。

因此，v3.0 的问题变成了：**我们不是需要更一般的函数，而是需要解释为什么这种分解本身成立。**

### v4.0 解决了什么？

v4.0 转向偏好与表示，从 target stock、恢复相对于目标的位置、加法结构和内生目标形成重新组织模型。它不再满足于“给定一个恢复函数”，而试图说明恢复项如何作为一个可表示对象进入结构。

同时，v4.0 加入 reinforcement–substitution reversal、multiple steady-state boundaries、Personal Equilibrium 式目标形成和 Neimark–Sacker 型循环等结果，使早期“复发”直觉得到更完整的结构表达。

### 但它没有解决什么？

表示理论如果仍然从强结构开始，就可能把希望得到的结论先写进 axioms。更重要的是，即使恢复项能被表示，**这些对象怎样从观察到的选择中被识别？** 这个问题还没有真正出现到台前。

---

# v4.0 — Axiomatic endogenous-recovery structural model

### 这一版增加了什么？

v4.0 是项目第一次真正把“恢复价值是什么”当作一个表示问题处理。恢复被写成相对于 target stock 的方向性价值，并与强化结构放在同一个模型中。它还把 endogenous target formation、稳态边界和周期性动态联系起来。

所以 v4.0 的增加，不只是更多动态结果，而是一次方法论变化：**从“假设一个恢复项”变成“尝试解释恢复项为什么可以这样表示”。**

### 它后来怎样被攻击？

**攻击类型：内部 primitive / representation 批评。**

问题是：即使形式更公理化，恢复函数依然是一个很强的结构对象。加法可分解、目标相对表示、连续性等条件可能已经包含大量结论。于是问题变成：能不能把 primitive 再往下推，不直接从一个全局恢复函数开始？

此外，动态结果越来越丰富，但与可观察行为之间的距离也越来越大。一个模型可以产生 folds、cycles 和 target formation，不等于这些结构已经被行为数据识别。

### v5.0 解决了什么？

v5.0 把 primitive 从“恢复效用函数”改成 target-relative paths 和 path-generated ledgers。它研究的是：在一个并不对任意加法封闭的行为域上，什么 cancellation 条件足以支持 additive measurement，以及怎样得到 Stieltjes 型表示。

这是对 v4.0 最直接的回应：**不先假设恢复函数，而先问行为域上的加法测量从哪里来。**

### 但它没有解决什么？

它把问题推进到了 measurement theory，但代价是主结果越来越依赖抽象表示假设。这个弱点随后被第一次 JME 投稿明确击中。

---

# v5.0 — Additive Measurement on Path-Generated Domains

**原投稿编号：JME-S-26-00480**

### 这一版增加了什么？

v5.0 把研究对象改造成 path-generated domain：primitive 是 target-relative continuous paths、可访问 ledger 和它们之间的行为比较，而不是一个预先给定的 recovery utility function。

这一版的技术核心包括：

- 在非任意可加域上的 cancellation / additive measurement；
- 一个把 common-increment condition 与 finite cancellation 分开的反例；
- 在附加条件下导向 Stieltjes representation 的路线。

这个版本第一次非常明确地把 rational addiction 降为应用，把真正的数学问题改成“有限生成路径域上的加法测量”。

### 它怎样被外部攻击？

**攻击类型：第一次明确的外部编辑 / AE 批评。**

JME 的 desk rejection 并没有说这篇文章没有技术内容。相反，意见明确承认 path-generated ledger construction 很认真，而且把 proposed common-increment condition 与 finite cancellation 分开的反例“technically interesting”。

真正的攻击点是主 representation theorem：它依赖强的 global extension 与 Archimedean assumptions，而这些假设本身已经在很大程度上提供了结论所需要的 ordered-group structure。于是主定理看起来更像是“在已经接近目标结构的假设下恢复目标结构”，而不是从较弱行为条件中真正识别出来。

所以第一次拒稿击中的核心可以概括成：

> **assumptions versus identification：到底是数据 / 行为条件推出了结构，还是维护假设已经把结构放进去了？**

### v6.0 解决了什么？

v6.0 不再把一个宏大的 additive representation 当作唯一终点，而先拆出一个更弱、更精确的问题：一条恢复历史在什么意义下可以被 exact passage compression？

它引入 universal passage carrier、path fibers，并把“历史信息的精确压缩”与“压缩后偏好是否再具有可加表示”分开。这样就回应了 v5.0 的核心问题：**不要让表示假设吞掉真正的信息问题。**

### 但它没有解决什么？

v6.0 仍然非常抽象。即使 passage compression 在数学上更干净，研究者仍然要回答：这些 path fibers、passage ledgers 和 additive objects 在经济数据里究竟如何观察？

---

# v6.0 — Recovery Histories: Exact Passage Compression and Additive Choice

### 这一版增加了什么？

v6.0 把 v5.0 中缠在一起的两个问题拆开：

1. 什么历史信息可以被**精确压缩**；
2. 压缩后的对象在什么额外条件下支持 additive choice / Stieltjes representation。

这一版形成了 universal passage carrier、exact path fibers、BPCC / PVBC / PROC 一类条件，并把 passage compression 本身变成一个独立命题，而不是 representation theorem 的附属步骤。

### 它后来怎样被攻击？

**攻击类型：内部可观察性与经济解释批评。**

v6.0 的逻辑比 v5.0 干净，但一个经济学问题越来越突出：这些历史对象怎样进入实际 choice data？如果研究者必须先拥有很丰富的 path-level object，理论才开始，那么“识别”可能只是发生在一个已经高度结构化的资料空间里。

换句话说：**我们解释了历史怎样压缩，却还没有解释经济学家怎样观察这些历史价值。**

### v7.0 解决了什么？

v7.0 主动退回标准 revealed preference / compensated choice。研究者不再直接观察一个抽象 recovery ledger，而是改变货币补偿直到选择切换，用 exact monetary switching thresholds 作为原始可观察量。

它试图用两个 compensated-choice experiments，把 reinforcement 与 recovery value 放在共同 money-metric geometry 下，从而解决 v6.0 “行为测量入口不清楚”的问题。

### 但它没有解决什么？

为了把旧结构搬进补偿选择语言，v7.0 又创造了大量自己的术语；而第二个实验需要直接给出已经稳定的状态 / continuation 条件，经济实施开始显得人为。这两个弱点随后被第二次 JME 投稿同时击中。

---

# v7.0 — Revealed Reinforcement and Recovery Value

**原投稿编号：JME-D-26-00519**

### 这一版增加了什么？

v7.0 的关键增加是把项目真正放回 choice data：

- 用 exact monetary switching thresholds 得到共同货币单位下的边值 / 差值；
- 用 compensated choice 描述 state-dependent valuation；
- 用两个实验寻找 reinforcement 与 recovery comparison 是否共享一个 common value geometry。

这解决了 v6.0 最明显的缺陷：理论终于有了一个“研究者到底观察什么”的答案。

### 它怎样被外部攻击？

**攻击类型：第二次明确的外部编辑 / AE 批评。**

这一次 JME 的批评与第一次完全不同。

第一，写作和术语。AE 指出，熟悉的经济与数学结构被大量新术语包裹，导致文章异常难读。例如 smooth case 下的 “revealed state reinforcement” 看起来对应标准 increasing differences。把术语翻译回熟悉语言后，剩余贡献是否足够 substantial 就变得不清楚。

第二，若干工具本身并不新。Exact monetary switching thresholds 已经在共同 numeraire 下给出 cardinal edge values；integrability、path independence 等也属于熟悉的基础工具。

第三，第二实验的经济实施不可信。它要求 contracts 直接交付 already stabilized states，同时固定 transition burdens 和其他属性；尤其在 addiction application 中很难解释。

因此第二次拒稿击中的核心可以概括成：

> **terminology / contribution versus implementation：即使数学正确，标准结构不能靠改名变成贡献；额外信息也必须来自可信的经济支持。**

### v8.0 解决了什么？

v8.0 做了两件直接回应：

1. 尽量去掉 reinforcement / recovery 的专有词汇，把问题写成 compensated choice 与 counterfactual identification；
2. 把两个实验压缩成同一个 monetary protocol 下的 recursive continuation problem，不再依赖一个独立、难解释的“第二把尺子”。

它用 transition matching、same-index propagation 和 recursive marginal restriction 来问：从一个可观察的补偿比较系统，哪些 continuation derivative directions 可以传到 counterfactual environment？

### 但它没有解决什么？

v8.0 虽然去掉了第二实验，却仍然给研究者一个相当强的 fiber-level information set：在一族 action-generated continuation fibers 上已经能直接观察 continuation comparisons。并且 projectivized tangent geometry、rank / kernel、propagation 等数学也可能再次把标准工具包装得过重。

---

# v8.0 — Compensated Choice and Recursive Counterfactual Identification

### 这一版增加了什么？

v8.0 把两实验结构收缩成一个 recursive monetary-comparison protocol。核心问题变成：如果 continuation value 在不同环境中共享，能否通过 transition matching 与 same-index propagation，把参考环境的补偿比较信息传递到一个没有直接局部比较的目标环境？

这一版的技术语言包括 projectivized tangent-bundle transition matching、recursive marginal restriction、same-index propagation 和 sharp response-direction identification。

### 它后来怎样被攻击？

**攻击类型：内部新颖性审计 + 信息集审计。**

继续向标准文献翻译以后，问题再次出现：切空间、rank / kernel、局部传播和比较静态原则本身并不构成新的经济理论。更关键的是，v8.0 的研究者已经在一整族 continuation fibers 上直接获得信息，这比真正想问的“目标环境只看到 baseline current choice”强得多。

于是一个非常重要的自我攻击出现了：

> **如果识别成立，是因为结构真的有内容，还是因为我们给研究者的数据已经太强？**

### v9.0 解决了什么？

v9.0 把信息集再削弱到 current-only：

- 目标环境只观察 baseline current choice；
- 不直接观察所需的邻近 target compensated comparisons；
- current-side values 被当作 nuisance effects；
- 通过 graph circulation / current-balanced comparisons 消去 nuisance current values；
- 只保留对 continuation functionals 真正有用的 contrasts；
- 两个四边比较块分别识别目标响应所需的 `H_xa` 与 `H_xx`，不恢复 continuation levels。

这解决了 v8.0 最重要的问题：**不再预先给研究者强 fiber-level continuation information，而是先问 current-only data 到底够不够。**

### 但它没有解决什么？

v9.0 仍然需要最后一次 claim audit：graph cycle space、rank formulas、kernel conditions、finite differences、implicit-function theorem 都是标准工具。真正还能留下多少 paper-specific 内容，必须重新切分。

---

# v9.0 — Compensated Current Choice and Counterfactual Identification

### 这一版增加了什么？

v9.0 是公开版本序列的终点。它把研究对象压缩到一个非常具体的缺失信息问题：

> 在参考环境有补偿比较、目标环境只有基准选择而缺少邻近比较时，什么 comparison support 足以识别目标局部响应？

这一版把 current-side value 当作 nuisance component，用 current graph circulation 消去它；用 `Q(ker D)` 一类对象描述消去 current nuisance 后还能估计的 continuation contrasts；用两个局部比较块恢复 `H_xa`、`H_xx`，再通过目标一阶条件 / implicit-function comparative static 得到 counterfactual response。

它最大的增加不是更多数学，而是**把目标从“恢复价值是什么”变成“缺失反事实响应需要什么信息”。**

### 它后来怎样被攻击？

**攻击类型：最终内部 prior-art / claim audit。**

最后的审计非常严格：

- compensated comparison 是标准测量思想；
- path independence / potential representation 是标准的；
- cancellation / additive representation 有成熟文献；
- nuisance estimability、row space、kernel、rank 是标准线性模型；
- graph cycle space / circulation 是标准工具；
- rectangle finite difference、centered second difference、Taylor expansion 是标准数值 / 分析工具；
- implicit-function comparative statics 也是标准工具。

因此，若继续把这些写成“新理论”，就会重新犯 v7.0 被指出的错误：**把成熟结构重新命名，制造表面新颖性。**

### 最终基础稿解决了什么？

最终的 `counterfactual_choice_theory_foundation.pdf` 没有成为 v10，而是对 v9.0 做了一次拆解和降噪。

它把最核心的 current-only structural identification 写成观察等价扰动上的锐利 iff：目标响应在所有保持 baseline 的允许扰动下不变，当且仅当相应的 kernel-inclusion 条件成立。在局部 `C^2` 扰动足够丰富时，这又能转成 continuation maps 的局部一阶 / 二阶几何匹配条件。

如果这个 matching 失败，基础稿再问什么额外信息真正有用。它证明 single-valued continuation support 下，任何消去 current nuisance 的对比也会把 continuation contrast 一起消掉；而 recombinable compound support 若可实施，则可以用同一个 monetary protocol 构造 current-balanced、continuation-unbalanced comparisons，识别 `H_xa` 与 `H_xx`。最终的潜在贡献被压缩成 strict identified-set comparison，而不是 cycle space 或 finite difference 本身。

基础稿还进一步区分了信息需求：精确响应通常需要二维 continuation information，但与固定 benchmark 的方向 / 符号比较可能只需要一个线性 functional。

### 为什么没有 v10？

因为到这里，剩下的问题已经不能靠内部再加定理解决。

真正还需要回答的是：

1. **prior art**：current-only structural iff、strict identified-set comparison、information-demand hierarchy 是否已有非常接近的祖先？
2. **economic implementation**：什么真实制度自然允许 same current consequence 对应多个 continuation consequences，并允许通过同一 numeraire 做可信的 compensated elicitation？

如果这两个问题没有新的外部答案，再增加一般 `m` 阶 jet、多环境路径、Bellman 扩展、动态分岔或新名词，都不会解决核心不确定性。

所以最后放弃的不是 counterfactual identification 这个问题，而是**继续把它扩张、改名并包装成一个自成体系的新理论。**

---

# 两次 JME 拒稿在整个版本链中的位置

把九个版本连起来看，两次拒稿分别击中了两个不同的层次。

第一次 v5.0 拒稿的核心是：

> **你得到的结构究竟来自行为信息，还是来自已经很强的表示假设？**

这推动了 v6.0 的 exact compression / representation 分离，并最终一路发展成 v9.0 的 observational equivalence 问题。

第二次 v7.0 拒稿的核心是：

> **把标准结构换一个名字不构成贡献；额外识别信息必须有可信的经济来源。**

这推动了 v8.0 的标准语言化和单一货币协议，也最终导致 v9.0 / 基础稿把 standard tools 全部降为 infrastructure，只保留 information structure 与 implementable support 作为可能的研究对象。

所以两次拒稿并不是同一个问题被否定两次。第一次迫使项目学习**不要让 assumptions 冒充 identification**；第二次迫使项目学习**不要让 terminology 和 standard tools 冒充 contribution，也不要让不可实施的实验冒充 information**。

---

# 一句话看完整个演化

| 版本 | 本版真正增加 | 它被击中的地方 | 下一版的回应 |
|---|---|---|---|
| v1.0 | 内生退出 / 恢复直觉与复发动态 | 函数与摩擦过于特定，结构太薄 | v2：完整动态结构 |
| v2.0 | DP、稳态、比较静态、区域结构 | primitive 仍任意 | v3：函数族推广 |
| v3.0 | 一般函数族与调整结构 | 加法分解 / double counting 无基础 | v4：偏好与表示重建 |
| v4.0 | target-relative recovery representation 与内生目标 | 表示仍可能预装结论，观测入口不清 | v5：path-generated behavioral domain |
| v5.0 | cancellation、反例、Stieltjes 路线 | JME：强 extension / Archimedean 假设几乎提供了结论 | v6：先做 exact passage compression，再谈表示 |
| v6.0 | history compression、path fibers、passage carrier | 对象抽象，如何从 choice data 观察不清楚 | v7：compensated choice / switching thresholds |
| v7.0 | money-metric compensated choice + 两实验 | JME：新术语包装标准结构；第二实验不可信 | v8：标准语言 + 单一 monetary protocol + recursive identification |
| v8.0 | transition matching / propagation 的递归路线 | fiber-level 信息太强；几何与 rank/kernel 仍可能是标准包装 | v9：current-only observational equivalence |
| v9.0 | nuisance elimination + continuation-information identification | 标准工具仍不能算贡献；实施与 prior art 未决 | 最终基础稿：只保留 structural iff、strict information comparison、support question |

---

# 最后到底剩下了什么？

最终基础稿把最稳的内容压缩成一个信息比较问题：

- current-only data 什么时候已经足够；
- 如果不够，怎样构造保持观测但改变目标响应的结构扰动；
- single-valued continuation support 为什么不能带来额外可估计 continuation contrast；
- 什么 recombinable compound support 能在消去 current nuisance 后保留真正需要的 continuation information；
- 精确响应与只判断方向时分别需要多少信息。

这里真正可能有研究含义的，不是 kernel、rank、cycle、finite difference 或 IFT，而是：**这些标准工具在什么经济信息结构下产生严格的 identified-set difference。**

---

# 为什么最后停下来？

项目停在这里，不是因为最后什么都没有成立。相反，是因为已经能够比较清楚地说出：

- 哪些结论真的成立；
- 哪些只是标准工具；
- 哪些可能仍有 paper-specific 内容；
- 哪些问题必须靠外部文献与制度事实决定。

继续写下一个版本，只有在解决两类外部问题时才有意义：一是 prior-art audit 显示 current-only structural identification 与 strict information comparison 确实存在尚未被覆盖的缺口；二是能够给出自然、可信、不是为定理临时制造出来的经济制度，使 recombinable continuation support 真正可实施。

在这两点没有新的证据之前，再增加定理、维度、动态系统或新名词不会增加识别内容，只会增加包装。

所以：

> **被放弃的不是“反事实选择识别”这个问题，而是继续把这条路线包装成一个不断扩张的独立“新理论”的做法。**

从 v1.0 到 v9.0，最重要的进步不是 claim 越来越多，而是 claim 越来越少、越来越准确：

> “一个新的理性复发机制”  
> → “恢复价值的表示问题”  
> → “路径域上的加法测量问题”  
> → “补偿选择下的状态依赖价值问题”  
> → “递归反事实识别问题”  
> → **“缺失比较与额外信息支持下的局部反事实识别问题”。**

这也是为什么仓库保留所有中间版本。它们记录的不是九次对同一个贡献的重复声明，而是一个研究问题在内部批评、两次 desk rejection 和文献审计中不断改变自己的对象，直到不能再靠内部推导决定下一步为止。

---

# 最后的研究纪律

如果未来有人继续这条路线，最值得继承的不是内部术语，而是三句话：

> **先问目标对象是否真的由现有数据识别。**  
> **再问额外信息究竟从哪里来。**  
> **最后才问这件事是不是新的。**

在没有新的 prior-art 结论或新的可实施制度之前，v9.0 是合适的公开终点；最终基础稿是对这条路线的内部理论清算，而不是 v10。