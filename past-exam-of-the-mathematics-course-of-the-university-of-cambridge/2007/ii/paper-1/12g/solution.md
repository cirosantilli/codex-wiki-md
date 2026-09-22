<h1 id="12g/solution">Solution</h1>

↑ **Parent:** [12G](../12g.md)

Using the diameter normalization, define $\mathcal H^d_\delta(E)=\inf\{\sum_j(\operatorname{diam}U_j)^d:E\subseteq\bigcup_jU_j,\ \operatorname{diam}U_j\le\delta\}$ and the [Hausdorff measure](../../../../../hausdorff-measure.md) $\mathcal H^d(E)=\lim_{\delta\downarrow0}\mathcal H^d_\delta(E)$. The [Hausdorff dimension](../../../../../hausdorff-dimension.md) is $\inf\{d:\mathcal H^d(E)=0\}$, equivalently $\sup\{d:\mathcal H^d(E)=\infty\}$.

The [Cantor set](../../../../../cantor-set.md) is the intersection of the sets left by successively removing open middle thirds from $[0,1]$. At level $k$ it has $2^k$ [Cantor cylinders](../../../../../cantor-cylinder.md) of diameter $3^{-k}$. For $s=\log2/\log3$, their total $s$-cost is $2^k3^{-ks}=1$, so $\mathcal H^s(C)\le1$.

The random series $\xi=\sum_{n\ge1}X_n3^{-n}$ converges absolutely, and its ternary digits are all zero or two. Thus $\xi\in C$ and its law is the [Cantor Bernoulli measure](../../../../../cantor-bernoulli-measure.md). Each level-$k$ cylinder has probability $2^{-k}$. Distinct such intervals have separation at least $3^{-k}$; a set $U$ of smaller diameter meets at most one. If $3^{-(k+1)}\le\operatorname{diam}U<3^{-k}$, then

$$
\mathbb P(\xi\in U)\le2^{-k}=2(3^{-(k+1)})^s\le2(\operatorname{diam}U)^s.
$$

Sets of diameter zero have probability zero, since the measure has no [measure atoms](../../../../../atom-measure-theory.md); diameters at least one give the bound trivially. For arbitrary nonmeasurable sets use outer probability. Any countable cover of $C$ therefore satisfies $1\le\sum_j\mathbb P^*(\xi\in U_j)\le2\sum_j(\operatorname{diam}U_j)^s$. Hence

$$
\boxed{\tfrac12\le\mathcal H^s(C)\le1,\qquad\dim_H C=\frac{\log2}{\log3}.}
$$

The last implication follows by multiplying the $s$-costs by powers of the cover diameter: measures above $s$ vanish and those below $s$ are infinite.

## ↑ Ancestors (10)

1. [12G](../12g.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
