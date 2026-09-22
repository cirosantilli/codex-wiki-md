<h1 id="4/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $Df(x)$ denote the upper limit of the displayed mean oscillation as $r\downarrow0$. For a continuous integrable approximation $g$, continuity gives $Dg(x)=0$. With $h=f-g$, the [triangle inequality](../../../../../triangle-inequality.md) yields

$$
Df(x)\leq Mh(x)+|h(x)|.
$$

Therefore the maximal inequality and [Chebyshev's inequality](../../../../../chebyshev-s-inequality.md) give

$$
\lambda(\{Df>2\varepsilon\})\leq\lambda(\{Mh>\varepsilon\})+\lambda(\{|h|>\varepsilon\})\leq\frac4\varepsilon\|f-g\|_1.
$$

Density makes the right side arbitrarily small. For each positive rational $\varepsilon$ the exceptional set is null, proving **$Df=0$ [almost everywhere](../../../../../almost-everywhere.md)**, the [Lebesgue differentiation theorem](../../../../../lebesgue-differentiation-theorem.md). Values where the chosen representative is not finite already form a [null set](../../../../../null-set.md).

For the fundamental theorem define $F(x)=\int_a^xf(t)dt$, with oriented integration for $x<a$. This function is absolutely continuous: for disjoint intervals the sum of $|F(b_j)-F(a_j)|$ is at most the integral of $|f|$ over their union, which is small when its [measure](../../../../../measure-split.md) is small by [absolute continuity](../../../../../absolutely-continuous-function.md) of the integral. At a [Lebesgue point](../../../../../lebesgue-point.md) of $f$, for $h\ne0$,

$$
\left|\frac{F(x+h)-F(x)}h-f(x)\right|\leq\frac1{|h|}\int_{x-|h|}^{x+|h|}|f(t)-f(x)|dt\to0.
$$

Thus **$F'=f$ [almost everywhere](../../../../../almost-everywhere.md)** and $F(b)-F(a)=\int_a^bf$. Differentiability at every point is not claimed for an arbitrary integrable function.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the real and harmonic analysis course of the University of Oxford](../../../../split.md)
6. [Real and harmonic analysis course of the University of Oxford](../../../../../real-and-harmonic-analysis-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
