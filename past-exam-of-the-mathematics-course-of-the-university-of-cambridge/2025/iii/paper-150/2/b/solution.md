<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $L=\log x$ and choose

$$
T=\exp(a\sqrt L),
\qquad
\sigma_0=1-\frac b{\sqrt L},
$$

with fixed positive $a,b$ chosen so that the rectangle up to height $T$ lies inside the [zero-free region of the Riemann zeta function](../../../../../../zero-free-region-of-the-riemann-zeta-function.md). Move the Perron contour from $1+1/L$ to $\sigma_0$. The only singularity crossed is the simple pole at $s=1$ of $-\zeta'(s)/\zeta(s)$, whose residue contributes $x$.

The standard bound $\zeta'(s)/\zeta(s)\ll(\log T)^2$ in this zero-free rectangle gives

$$
\int_{\sigma_0-iT}^{\sigma_0+iT}
\frac{\zeta'(s)}{\zeta(s)}\frac{x^s}{s}\,ds
\ll x^{\sigma_0}(\log T)^3
\ll x\exp(-b\sqrt L)L^{3/2}.
$$

The two horizontal sides are $\ll x(\log T)^2/T$, and the truncation error from part a is $\ll xL^2/T$. Polynomial factors in $L$ can be absorbed by slightly reducing the exponential constant. Thus some $c>0$ satisfies

$$
\sum_{n\leq x}\Lambda(n)
=x+O\left(x\exp(-c\sqrt{\log x})\right).
$$

This is the [Prime number theorem with classical zero-free-region error](../../../../../../prime-number-theorem-with-classical-zero-free-region-error.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 150](../../../paper-150-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
