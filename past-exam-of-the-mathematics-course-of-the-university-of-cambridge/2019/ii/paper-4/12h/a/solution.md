<h1 id="12h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let

$$
S=\{x+iy:-1\leq x,y\leq1\},
$$

and choose $0<\eta<\delta$. Write $C_\eta$ for the positively oriented boundary of the square with $|x|,|y|\leq1+\eta$. The [Cauchy integral formula](../../../../../../cauchy-integral-formula.md) gives, for every $z\in S$,

$$
f(z)=\frac1{2\pi i}\int_{C_\eta}\frac{f(\zeta)}{\zeta-z}\,d\zeta.
$$

Because $C_\eta$ and $S$ are compact and separated by a positive distance, Riemann sums for this contour integral converge uniformly in $z\in S$. Thus, for any $\varepsilon>0$, there are points $\zeta_j\in C_\eta$ and constants $c_j$ such that

$$
\sup_{z\in S}\left|f(z)-\sum_{j=1}^m\frac{c_j}{z-\zeta_j}\right|<\frac\varepsilon2.
$$

It remains to approximate each resolvent by polynomials on $S$. Let $\Lambda$ be the set of $\lambda\notin S$ for which $(z-\lambda)^{-1}$ is polynomially uniformly approximable on $S$. If $|\lambda|>\sup_{z\in S}|z|$, the [geometric series](../../../../../../geometric-series.md)

$$
\frac1{z-\lambda}
=-\frac1\lambda\sum_{n=0}^{\infty}\left(\frac z\lambda\right)^n
$$

shows that $\lambda\in\Lambda$. Moreover, the [resolvent propagation across a complementary component](../../../../../../resolvent-propagation-across-a-complementary-component.md) argument shows that $\Lambda$ is both open and closed relative to $\mathbb C\setminus S$. The complement of a square is [connected](../../../../../../connected-space.md), and $\Lambda$ is nonempty, so $\Lambda=\mathbb C\setminus S$.

In particular, every $\zeta_j$ lies in $\Lambda$. Approximate the finitely many resolvents accurately enough that their weighted sum differs by less than $\varepsilon/2$. Combining this with the Riemann-sum estimate produces a polynomial $p$ satisfying

$$
\sup_{z\in K}|f(z)-p(z)|
\leq\sup_{z\in S}|f(z)-p(z)|
<\varepsilon.
$$

This proves the claimed [elementary polynomial approximation on a square](../../../../../../elementary-polynomial-approximation-on-a-square.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [12H](../../12h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
