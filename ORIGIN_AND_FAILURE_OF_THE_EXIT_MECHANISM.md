# 退出机制是怎样产生的，以及我为什么最终放弃它

> **Status:** retrospective research note, not a new model version.
>
> 这份文件记录一个我曾经真诚相信的新经济机制如何产生、为什么它一度令我非常兴奋、它最终为什么在理论上失败，以及这个错误为什么反而产生了后来真正存活下来的研究问题。
>
> 关于 v1.0–v9.0 的完整版本历史，见 [`RESEARCH_HISTORY.md`](./RESEARCH_HISTORY.md)。关于每一版具体增加了什么、后来受到什么批评、下一版又解决了什么，见 [`WHY_THE_PROJECT_CHANGED.md`](./WHY_THE_PROJECT_CHANGED.md)。本文只在必要处简单定位这些版本，不重复逐版叙述。

---

## 1. 为什么我会开始研究这个问题

我开始这个项目时刚刚系统接触微观经济学不久。

当时的动机并不只是完成一篇课程论文。我有一个很强、现在回头看甚至有些过度的愿望：

> **我希望找到一个经济学里尚未被发现、但一旦被发现就真正重要的问题，并成为一个重要的经济学家。**

成瘾问题吸引我的原因很直接。标准理性成瘾理论强调，过去消费形成的 addictive stock 可以改变今天和未来的消费激励。但我不断想到另一个方向：

> 如果强化可以成为理性选择的一部分，那么减少、戒除和恢复为什么只能来自外部承诺、冲击或者非理性？一个完全理性的行为人，能不能主动“投资于退出”？

这就是最初的 **exit mechanism**。

在 [`v1.0`](./v1.0/) 中，我甚至把它明确称为一种 endogenous **hedging commodity**：行为人像持有一种对冲资产一样，通过退出机制抵消 addictive stock 所产生的强化作用。原始 README 以及当时的 priority claim 均继续保留在 [`v1.0/README.md`](./v1.0/README.md) 中，因为它们准确记录了我当时真正相信的东西，而不是今天希望当年的自己相信什么。

今天我已经不再认可这种经济解释。

---

## 2. 一个错误的 Marshallian–Hicksian 类比

这个想法和我刚学习消费者理论有直接关系。

当时我刚接触 Marshallian demand 与 Hicksian demand，对它们的理解还很粗糙。我模糊地产生了这样一个类比：

- 成瘾消费像一种直接选择；
- 戒除或退出像一种补偿后的选择；
- 如果 Marshallian object 有某种 Hicksian counterpart，那么成瘾行为是不是也应该存在一个与之对应的“退出对象”？

严格来说，这个类比是错误的。

Marshallian demand

\[
x(p,w)
\]

与 Hicksian demand

\[
h(p,\bar u)
\]

不是两种竞争商品，而是同一偏好在两个不同优化问题下产生的需求对象。因此，从 Marshallian/Hicksian duality 并不能推出一种独立的“退出商品”。

但是，这个错误留下了一样后来真正重要的东西。

我虽然把一种 **trade-off** 错误地理解成了一种 **commodity**，却开始认真思考：

\[
\boxed{
\text{获得一个给定增益时，行为人愿意牺牲多少另一种东西？}
}
\]

后来真正存活下来的不是 exit commodity，而是 **compensation**。

---

## 3. 为什么我曾经把整个世界压成两类商品

另一个最初非常朴素的想法，是把所有选择压成两边：

\[
\text{成瘾品}
\]

与

\[
\text{普通商品和储蓄}.
\]

我当时担心一个很直接的批评：

> 如果消费者还有第三种、第四种、第五种选择怎么办？如果偏好非常复杂怎么办？

我的解决办法不是继续增加变量。恰恰相反，我希望把选择压到最小。

我当时的想法大致是：

> 如果最终只保留两个方向，那么行为人要么选这一边，要么选另一边。这样模型不会因为再增加第三种选择而“逃出去”。

今天看来，把现实中的所有普通消费和储蓄直接聚合成一个商品当然不是由定义保证的，它需要额外的可分性或聚合条件。

但后来我逐渐发现，真正重要的并不是“两商品世界”。真正重要的是一个实验结构：

\[
\boxed{
\text{一个标准化的目标增益}
+
\text{一个单调的补偿方向}
}
\]

也就是说，我并不需要声称现实只有两种商品。我只需要构造一个二元比较，使两个方案之间只留下：

