<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [function](../../../../function-split.md) is continuous for $x>0$, hence [Lebesgue measurable](../../../../lebesgue-measurable-set.md). Near zero, the bound $|\sin x|\leq x$ gives

$$
\int_0^1\left|\frac{\sin x}{x^q}\right|\,dx
\leq\int_0^1x^{1-q}\,dx=\frac{1}{2-q}<\infty\qquad(0<q<2).
$$

Thus **$f$ is [Lebesgue integrable](../../../../lebesgue-integrable-function.md) on $(0,1]$ for $q<2$**. The convergence is an instance of [power singularity integrability](../../../../power-singularity-integrability.md).

For the tail, take the pairwise [disjoint](../../../../disjoint-sets.md) [intervals](../../../../interval-mathematics.md)

$$
I_k=\left[k\pi+\frac\pi6,\ k\pi+\frac{5\pi}6\right],\qquad k\geq1.
$$

On each $I_k$, $|\sin x|\geq1/2$, $x\leq(k+1)\pi$, and the interval length is $2\pi/3$. Therefore

$$
\int_{I_k}\frac{|\sin x|}{x^q}\,dx
\geq\frac{\pi}{3}\bigl((k+1)\pi\bigr)^{-q}
=\frac{\pi^{1-q}}{3(k+1)^q}.
$$

Summing the nonnegative [integrals](../../../../integral-split.md) over these [disjoint](../../../../disjoint-sets.md) [intervals](../../../../interval-mathematics.md) yields

$$
\int_1^\infty\frac{|\sin x|}{x^q}\,dx
\geq\frac{\pi^{1-q}}3\sum_{k=1}^\infty\frac1{(k+1)^q}=\infty
\qquad(0<q\leq1),
$$

by divergence of the [p-series](../../../../p-series.md). Hence **$f$ is not [Lebesgue integrable](../../../../lebesgue-integrable-function.md) on $[1,\infty)$ for $0<q\leq1$**.

The test is [absolute integrability](../../../../integrability.md): oscillatory sign cancellation does not make the absolute-value [integral](../../../../integral-split.md) finite. A conditionally convergent [improper integral](../../../../improper-integral.md) is a different notion. The [sine power kernel integrability](../../../../sine-power-kernel-integrability.md) criterion separates these endpoint thresholds.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the integration course of the University of Oxford](../../../split.md)
5. [Integration course of the University of Oxford](../../../../integration-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
