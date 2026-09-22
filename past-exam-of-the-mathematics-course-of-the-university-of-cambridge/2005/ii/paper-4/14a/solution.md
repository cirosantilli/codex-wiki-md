<h1 id="14a/solution">Solution</h1>

↑ **Parent:** [14A](../14a.md)

The [Dirichlet series](../../../../../dirichlet-series.md) for the [Riemann zeta function](../../../../../riemann-zeta-function.md) converges for $\Re z>1$. In the Hankel [integral representation](../../../../../integral-representation.md) the branch is a branch of $t^{z-1}$, so the argument restriction concerns $t$, not the parameter $z$. Use the principal branch cut along the negative real axis and a positive Hankel loop with a fixed small indentation around zero. Its integral $I(z)$ is an entire function of $z$, since the tails have exponential decay and the fixed contour avoids zero. Multiplication by $\Gamma(1-z)/(2\pi i)$ gives the [meromorphic continuation](../../../../../meromorphic-continuation.md) of $\zeta$: it is directly defined away from positive integers, has a pole at $1$, and the apparent singularities at $2,3,\ldots$ are interpreted by limits.

For a check in the initial half-plane, collapsing the indentation for $\Re z>1$ gives

$$
I(z)=2i\sin(\pi z)\int_0^\infty\frac{r^{z-1}}{e^r-1}\,dr
=2i\sin(\pi z)\Gamma(z)\zeta(z).
$$

Expansion of $(e^r-1)^{-1}$ into exponentials justifies the last equality there, and the [Gamma reflection formula](../../../../../gamma-reflection-formula.md) recovers the printed [integral representation](../../../../../integral-representation.md).

Take the upper semicircle contour with the straight segment oriented from left to right, making the total orientation positive. Its enclosed poles are $t=2\pi ij$, $j=1,\ldots,N$; each has [residue](../../../../../residue.md) $-(2\pi ij)^{z-1}$. Thus

$$
\boxed{\int_\gamma\frac{t^{z-1}}{e^{-t}-1}\,dt
=-2\pi i(2\pi)^{z-1}e^{i\pi(z-1)/2}\sum_{j=1}^N j^{z-1}}.
$$

The reverse orientation changes the sign.

Initially take $\Re z<0$, so the series on the right converges as $N\to\infty$ and the large arcs can be discarded under the given assumption. Denote by $L_+$ and $L_-$ the integrals along horizontal lines just above and below the real axis, both from left to right. The [residue](../../../../../residue.md) computation and its lower-half-plane clockwise counterpart give

$$
L_+=-2\pi i(2\pi i)^{z-1}\zeta(1-z),\qquad
L_-=2\pi i(-2\pi i)^{z-1}\zeta(1-z).
$$

Contour deformation about the negative-axis branch cut gives $I=L_--L_+$. Hence

$$
I(z)=4\pi i(2\pi)^{z-1}\sin(\pi z/2)\zeta(1-z).
$$

Multiplying by $\Gamma(1-z)/(2\pi i)$ yields

$$
\boxed{\zeta(z)=2^z\pi^{z-1}\sin(\pi z/2)\Gamma(1-z)\zeta(1-z)}.
$$

It extends by [meromorphic continuation](../../../../../meromorphic-continuation.md) to all $z\ne1$, with removable products evaluated by limits where individual factors diverge. The derivation does not assert ordinary convergence of the original positive-term series outside $\Re z>1$.

## ↑ Ancestors (10)

1. [14A](../14a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
