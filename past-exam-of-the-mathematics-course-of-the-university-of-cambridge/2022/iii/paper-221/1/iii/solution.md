<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For one unit write $M=(M_1,M_2,M_3)$ and $W=(M,Z_1,Z_3)$. Since the graph makes $S$ independent of $M$, the known distributions determine the conditional assignment law

$$
q(z_2\mid w)
=\frac{
\sum_s p(s)p(z_1,z_2,z_3\mid m,s)
}{
\sum_s\sum_{z_2'}p(s)p(z_1,z_2',z_3\mid m,s)
}.
$$

Under the [sharp causal null hypothesis](../../../../../../causal-null-hypothesis.md) that $A$ has no effect on $Y$, delete $A\to Y$. The [D-separation](../../../../../../d-separation.md) criterion then gives

$$
Z_2\mathrel\perp Y\mid W:
$$

$M_2$ blocks the route through $C$, $Z_3$ blocks the route through $S$, $M_1$ and $M_3$ block the collider-opened detours through $Z_1$ and $Z_3$, and $A$ remains a collider on routes through $U$.

For independent units $i=1,\ldots,n$, choose a [test statistic](../../../../../../test-statistic.md) $T(Z_{2,1:n},Y_{1:n},W_{1:n})$ that measures residual association between $Z_2$ and $Y$. Hold $(Y_i,W_i)$ fixed and independently draw

$$
Z_{2i}^{(b)}\sim q(\mathord\cdot\mid W_i),
\qquad b=1,\ldots,B.
$$

Recompute $T^{(b)}$ after each draw. A valid Monte Carlo [conditional randomization test](../../../../../../conditional-randomization-test.md) uses

$$
p_B=\frac{1+\sum_{b=1}^B\mathbf1_{\{T^{(b)}\geq T^{\rm obs}\}}}{B+1},
$$

with a two-sided statistic or absolute value when appropriate.

Under the null, conditional on $(Y_{1:n},W_{1:n})$, the observed $Z_{2,1:n}$ and its $B$ resamples are exchangeable because they have the same product law $\prod_iq(\mathord\cdot\mid W_i)$. The rank of $T^{\rm obs}$ among the $B+1$ values is therefore uniform after randomized tie breaking and conservative without it. Consequently

$$
\mathbb P_{H_0}(p_B\leq\alpha\mid Y_{1:n},W_{1:n})\leq\alpha.
$$

Taking expectations proves unconditional [Type I error](../../../../../../type-i-and-type-ii-errors.md) control.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 221](../../../paper-221-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
