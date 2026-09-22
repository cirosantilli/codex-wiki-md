<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $I_0$ be the indices of the true [null hypotheses](../../../../../null-hypothesis.md), let $m_0=|I_0|$, and let $V$ count false rejections. The [familywise error rate](../../../../../familywise-error-rate.md) is

$$
\boxed{\operatorname{FWER}=\mathbb P(V\geq1).}
$$

The [Bonferroni correction](../../../../../bonferroni-correction.md) rejects a null exactly when its [p-value](../../../../../p-value.md) is at most $\alpha/m$. The [union bound](../../../../../boole-s-inequality.md) gives

$$
\mathbb P(V\geq1)\leq\sum_{i\in I_0}\mathbb P(P_i\leq\alpha/m)=\frac{m_0\alpha}{m}\leq\alpha.
$$

This controls the [familywise error rate](../../../../../familywise-error-rate.md) for every configuration of true and false nulls, with arbitrary dependence between their [p-values](../../../../../p-value.md). Marginal super-uniformity, $\mathbb P(P_i\leq t)\leq t$, would also suffice.

For the [Holm step-down procedure](../../../../../holm-bonferroni-method.md), inspect the ordered [p-values](../../../../../p-value.md) in ascending order and stop at the first failed comparison. If the first comparison fails, reject none; this is the convention $k=0$ when the defining set is empty. Ties can be ordered by any fixed rule.

If $m_0=0$ there can be no false rejection. Otherwise let $j$ be the rank of the first true null. Since at most $m-m_0$ false nulls precede it, $j\leq m-m_0+1$ and thus $m-j+1\geq m_0$. If any true null is rejected, the step-down rule must have rejected this first true null, which requires

$$
\min_{i\in I_0}P_i=P_{(j)}\leq\frac\alpha{m-j+1}\leq\frac\alpha{m_0}.
$$

Using the [union bound](../../../../../boole-s-inequality.md) on the true-null [p-values](../../../../../p-value.md) proves

$$
\operatorname{FWER}\leq\mathbb P\left(\min_{i\in I_0}P_i\leq\alpha/m_0\right)\leq m_0\frac\alpha{m_0}=\alpha.
$$

This [first true null argument for Holm control](../../../../../first-true-null-argument-for-holm-control.md) also requires no independence. **Holm controls the familywise error rate at level $\alpha$ under arbitrary dependence.**

Now let $R$ count all rejections. The [false discovery rate](../../../../../false-discovery-rate.md) is the expected proportion of rejections that are false, with zero assigned when nothing is rejected:

$$
\boxed{\operatorname{FDR}=\mathbb E\left[\frac{V}{R\vee1}\right].}
$$

It differs from the [familywise error rate](../../../../../familywise-error-rate.md): several false rejections can still represent a small proportion of a large collection of discoveries.

The [BH procedure](../../../../../benjamini-hochberg-procedure.md) is a step-up rule. Set

$$
K=\max\left(\{k\in\{1,\ldots,m\}:P_{(k)}\leq\alpha k/m\}\cup\{0\}\right).
$$

If $K=0$, reject nothing; otherwise reject all hypotheses with $P_i\leq\alpha K/m$. Exactly $K$ hypotheses are rejected: if more than $K$ [p-values](../../../../../p-value.md) were below that threshold, the next ordered value would also satisfy its own larger threshold, contradicting maximality. Thus $R=K$. Unlike the step-down rule, a failed early comparison does not make this procedure stop.

For the proof, assume that each true-null [p-value](../../../../../p-value.md) is uniform on $[0,1]$ and independent of the entire vector of the other [p-values](../../../../../p-value.md). Joint independence of all [p-values](../../../../../p-value.md) is a sufficient condition; the false-null marginal distributions can be arbitrary. Mere uniformity of the true-null marginals without a dependence condition is insufficient for this argument or for general unmodified BH control.

Fix a true null $i$. Replace its [p-value](../../../../../p-value.md) by zero and let $R^{(i)}$ be the number of rejections made by the [Benjamini-Hochberg procedure](../../../../../benjamini-hochberg-procedure.md) on the modified vector. This variable depends only on the other [p-values](../../../../../p-value.md), and $R^{(i)}\geq1$. The [Benjamini-Hochberg leave-one-out identity](../../../../../benjamini-hochberg-leave-one-out-identity.md) is

$$
\{P_i\leq\alpha R/m,\ R=r\}=\{P_i\leq\alpha r/m,\ R^{(i)}=r\},\qquad 1\leq r\leq m.
$$

To prove it, suppose $i$ is rejected with $R=r$. Decreasing its [p-value](../../../../../p-value.md) to zero leaves every ordered value above rank $r$ unchanged, since it was already among the first $r$ values. Those higher ranks still fail their thresholds, while rank $r$ still succeeds; hence $R^{(i)}=r$. Conversely, suppose $R^{(i)}=r$ and $P_i\leq\alpha r/m$. Restoring $P_i$ still leaves at least $r$ values at most $\alpha r/m$, so $R\geq r$. Increasing one [p-value](../../../../../p-value.md) cannot increase the maximal successful rank, so $R\leq R^{(i)}=r$. This gives equality and rejection of $i$.

Independence and uniformity now give

$$
\begin{aligned}
\mathbb E\left[\frac{\mathbf1_{\{i\text{ rejected}\}}}{R\vee1}\right]
&=\sum_{r=1}^m\frac1r\mathbb P(P_i\leq\alpha r/m,\ R^{(i)}=r)\\
&=\sum_{r=1}^m\frac1r\frac{\alpha r}{m}\mathbb P(R^{(i)}=r)=\frac\alpha m.
\end{aligned}
$$

Summing over the $m_0$ true nulls proves the [exact false discovery rate under independent null p-values](../../../../../exact-false-discovery-rate-under-independent-null-p-values.md):

$$
\boxed{\operatorname{FDR}=\frac{m_0\alpha}{m}\leq\alpha.}
$$

If the independent true-null [p-values](../../../../../p-value.md) are only super-uniform, the same calculation gives the inequality instead of equality. The distinction between the two types of error control and the dependence conditions is essential: Bonferroni and Holm have the preceding guarantees without independence, while the BH proof here explicitly uses it.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 31](../../paper-31-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