1. 一个我关心的有限增量；
2. 一个可以连续调整的 compensating sacrifice。

于是原来的“两商品假设”开始转化成一个 **binary compensated design**。

---

## 4. 从二分法到精确补偿阈值

最初的二元化只是为了简化模型。后来它逐渐变成：

\[
B_0=(x,m)
\]

与

\[
B_1(p)=(x+\Delta,m-p\Delta).
\]

固定增益 \(\Delta\)，改变补偿价格 \(p\)，直到行为人恰好无差异：

\[
B_0\sim B_1(p_\Delta(x)).
\]

于是一个二元选择不再只是告诉我们：

\[
A\succ B.
\]

它给出了一个有限而精确的 trade-off：

\[
\text{一个标准化增益}
\sim
\text{一个精确补偿损失}.
\]

这件事在最初提出 exit mechanism 时完全不是我的研究目标。我当时只是想让消费者“无处可逃”。但后来真正有力量的地方恰恰变成：

> **把一个复杂偏好问题压成一个可以精确测量的有限比较。**

多个这样的有限比较一旦组合起来，就开始产生新的问题：

\[
\text{它们能不能同时来自同一个偏好结构？}
\]

\[
\text{什么时候只能校准，什么时候具有拒绝力？}
\]

\[
\text{什么时候能够识别相对价值？}
\]

这最终成为后来 compensated-choice 研究的真正来源之一。

---

## 5. v3.0：我第一次试图消灭 functional-form criticism

早期 exit mechanism 使用了比较特殊的函数形式。我很快开始担心：

> 如果别人问“为什么一定是这个函数”，我该怎么办？

因此到了 [`v3.0`](./v3.0/)，我把退出函数推广成一个函数族：

\[
g(c,A)=\int_c^A q(s)\,ds,
\qquad q(s)>0,\quad q'(s)<0,
\]

并尝试通过一组公理描述允许的整个函数类。原始的函数族、state-invariance 命题和 spiral-relapse 叙述仍保留在 [`v3.0/README.md`](./v3.0/README.md) 中。

我想证明的已经不再是：

\[
\exists g_0\quad \text{使模型产生想要的现象},
\]

而是尽可能接近：

\[
\forall g\in\mathcal G,
\quad
\text{主要结论仍然成立}.
\]

这是整个项目第一次明确追求 functional-form robustness。

v3.0 也是当时最令我兴奋的一版。它产生了非常漂亮的 spiral relapse dynamics。我曾经认为，如果一个完全理性的优化模型真的能够内生产生

\[
\text{退出}\rightarrow\text{复发}\rightarrow\text{再次退出}
\]

的螺旋轨迹，那么这个结果可能会非常重要。

后来我才发现，真正致命的问题根本不在这个函数族够不够一般。

---

# 6. 为什么 exit mechanism 最终是错的

考虑一个最简单的版本。假设同一可行集和同一状态转移下，生命周期目标写成

\[
\sum_{t=0}^{\infty}
\beta^t
\left[
u(c_t,A_t)+g(c_t,A_t)-\Phi(c_t,c_{t-1})
\right],
\]

其中 \(g\) 被解释成一个独立的 exit / recovery value。

现在定义 reduced-form utility：

\[
\bar u(c,A)=u(c,A)+g(c,A).
\]

那么对任意可行历史，都有

\[
u(c_t,A_t)+g(c_t,A_t)=\bar u(c_t,A_t).
\]

因此原模型与

\[
\sum_{t=0}^{\infty}
\beta^t
\left[
\bar u(c_t,A_t)-\Phi(c_t,c_{t-1})
\right]
\]

在每一条可行路径上的目标函数完全相同。

于是它们产生同样的：

\[
\text{preference ordering},
\qquad
\text{optimal policy},
\qquad
\text{Bellman / Euler conditions},
\]

\[
\text{steady states},
\qquad
\text{closed-loop dynamics}.
\]

如果用 \(\mathcal O\) 表示由模型产生的可观察行为，那么：

\[
\boxed{
\mathcal O(u,g)=\mathcal O(u+g,0).
}
\]

所以，仅仅从这些行为数据中，没有办法证明 \(g\) 是一种独立存在的 economic mechanism。它可以完全被吸收到原来的 state-dependent utility 中。

这才是最初 exit mechanism 最根本的失败。

