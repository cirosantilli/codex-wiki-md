<h1 id="2f/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $K=\{z:|\operatorname{Re}z|+|\operatorname{Im}z|\leq1\}$. Choose a unit complex number $u$ normal to a supporting side of this [convex set](../../../../../../convex-set.md), with

$$
\operatorname{Re}(\overline u\zeta)>h:=\max_{z\in K}\operatorname{Re}(\overline uz).
$$

Such a choice exists explicitly: take $u=(s+it)/\sqrt2$, where $s,t\in\{-1,1\}$ are the signs of the real and imaginary parts of $\zeta$; then $h=1/\sqrt2$ and the strict inequality is exactly the hypothesis. Set $c=-Ru$. Since $|z|\leq1$ on $K$,

$$
|z-c|^2\leq R^2+2Rh+1,\qquad |\zeta-c|^2=R^2+2R\operatorname{Re}(\overline u\zeta)+|\zeta|^2.
$$

For sufficiently large $R$, the former is strictly smaller than the latter uniformly on $K$. Consequently $q=\max_K|z-c|/|\zeta-c|<1$.

The [geometric series](../../../../../../geometric-series.md) now supplies actual approximating [polynomials](../../../../../../polynomial-split.md):

$$
p_N(z)=-\frac1{\zeta-c}\sum_{j=0}^N\left(\frac{z-c}{\zeta-c}\right)^j,\qquad
\sup_{z\in\Gamma}\left|p_N(z)-\frac1{z-\zeta}\right|\leq\frac{q^{N+1}}{|\zeta-c|(1-q)}.
$$

Choose $N$ so the right-hand side is below $\epsilon$. This proves the required [uniform approximation](../../../../../../uniform-approximation-split.md) without assuming a general approximation theorem.

$$
\boxed{\sup_{z\in\Gamma}|p_N(z)-(z-\zeta)^{-1}|<\epsilon\quad\text{for sufficiently large }N.}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2F](../../2f.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
