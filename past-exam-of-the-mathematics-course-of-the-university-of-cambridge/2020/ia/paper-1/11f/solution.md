<h1 id="11f/solution">Solution</h1>

↑ **Parent:** [11F](../11f.md)

For events $A_1,\ldots,A_n$, the probabilistic [inclusion-exclusion principle](../../../../../inclusion-exclusion-principle.md) is

$$
\boxed{\mathbb P\left(\bigcup_{i=1}^nA_i\right)
=\sum_{\varnothing\ne J\subseteq\{1,\ldots,n\}}
(-1)^{|J|+1}\mathbb P\left(\bigcap_{j\in J}A_j\right)}.
$$

To prove it, fix an outcome lying in exactly $r$ events. Its total coefficient on the right is

$$
\sum_{k=1}^r(-1)^{k+1}\binom rk=1
$$

by the [binomial theorem](../../../../../binomial-theorem.md); outcomes in no event contribute zero. Taking expectations of this pointwise indicator identity proves the formula. Truncating after the pair terms gives the [Bonferroni inequalities](../../../../../bonferroni-inequalities.md)

$$
\mathbb P\left(\bigcup_iA_i\right)
\geq\sum_i\mathbb P(A_i)-\sum_{i<j}\mathbb P(A_i\cap A_j).
$$

For the final bound, let $X=\sum_i\mathbf1_{A_i}$ and $S=\mathbb EX=\sum_i\mathbb P(A_i)$. The intersection assumption gives

$$
\mathbb E[X^2]
=S+2\sum_{i<j}\mathbb P(A_i\cap A_j)
\leq S+n-1.
$$

The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) applied to $X\mathbf1_{X>0}$ yields $S^2\leq\mathbb E[X^2]\mathbb P(X>0)\leq S+n-1$. Therefore

$$
S\leq\frac{1+\sqrt{4n-3}}2\leq2\sqrt n,
$$

so the required universal constant may be taken as $\boxed{c=2}$. This is a [second moment method](../../../../../second-moment-method.md) estimate.

## ↑ Ancestors (10)

1. [11F](../11f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