> **Scope of this argument.** 这个结论针对的是：所谓 exit value 没有自己的独立可行选择维度，而只是已有变量 \((c,A)\) 的一个附加效用项。若未来模型真的引入一个可独立操纵、可观察或被外生扰动的退出维度，那么需要重新分析；这里否定的是早期模型中那个可以被 reduced form 完全吸收的独立机制解释。

---

## 7. 更严重的是：分解本身不被识别

问题还不只是 \(g\) 可以被一次性吸收。

对于任意合适的函数 \(H(c,A)\)，令

\[
u^H=u+H,
\qquad
g^H=g-H.
\]

那么

\[
u^H+g^H=u+g.
\]

于是存在一整族 observationally equivalent decompositions：

\[
(u,g)\sim(u+H,g-H).
\]

因此问题不是：

> “我能不能选择一个合理 normalization 来定义 recovery？”

而是：

\[
\boxed{
\text{行为数据没有告诉我们总价值应该怎样被拆成这两个部分。}
}
\]

normalization 可以选择一个表示，但它不能创造 mechanism identification。

---

## 8. 为什么 v3.0 的一般函数也救不了它

v3.0 的

\[
g(c,A)=\int_c^A q(s)\,ds
\]

确实解决了一个问题：结果不必依赖某一个线性、指数或者二次函数。

