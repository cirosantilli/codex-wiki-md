<h1 id="a/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The vertical integral is [absolutely convergent](../../../../absolute-convergence.md) because the denominator is quadratic in the imaginary part. If $x<1$, move its line to the right: no poles are crossed, and the integral on $\operatorname{Re}s=R$ is $O(x^R/R)$, tending to [zero](../../../../zero-of-a-function.md). If $x>1$, move left across the simple poles at $0,-1$. Their residues are $1$ and $-x^{-1}$, and the far-left integral tends to [zero](../../../../zero-of-a-function.md). Horizontal segments vanish by their $O(|\operatorname{Im}s|^{-2})$ decay for a fixed pair of vertical lines. At $x=1$, dominated convergence on the original line gives the limiting value [zero](../../../../zero-of-a-function.md). Hence the [kernel](../../../../kernel-of-a-linear-map-split.md) is $0$ below one and $1-x^{-1}$ at or above one.

On a line $c>2$, [absolute convergence](../../../../absolute-convergence.md) permits interchanging the totient [Dirichlet series](../../../../dirichlet-series.md) and this integral. The $n$th term is $x\phi(n)$ times the [kernel](../../../../kernel-of-a-linear-map-split.md) at $x/n$, giving exactly $\phi(n)(x-n)$ for $n\le x$. Thus

$$
S(x):=\sum_{n\le x}\phi(n)(x-n)
=\frac1{2\pi i}\int_{c-i\infty}^{c+i\infty}
\frac{\zeta(s-1)}{\zeta(s)}\frac{x^{s+1}}{s(s+1)}\,ds.
$$

We may take $c=5/2$ and shift to $\operatorname{Re}s=3/2$. The denominator has no zeros in this strip; the only [pole](../../../../pole.md) crossed is $s=2$, where $\zeta(s-1)$ has [residue](../../../../residue.md) one. Its [residue](../../../../residue.md) in the integrand is

$$
\frac{x^3}{6\zeta(2)}=\frac{x^3}{\pi^2}.
$$

On the new line, the supplied estimates bound the integrand by $O(x^{5/2}|t|^{-3/2}\log^8|t|)$ for $|t|\ge2$, an integrable function. The compact portion is bounded as well. The same estimates, uniformly across the strip, make the horizontal integrals tend to [zero](../../../../zero-of-a-function.md). Consequently

$$
\boxed{S(x)=\frac{x^3}{\pi^2}+O(x^{5/2})\sim\frac{x^3}{\pi^2}.}
$$

For the Tauberian step let $A(x)=\sum_{n\le x}\phi(n)$. It is nondecreasing because the summands are nonnegative, and $S(x)=\int_0^xA(t)\,dt$. For fixed $0<\epsilon<1$,

$$
\frac{S(x)-S((1-\epsilon)x)}{\epsilon x}
\le A(x)\le
\frac{S((1+\epsilon)x)-S(x)}{\epsilon x}.
$$

After division by $x^2$ and passage to lower and upper limits, the asymptotic for $S$ gives bounds $(3-3\epsilon+\epsilon^2)/\pi^2$ and $(3+3\epsilon+\epsilon^2)/\pi^2$. Letting $\epsilon\downarrow0$ squeezes them together. Therefore

$$
\boxed{\sum_{n\le x}\phi(n)\sim\frac{3x^2}{\pi^2}.}
$$

This uses monotonicity of the summatory function; differentiating an asymptotic formula without such control would not justify the conclusion.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [A](../../a.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the analytic number theory and elliptic curves course of the University of Oxford](../../../split.md)
5. [Analytic number theory and elliptic curves course of the University of Oxford](../../../../analytic-number-theory-and-elliptic-curves-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
