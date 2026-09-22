<h1 id="3/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Interpret the source's missing variable in the limit arrow as $t\to\infty$. We prove [convergence in distribution](../../../../../convergence-in-distribution.md) by showing that the angle of the [Brownian motion](../../../../../brownian-motion-split.md) becomes uniform on the [circle group](../../../../../circle-group.md).

Let $Z_t=e^{iB(t)}$. For every integer $m$, its angular [Fourier coefficients](../../../../../fourier-coefficient.md) satisfy

$$
\mathbb E[Z_t^m]=e^{-m^2t/2}
\longrightarrow
\begin{cases}1,&m=0,\\0,&m\ne0.\end{cases}
$$

These are precisely the [Fourier coefficients](../../../../../fourier-coefficient.md) of the [uniform distribution](../../../../../continuous-uniform-distribution.md) on the [unit circle](../../../../../complex-unit-circle.md). Thus [expectations](../../../../../expected-value-split.md) of every [trigonometric polynomial](../../../../../trigonometric-polynomial.md) converge to its uniform angular average. By the [Stone-Weierstrass theorem](../../../../../stone-weierstrass-theorem.md), [trigonometric polynomials](../../../../../trigonometric-polynomial.md) approximate continuous functions on the [unit circle](../../../../../complex-unit-circle.md) uniformly. Given an approximation error $\varepsilon$, the discrepancy of [expectations](../../../../../expected-value-split.md) is at most the polynomial discrepancy plus $2\varepsilon$. Taking $t\to\infty$ and then $\varepsilon\to0$ proves [weak convergence of probability measures](../../../../../weak-convergence-of-probability-measures.md) to uniform angular measure.

The [function](../../../../../function-split.md) $z\mapsto(\operatorname{Im}z)^2$ is continuous on the [unit circle](../../../../../complex-unit-circle.md), so the [continuous mapping theorem](../../../../../continuous-mapping-theorem.md) and part (a)(ii) imply

$$
\boxed{\Delta(t)\ \xrightarrow[t\to\infty]{\mathrm d}\ A,
\qquad A\sim\operatorname{Beta}\!\left(\frac12,\frac12\right).}
$$

Equivalently, the limiting [arcsine distribution](../../../../../arcsine-distribution.md) has [cumulative distribution function](../../../../../cumulative-distribution-function.md) $2\arcsin\sqrt{x}/\pi$ for $0\leq x\leq1$, and [probability density function](../../../../../probability-density-function.md) $1/(\pi\sqrt{x(1-x)})$ for $0<x<1$. This proves the limiting law rather than inferring it merely from the limiting [mean](../../../../../expected-value-split.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the random matrix theory course of the University of Oxford](../../../../split.md)
6. [Random matrix theory course of the University of Oxford](../../../../../random-matrix-theory-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
