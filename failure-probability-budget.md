# Failure-probability budget

↑ **Parent:** [Boole's inequality](boole-s-inequality.md)

A [failure-probability budget](failure-probability-budget.md) assigns nonnegative numbers $\delta_i$ to a finite or [countable](countable-set.md) family of failure [events](event.md) $F_i$ in a common [probability space](probability-space.md), with verified bounds $\mathbb P(F_i)\leq\delta_i$. The [union bound](boole-s-inequality.md) guarantees that the [probability](probability.md) of any failure is at most $\min\{1,\sum_i\delta_i\}$. By [De Morgan's laws](de-morgan-s-laws.md) and the [complement rule of probability](complement-rule-of-probability.md), the [probability](probability.md) that every requirement succeeds obeys

$$
\mathbb P\left(\bigcap_i F_i^c\right)=1-\mathbb P\left(\bigcup_i F_i\right)\geq\max\left\{0,1-\sum_i\delta_i\right\}.
$$

Thus $\sum_i\delta_i\leq\delta$ guarantees simultaneous success with [probability](probability.md) at least $1-\delta$, even when all failure [events](event.md) depend on the same observations. The numbers $\delta_i$ are upper allowances; adding them is not a calculation of the exact failure [probability](probability.md).

For three requirements, give each a [failure-probability budget](failure-probability-budget.md) $\delta_i=1/20$. The total budget is $3/20$, so simultaneous success has [probability](probability.md) at least $17/20$. On a [sample space](sample-space.md) of twenty equally likely outcomes, let $F_1=\{1\}$, $F_2=\{2\}$, and $F_3=\{3\}$. These [disjoint events](disjoint-events.md) attain the budget and the success bound. If instead all three failure [events](event.md) equal $\{1\}$, their individual [probabilities](probability.md) are unchanged, but exact failure has [probability](probability.md) $1/20$ and simultaneous success has [probability](probability.md) $19/20$. This second model shows how overlap can leave the guarantee conservative.

<a id="image-a-shared-failure-probability-budget-covers-both-separate-failures-and-one-common-failure"></a>
![](union-bound-failure-budget-sample-space.png)

**[Figure 9](#image-a-shared-failure-probability-budget-covers-both-separate-failures-and-one-common-failure). A shared failure-probability budget covers both separate failures and one common failure**. The two panels each have twenty equally likely numbered outcomes. The blue, orange, and purple marks identify membership in $F_1$, $F_2$, and $F_3$, respectively. Their individual [probabilities](probability.md) are $1/20$ in both panels. The [union](set-union.md) has three outcomes on the left and one on the right, while the [union bound](boole-s-inequality.md) is $3/20$ in both. The [event](event.md) of simultaneous success is the [complement of an event](complement-of-an-event.md) of any failure and contains seventeen or nineteen outcomes. These are illustrative [probability](probability.md) models, not measured failure rates.

For $n$ requirements, an equal allocation $\delta_i=\delta/n$ is convenient; unequal allocations also work when some requirements are harder to satisfy. For infinitely many requirements indexed by $i\geq1$, the allocation $\delta_i=\delta/2^i$ uses total budget $\delta$ by the [geometric series](geometric-series.md). A fixed positive allowance for every requirement instead gives an infinite sum and no positive simultaneous-success guarantee from the [union bound](boole-s-inequality.md). The individual [probability](probability.md) bounds must cover all the failure [events](event.md) being combined: omitting possible failure modes leaves the resulting guarantee about the listed requirements only. The same addition of error allowances underlies the [Bonferroni correction](bonferroni-correction.md) in simultaneous [hypothesis tests](statistical-hypothesis-test.md).

## ↑ Ancestors (7)

1. [Boole's inequality](boole-s-inequality.md)
2. [Probability inequality](probability-inequality-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Failure-probability budget](failure-probability-budget.md)
