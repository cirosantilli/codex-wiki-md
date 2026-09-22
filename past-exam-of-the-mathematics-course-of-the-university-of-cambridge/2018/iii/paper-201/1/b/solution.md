<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [martingale convergence theorem](../../../../../../martingale-convergence-theorem.md) says that if a discrete-time [martingale](../../../../../../martingale-split.md) $(M_n)$ satisfies $C=\sup_n\mathbb E|M_n|<\infty$, then there is an [integrable random variable](../../../../../../integrable-random-variable.md) $M_\infty$ such that

$$
\boxed{M_n\longrightarrow M_\infty\quad\text{almost surely},\qquad \mathbb E|M_\infty|\leq C.}
$$

The hypothesis does not by itself ensure [convergence in L1](../../../../../../convergence-in-l1.md).

For each pair of [rational numbers](../../../../../../rational-number.md) $a<b$, the [Doob upcrossing inequality](../../../../../../doob-upcrossing-inequality.md) gives $\mathbb E U_N[a,b]\leq(C+|a|)/(b-a)$. The [monotone convergence theorem](../../../../../../monotone-convergence-theorem.md) therefore gives a finite [expected value](../../../../../../expected-value.md) for $U_\infty[a,b]=\lim_NU_N[a,b]$, so this [upcrossing count](../../../../../../upcrossing-count.md) is finite [almost surely](../../../../../../almost-sure-convergence.md). There are only countably many such pairs, hence all their [upcrossing counts](../../../../../../upcrossing-count.md) are simultaneously finite outside one event of probability zero.

If $\liminf_nM_n<\limsup_nM_n$, the [density of the rational numbers](../../../../../../density-of-the-rational-numbers.md) supplies $a<b$ strictly between them, forcing infinitely many [upcrossings](../../../../../../upcrossing.md). Consequently $M_n$ has a limit in the [extended real numbers](../../../../../../extended-real-number-line.md) [almost surely](../../../../../../almost-sure-convergence.md). By the [Fatou lemma](../../../../../../fatou-s-lemma.md),

$$
\mathbb E\left[\liminf_n|M_n|\right]\leq\liminf_n\mathbb E|M_n|\leq C.
$$

A limit of either $+\infty$ or $-\infty$ would make this lower limit infinite, so the limit is finite [almost surely](../../../../../../almost-sure-convergence.md), and the same inequality proves its [integrability](../../../../../../integrable-random-variable.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
