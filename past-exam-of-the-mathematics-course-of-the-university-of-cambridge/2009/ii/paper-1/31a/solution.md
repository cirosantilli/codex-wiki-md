<h1 id="31a/solution">Solution</h1>

↑ **Parent:** [31A](../31a.md)

[Watson's lemma](../../../../../watson-s-lemma.md) gives, under integrability away from zero and the stated endpoint [asymptotic expansion](../../../../../asymptotic-expansion.md),

$$
\boxed{I(\lambda)\sim\sum_{n=0}^\infty\frac{a_n\Gamma(n\beta+1)}{\lambda^{n\beta+1}}.}
$$

Indeed each power integrates over the positive half-line to $\Gamma(n\beta+1)\lambda^{-(n\beta+1)}$; replacing a fixed upper endpoint by infinity has exponentially small error. A remainder $o(t^{N\beta})$ near zero gives $o(\lambda^{-N\beta-1})$ after splitting off a small endpoint neighbourhood and rescaling $u=\lambda t$.

For [Laplace's method](../../../../../laplace-s-method.md), assume the phase and amplitude are smooth near the nondegenerate maximum, as required for a full expansion. Localize to a small neighbourhood of $c$: outside it the unique maximum and continuity make the exponential smaller by a factor $e^{-\lambda\varepsilon}$. Set

$$
\zeta=\operatorname{sgn}(t-c)\sqrt{2(\phi(c)-\phi(t))}.
$$

Near $c$ this is a smooth increasing coordinate, with $\zeta'(c)=\sqrt{|\phi''(c)|}$. It need not be monotonic on the entire integration interval. In the localized integral put $A(\zeta)=F(t(\zeta))\,dt/d\zeta$. Extending its Gaussian integration to both infinite endpoints incurs exponentially small error. Taylor expansion of $A$ and integration of even Gaussian moments gives

$$
J(\lambda)\sim e^{\lambda\phi(c)}\sqrt{2\pi}\sum_{j\geq0}
\frac{A^{(2j)}(0)}{2^j j!\,\lambda^{j+1/2}}.
$$

Here $A(0)=F(c)/\sqrt{|\phi''(c)|}$, giving **the leading term $\boxed{e^{\lambda\phi(c)}F(c)\sqrt{2\pi/(\lambda|\phi''(c)|)}}$**. The asymptotic-equivalence notation for that term presumes $F(c)\ne0$; if it vanishes the series determines the first nonzero term. The maximum condition alone, without amplitude regularity, would not imply a full expansion.

For the [gamma function](../../../../../gamma-function.md), set $t=xs$:

$$
\Gamma(x+1)=x^{x+1}\int_0^\infty e^{x(\log s-s)}\,ds.
$$

The phase has unique maximum $-1$ at $s=1$, with second derivative $-1$. To obtain the correction, put $s=1+u/\sqrt x$. Expansion gives

$$
x(\log s-s)=-x-\frac{u^2}{2}+\frac{u^3}{3\sqrt x}-\frac{u^4}{4x}+O(x^{-3/2}u^5),
$$

and hence a Gaussian multiplier

$$
1+\frac{u^3}{3\sqrt x}+\frac1x\left(-\frac{u^4}4+\frac{u^6}{18}\right)+\cdots.
$$

The odd term integrates to zero. The normalized Gaussian fourth and sixth moments are 3 and 15, so the correction is $-3/4+15/18=1/12$. Localization near one, with the exponentially suppressed endpoint tails, justifies termwise expansion. Thus [Stirling's formula](../../../../../stirling-formula.md) is

$$
\boxed{\Gamma(x+1)\sim\sqrt{2\pi}\,x^{x+1/2}e^{-x}\left(1+\frac1{12x}+O(x^{-2})\right).}
$$

## ↑ Ancestors (10)

1. [31A](../31a.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
