<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A bounded operator $T:H\to H$ is a [Fredholm operator](../../../../../../fredholm-operator.md) when its range is closed and both $\ker T$ and $\operatorname{ran}(T)^\perp=\ker T^*$ have finite dimension. Its [Fredholm index](../../../../../../fredholm-index.md) is

$$
\operatorname{ind}T=\dim\ker T-\dim\ker T^*.
$$

For index zero, choose an isomorphism $J:\ker T\to\ker T^*$ and extend it by zero on $(\ker T)^\perp$. The restricted map $T:(\ker T)^\perp\to\operatorname{ran}T$ is a bounded isomorphism, by the [bounded inverse theorem](../../../../../../bounded-inverse-theorem.md). The [finite-rank operator](../../../../../../finite-rank-operator.md) $J$ fills exactly the missing kernel-to-cokernel block. Thus $T+J$ is invertible and $T=(T+J)-J$ is an invertible operator plus a [compact operator](../../../../../../compact-operator-split.md).

Conversely suppose $T=A+K$ with $A$ invertible and $K$ compact. The [Atkinson theorem](../../../../../../atkinson-theorem.md) proved in part (b) makes every $A+tK$, $0\leq t\leq1$, [Fredholm](../../../../../../fredholm-operator.md): its quotient image is always $[A]$. The block argument in part (c) proves [local constancy of the Fredholm index](../../../../../../local-constancy-of-the-fredholm-index.md), so its index is constant along this interval and equals $\operatorname{ind}A=0$. This invokes the actual parametrix and block proofs below, not an unproved perturbation assertion. **The claimed equivalence holds.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
