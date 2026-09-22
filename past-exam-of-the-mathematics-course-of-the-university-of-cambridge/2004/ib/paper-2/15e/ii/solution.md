<h1 id="15e/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [weighted binary-sequence metric](../../../../../../weighted-binary-sequence-metric.md) is finite because $0\leq d(\epsilon,\eta)\leq\sum_{n\geq1}2^{-n}=1$. It is symmetric and nonnegative. If $d(\epsilon,\eta)=0$, every nonnegative summand is zero, so every coordinate agrees; conversely agreement makes the sum zero. For three sequences, apply $|\epsilon_n-\zeta_n|\leq|\epsilon_n-\eta_n|+|\eta_n-\zeta_n|$ in each coordinate and sum. This proves the [triangle inequality](../../../../../../triangle-inequality.md), so **$d$ is a [metric](../../../../../../metric.md)**.

If two sequences differ in one of their first $n$ coordinates, their distance is at least $2^{-n}$. Thus the [open ball](../../../../../../open-ball.md) $B_d(\eta,2^{-n})$ is contained in $C_n(\eta)$. For every $\eta\in C_n(\epsilon)$, the latter cylinder equals $C_n(\eta)$, so each [cylinder set](../../../../../../cylinder-set.md) is open in the [metric topology](../../../../../../metric-topology.md). Every set in the specified topology, being a union of [cylinder sets](../../../../../../cylinder-set.md), is therefore metric-open.

Conversely, agreement in the first $n$ coordinates gives

$$
d(\epsilon,\eta)\leq\sum_{k>n}2^{-k}=2^{-n}.
$$

Given a metric-open set containing $\epsilon$, choose a ball $B_d(\epsilon,r)$ inside it, then choose $n$ with $2^{-n}<r$. The bound gives $C_n(\epsilon)\subseteq B_d(\epsilon,r)$, establishing the required prefix-neighbourhood condition. **The two topologies coincide.** The strict inequality $2^{-n}<r$ avoids incorrectly treating the closed tail bound as a strict ball bound.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [15E](../../15e.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
