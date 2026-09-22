<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Fix a sequence of deterministic partitions with mesh tending to zero and define the completed-increment sums

$$
S_t^{(n)}=\sum_j\bigl(X_{t\wedge t_{j+1}^{(n)}}-X_{t\wedge t_j^{(n)}}\bigr)^2.
$$

For a [continuous semimartingale](../../../../../../continuous-semimartingale.md), these sums converge to $[X]_t$ in [uniform convergence on compacts in probability](../../../../../../uniform-convergence-on-compacts-in-probability.md), the standard path-increment formula for [quadratic variation](../../../../../../quadratic-variation.md). The sums use only the path of $X$, and do not mention a [filtration](../../../../../../filtration-probability-theory.md). If the same process is a [semimartingale](../../../../../../semimartingale.md) for two [filtrations](../../../../../../filtration-probability-theory.md), the same sums have both proposed [quadratic variations](../../../../../../quadratic-variation.md) as limits. Uniqueness of limits in probability, followed by continuity, makes these limits indistinguishable.

For the change of measure, let $R=d\mathbb Q/d\mathbb P$. If $\mathbb P(A_n)\to0$, then

$$
\mathbb Q(A_n)=\mathbb E_{\mathbb P}(R\mathbf1_{A_n})\longrightarrow0:
$$

truncate $R$ at a large constant, use $\mathbb E[R\mathbf1_{\{R>K\}}]\to0$, and then let $\mathbb P(A_n)\to0$. Apply this argument to the event $\sup_{s\le t}|S_s^{(n)}-[X]_s^{\mathbb P}|>\varepsilon$. The same sums converge to the P-version of the bracket in Q-probability, and the Q-semimartingale formula makes them converge to the Q-version. Therefore

$$
\boxed{[X]^{\mathbb Q}=[X]^{\mathbb P}\quad\mathbb Q\text{-indistinguishably}.}
$$

This is [quadratic variation under an absolutely continuous measure change](../../../../../../quadratic-variation-under-an-absolutely-continuous-measure-change.md). With only $\mathbb Q\ll\mathbb P$, the equality is asserted under Q: a Q-version is unconstrained on a Q-null set that might have positive P-probability.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
