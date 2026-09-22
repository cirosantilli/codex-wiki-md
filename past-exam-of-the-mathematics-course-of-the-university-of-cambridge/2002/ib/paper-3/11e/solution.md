<h1 id="11e/solution">Solution</h1>

↑ **Parent:** [11E](../11e.md)

The function $\phi(t)=t/(1+t)$ increases for $t\ge0$, and

$$
\phi(b)+\phi(c)=\frac b{1+b}+\frac c{1+c}
\ge\frac b{1+b+c}+\frac c{1+b+c}=\phi(b+c).
$$

Thus $a\le b+c$ implies $\boxed{\phi(a)\le\phi(b)+\phi(c)}$. Applying this to the triangle inequality for a [metric](../../../../../metric.md) proves the triangle inequality for the [bounded metric transform](../../../../../bounded-metric-transform.md) $d_b=\phi\circ d$. Symmetry and nonnegativity are immediate, and $d_b(x,y)=0$ exactly when $d(x,y)=0$, so $\boxed{d_b\text{ is a metric}}$.

Each $K_n$ is compact and lies inside $D$, so the [supremum norm](../../../../../supremum-norm.md) $\|f-g\|_n$ is finite for continuous $f,g$. Every summand of $\sigma$ lies between zero and $2^{-n}$, giving absolute convergence and $0\le\sigma\le1/2$. Symmetry is inherited from these norms. If $\sigma(f,g)=0$, all the nonnegative summands vanish, hence $f=g$ on every $K_n$; their union is $D$, so $f=g$ everywhere. Finally

$$
\|f-h\|_n\le\|f-g\|_n+\|g-h\|_n
$$

and the subadditivity already proved give the triangle inequality term by term and then after summation. Therefore $\boxed{\sigma\text{ is a metric on }\mathcal F}$. This is a [weighted metric for local uniform convergence](../../../../../weighted-metric-for-local-uniform-convergence.md), representing the [compact-open topology](../../../../../compact-open-topology.md).

The geometric-series sum is $s(z)=1/(1-z)$ and its remainder is $s-s_k=z^{k+1}/(1-z)$. Writing $r_n=1-1/n$, the triangle inequality gives

$$
\left|\frac{z^{k+1}}{1-z}\right|\le\frac{r_n^{k+1}}{1-r_n}=n r_n^{k+1}\qquad(|z|\le r_n).
$$

Equality occurs at the positive real point $z=r_n$. Thus

$$
\boxed{\|s_k-s\|_n=n(1-1/n)^{k+1}}.
$$

For every integer $N\ge2$, split the defining sum into a finite head and its tail. Since $\phi(t)\le t$ and $\phi(t)\le1$,

$$
\boxed{\sigma(s_k,s)\le\sum_{n=2}^{N}\|s_k-s\|_n+\sum_{n>N}2^{-n}
=\sum_{n=2}^{N}\|s_k-s\|_n+2^{-N}}.
$$

Given $\varepsilon>0$, choose $N$ with $2^{-N}<\varepsilon/2$. For that fixed $N$, each of the finitely many displayed norms tends to zero, so their sum is below $\varepsilon/2$ for sufficiently large $k$. Hence $\boxed{\sigma(s_k,s)\to0}$, even though convergence is not uniform on the whole open disk.

## ↑ Ancestors (10)

1. [11E](../11e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
