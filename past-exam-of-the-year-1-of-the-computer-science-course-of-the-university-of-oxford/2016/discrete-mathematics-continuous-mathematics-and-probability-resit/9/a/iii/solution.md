<h1 id="9/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $S(x)=\mathbb P(X>x)=1-F_X(x)$ for $x\geq0$. Since $f_X=0$ on the negative half-line, $X\geq0$ almost surely. We have $S'=-f_X$ almost everywhere. On a finite interval, [integration by parts](../../../../../../integration-by-parts.md) gives

$$
\int_0^R x f_X(x)\,dx
=-\int_0^R xS'(x)\,dx
=-RS(R)+\int_0^R S(x)\,dx.
$$

The lower endpoint contributes zero. The stated hypothesis gives $RS(R)\to0$ as $R\to\infty$. Taking the increasing limits of the two nonnegative [integrals](../../../../../../integral-split.md) proves the [tail-integral identity](../../../../../../tail-integral-formula-for-expectation.md)

$$
\boxed{\mathbb E(X)=\int_0^{\infty}\mathbb P(X>x)\,dx}.
$$

The equality allows the value $+\infty$; the boundary hypothesis alone does not force a finite expectation. In fact the formula for nonnegative $X$ also follows directly from [Tonelli theorem](../../../../../../tonelli-theorem.md), without that additional boundary hypothesis, by integrating $x=\int_0^{\infty}\mathbf1_{\{t<x\}}\,dt$ against the [probability density function](../../../../../../probability-density-function.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [9](../../../9.md)
4. [Discrete mathematics, continuous mathematics and probability (resit)](../../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
5. [2016](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
