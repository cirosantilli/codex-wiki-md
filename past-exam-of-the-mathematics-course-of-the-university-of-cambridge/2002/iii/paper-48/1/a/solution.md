<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $L=\log\lambda$ and integrate by parts using $x^{-2}=-d(x^{-1})/dx$. The exponential cutoff has [derivative](../../../../../../derivative.md) $\lambda e^{-x}e^{-\lambda e^{-x}}$, so the endpoint at infinity vanishes and the lower endpoint gives

$$
I(\lambda)=e^{-\lambda/e}+\int_1^\infty\frac{\lambda e^{-x}e^{-\lambda e^{-x}}}{x}\,dx.
$$

With $u=\lambda e^{-x}$ this becomes

$$
I(\lambda)=e^{-\lambda/e}+\int_0^{\lambda/e}\frac{e^{-u}}{L-\log u}\,du.
$$

The mass of the transformed [integral](../../../../../../integral.md) lies at $u=O(1)$, where

$$
\frac1{L-\log u}=\frac1L+\frac{\log u}{L^2}
+O\left(\frac{(\log u)^2}{L^3}\right).
$$

To control this [asymptotic expansion](../../../../../../asymptotic-expansion.md), split at $u=e^{-L/2}$ and $u=e^{L/2}$. On the central interval the geometric-series remainder is bounded by $2(\log u)^2/L^3$, whose [integral](../../../../../../integral.md) against $e^{-u}$ is finite. The lower tail has length $e^{-L/2}$ and denominator at least $L$; the upper tail is exponentially small in $e^{L/2}$, with the original denominator at least one. The omitted tails of the logarithmic moments are likewise negligible. Thus extending the moments to $(0,\infty)$ is justified.

The [Gamma function](../../../../../../gamma-function.md) gives $\int_0^\infty e^{-u}\,du=1$, and the first logarithmic moment is $-\gamma$, with $\gamma$ [Euler's constant](../../../../../../euler-s-constant.md). Therefore

$$
\boxed{I(\lambda)=\frac1{\log\lambda}
-\frac\gamma{(\log\lambda)^2}
+O\bigl((\log\lambda)^{-3}\bigr)}.
$$

This is the [moving Gumbel cutoff in an inverse-power tail](../../../../../../moving-gumbel-cutoff-in-an-inverse-power-tail.md): replacing the original cutoff by a sharp step at $x=\log\lambda$ gives the first term, but its smooth transition supplies the Euler-constant correction.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 48](../../../paper-48-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
