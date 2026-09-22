<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Allow $g_D$ to take the value $+\infty$. Fix a closed ball $\overline{B(z,r)}\subset D$, independently choose a radius $R$ with density $ns^{n-1}/r^n$ on $(0,r)$, and let $S$ be the first time the [Brownian motion](../../../../../../brownian-motion-split.md) from $z$ reaches that radius. Conditional on $R=s$, the [Strong Markov property](../../../../../../strong-markov-property.md) at $S$ decomposes the remaining [Brownian exit time](../../../../../../brownian-exit-time.md) from $D$. Since $S<T_D$ and the conditional exit time has mean $s^2/n$, [Tonelli's theorem](../../../../../../tonelli-theorem.md) and part (a) give the [Brownian exit-time ball averaging identity](../../../../../../brownian-exit-time-ball-averaging-identity.md)

$$
g_D(z)=\mathbb E_zS+\mathbb E_zg_D(W_S)
=\frac{r^2}{n+2}+\frac1{|B(z,r)|}\int_{B(z,r)}g_D(w)\,dw.
$$

This identity is valid in the extended nonnegative reals; no finiteness was assumed to derive it.

If $g_D(z)<\infty$, the integral over $B(z,r)$ is finite. For any $y\in B(z,r)$ choose $\rho>0$ with $\overline{B(y,\rho)}\subset B(z,r)$. The same identity at $y$ has a finite right side because its integral is over a subset of the integrable ball. Thus $g_D(y)<\infty$. The set $F=\{z\in D:g_D(z)<\infty\}$ is therefore open relative to $D$.

It is also relatively closed. If $z_j\in F$ converges to $y\in D$, choose $r>0$ with $\overline{B(y,3r)}\subset D$. For large $j$, $|z_j-y|<r$, and $\overline{B(z_j,2r)}\subset D$. The preceding argument shows that every point in $B(z_j,2r)$, including $y$, belongs to $F$. Hence $F$ is closed in $D$. Since $F$ is nonempty and $D$ is [connected](../../../../../../connected-space.md), **$g_D(y)<\infty$ for every $y\in D$**. This proves [finiteness propagation of Brownian mean exit times](../../../../../../finiteness-propagation-of-brownian-mean-exit-times.md) without assuming beforehand that $g_D$ solves a smooth [Poisson equation](../../../../../../poisson-equation.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
