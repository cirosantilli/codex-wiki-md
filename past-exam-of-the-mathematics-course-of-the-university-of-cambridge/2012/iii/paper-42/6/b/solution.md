<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

There is a parity qualification in the printed claim. With the usual strict-majority definition, an even electorate need not have a [Condorcet winner](../../../../../../condorcet-winner.md). On the axis $a<b<c$, the two orders $a\succ b\succ c$ and $c\succ b\succ a$ are both [single-peaked preferences](../../../../../../single-peaked-preferences.md), but every pairwise contest is tied. Thus no alternative strictly defeats every other one. We first prove the intended strict-winner result for odd $n$.

Let $n=2k+1$ and order the peaks along the common axis. Their median $w$ has at least $k+1$ peaks at or to each side. For any $y<w$, the $k+1$ voters whose peaks are at or to the right of $w$ prefer $w$ to $y$ by single-peakedness. For any $y>w$, the corresponding $k+1$ voters on the left prefer $w$. Thus **the median peak is the unique [Condorcet winner](../../../../../../condorcet-winner.md)**.

The corresponding [median voter rule](../../../../../../median-voter-rule.md) is [strategyproof](../../../../../../strategyproofness.md). Fix the other $2k$ peaks $q_1\leq\cdots\leq q_{2k}$. As one voter reports a peak $p$, the selected median is

$$
\operatorname{median}(q_1,\ldots,q_{2k},p)=\min\{q_{k+1},\max\{q_k,p\}\},
$$

where minimum and maximum refer to the common axis. All attainable outcomes lie between $q_k$ and $q_{k+1}$. If the true peak lies inside this interval, truthful reporting obtains the voter's top. If it lies left of the interval, truthful reporting obtains its left endpoint, which the voter's single-peaked order prefers to every larger attainable outcome. The case right of the interval is symmetric. No report improves the outcome. For one voter the rule simply selects its peak.

There is also a proof that does not depend on knowing the axis. If a voter truly prefers a proposed new winner $z$ to the current strict [Condorcet winner](../../../../../../condorcet-winner.md) $w$, that voter already opposes $w$ in the contest $w$ versus $z$. The strict majority supporting $w$ in that contest therefore consists of other voters and is unaffected by its report. Thus $z$ cannot become a strict [Condorcet winner](../../../../../../condorcet-winner.md) after a profitable misreport. This proves [strategyproofness](../../../../../../strategyproofness.md) on the domain of profiles for which the selected strict winner exists, including all admissible odd-electorate single-peaked profiles.

For even $n$, a [weak Condorcet winner](../../../../../../weak-condorcet-winner.md) is guaranteed: every alternative between the two middle peaks weakly defeats each other alternative, allowing ties. With a fixed common axis, consistently choosing the lower median or consistently choosing the upper median gives a single-valued [strategyproof](../../../../../../strategyproofness.md) rule, by the same interval-clamping argument for an [order statistic](../../../../../../order-statistic.md). Arbitrary tie selection is not asserted to have this property. The corrected conclusion is therefore **a unique strict winner and its [strategyproof](../../../../../../strategyproofness.md) selection for odd electorates; a weak winner with a specified median rule for even electorates**.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 42](../../../paper-42-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