但是如果令 \(Q'=q\)，那么

\[
g(c,A)=Q(A)-Q(c),
\]

仍然可以写进

\[
\bar u(c,A)=u(c,A)+Q(A)-Q(c).
\]

所以 v3.0 解决的是

\[
\text{functional-form robustness},
\]

却没有解决

\[
\text{mechanism identification}.
\]

这是我后来才真正认识到的区别：

\[
\boxed{
\text{一个机制可以对很大的函数类稳健，}
\text{同时仍然完全不可独立识别。}
}
\]

---

## 9. 如果 exit 真的是一种商品，它至少必须是一个独立选择维度

最初我把 exit mechanism 称为 hedging commodity。

但如果它真的像一种独立商品一样进入选择，那么原则上应该存在

\[
(c,A,e_1)
\]

和

\[
(c,A,e_2),
\qquad e_1\neq e_2,
\]

即在相同的 \((c,A)\) 下仍能独立改变 \(e\)。

如果实际上

\[
e=h(c,A),
\]

那么在可行集上

\[
U(c,A,e)=U(c,A,h(c,A))\equiv\widetilde U(c,A).
\]

此时 \(e\) 没有增加新的 feasible dimension，它只是已有变量的重新编码。

因此，我最初真正犯的错误可以很简单地表达：

\[
\boxed{
\text{我把一个 trade-off 当成了一个 commodity。}
}
\]

后来存活下来的版本则是：

\[
\boxed{
\text{不选择不是一种新商品，但放弃可以形成一个可测量的 trade-off。}
}
\]

---

## 10. 漂亮的螺旋为什么也不能证明机制存在

v3.0 中最令我着迷的结果是 spiral relapse。

但是，如果 \((u,g)\) 和 \((u+g,0)\) 在每一条可行历史上的 objective 完全相同，那么两者的 optimal policy 相同。于是 closed-loop transition map \(\Psi\) 相同，局部 Jacobian

\[
D\Psi
\]

相同，所以 eigenvalues、complex roots 和 spiral dynamics 也相同。

因此：

\[
\boxed{
\text{spiral dynamics}\not\Rightarrow\text{independent exit mechanism}.
}
\]

图可以是真的，动态可以是真的，但我对动态附加的机制解释仍然可以是假的。

这是整个项目给我留下的最重要的方法论教训之一。

---

## 11. 其他版本在这条思想链中的位置

这里不再重复逐版本历史。完整内容见 [`RESEARCH_HISTORY.md`](./RESEARCH_HISTORY.md) 与 [`WHY_THE_PROJECT_CHANGED.md`](./WHY_THE_PROJECT_CHANGED.md)。这里只做最短定位：

- **v1–v2**：把 exit intuition 写成动态结构；
- **v3**：从特殊函数推进到一般函数族；
- **v4**：问题开始转向 representation、target dependence 与 double counting；
- **v5**：不再直接从 recovery utility 出发，而转向 path-generated additive measurement；
- **v6**：进一步把 representation 与 exact path-information compression 分开；
- **v7**：把抽象对象重新翻译成可观察的 compensated choice；
- **v8–v9**：问题进一步收缩到 counterfactual identification、nuisance cancellation 与 support。

这些版本不是一条不断证明 exit mechanism 越来越正确的路线。

恰恰相反，它们记录的是：

\[
\boxed{
\text{exit mechanism 一点点消失，而真正的问题一点点显现。}
}
\]

---

## 12. 一个错误理论怎样产生了两个后来可以独立存在的研究方向

回头看，这个失败至少留下了两条与原 exit mechanism 已经可以分离的路线。

第一条来自 v5–v6：

\[
\text{局部 cancellation}
\rightarrow
\text{有限 cancellation}
\rightarrow
\text{非加法封闭域}
\rightarrow
\text{一般加法域与路径结构}.
\]

第二条来自 v7–v9 以及后来的有限补偿研究：

\[
\text{binary choice}
\rightarrow
\text{exact compensation}
\rightarrow
\text{finite thresholds}
\rightarrow
\text{support}
\rightarrow
\text{closure / falsification / identification}.
\]

第一条最终越来越像一个独立的 additive-domain / path-structure 数学问题。

第二条则越来越像一个 finite revealed-measurement 问题。

它们都已经不需要 exit mechanism 为真。

---

## 13. 从“你根本跑不出去”到 sparse compensated comparisons

我现在尤其觉得有意思的一点，是最初那个非常不成熟的二分法最终留下了什么。

当时我的想法只是：

> 我把选择压成两边，你要么选这个，要么选那个。这样模型不会因为还有别的商品而逃出去。

后来这逐渐变成一个完全不同的问题：

> 如果研究者只观察极少量精确的二元补偿比较，一个偏好模型究竟在什么时候第一次失去逃避反驳的能力？

例如三个有限关系：

\[
A\sim2B,
\qquad
B\sim2C,
\qquad
A\sim C.
\]

最初看起来几乎只是一个小学算术谜题。

但如果不能偷用线性“汇率”，真正的问题就变成：

\[
\text{仅凭单调性、可加性和曲率，}
\text{这些有限比较能否共同成立？}
\]

这才逐渐导向后来关于 minimal rejection support、finite curvature、closure 与 bounded identification 的问题。

因此，最初那句“你根本跑不出去”，后来变成了一个更严格的研究问题：

\[
\boxed{
\text{模型究竟在第几个有限观测上第一次无处可逃？}
}
\]

这可能是整个项目中最意外的一次转化。

这条 finite compensated-comparison 路线后来继续发展为独立于本仓库 v1–v9 版本链的研究。当前论文入口见 SSRN: [Closure and Curvature in Sparse Compensated Comparisons](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=7363901)。

---

## 14. 我为什么不删除早期错误版本

v1.0 原始 README 曾经非常明确地声称 Exit Mechanism 是本研究的核心创新，并把它称为一种 endogenous hedging commodity。我甚至留下过 priority claim。

今天最容易做的事情，是把这些表述删掉或者悄悄改成更成熟的语言。

我不准备这样做。

我宁愿同时保留：

1. 当时真正相信的原始版本；
2. 今天对它为什么错误的正式说明。

因为研究档案如果只保存最后正确的结论，就会把真正的发现过程清洗掉。

所以我希望这个仓库能够明确记录：

> **我曾经认为 exit mechanism 是一个独立的新经济机制。**
>
> **今天我认为这个判断是错误的。**

这不是对历史版本的否定性删除，而是保存历史的一部分。

---

## 15. 今天我怎样理解这段研究

如果一定要用一句话概括整个过程：

> **我最初把一种 trade-off 错误地当成了一种 commodity；为了证明这个 commodity 存在，我不断增强模型；最后却发现真正值得研究的东西正是那个 trade-off 本身。**

最初的问题是：

\[
\text{退出机制存在吗？}
\]

后来变成：

\[
\text{这个分解凭什么？}
\]

再后来变成：

\[
\text{什么行为能够支持这种表示？}
\]

然后是：

\[
\text{什么有限观察真正识别了什么？}
\]

最终，我更关心的是：

\[
\boxed{
\text{给定尽可能少的行为信息，}
\text{一个模型究竟能够逃避多少，}
\text{又在什么时候第一次被迫作出可拒绝的承诺？}
}
\]

所以 exit mechanism 不是这个研究计划最终的答案。

它是一个错误的起点。

而正因为它是错的，它迫使整个项目不断往更基础的问题退。

这也是我选择把它完整保留下来的原因。
