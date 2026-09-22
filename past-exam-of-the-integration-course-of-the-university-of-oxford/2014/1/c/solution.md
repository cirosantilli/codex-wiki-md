<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [function](../../../../function-split.md) is continuous for $x>0$, hence [Lebesgue measurable](../../../../lebesgue-measurable-set.md). On $(0,1)$, $|\sin x|\leq x$ and $|\cos x|\leq1$ give

$$
|f(x)|\leq\frac{x}{x\sqrt x}+\frac1{\sqrt x}=2x^{-1/2}.
$$

Since $\int_0^12x^{-1/2}\,dx=4$, **$f$ is [Lebesgue integrable](../../../../lebesgue-integrable-function.md) on $(0,1)$** by [power singularity integrability](../../../../power-singularity-integrability.md).

On $(1,\infty)$, the first summand is [Lebesgue integrable](../../../../lebesgue-integrable-function.md):

$$
\int_1^\infty\frac{|\sin x|}{x^{3/2}}\,dx\leq\int_1^\infty x^{-3/2}\,dx=2.
$$

The second summand is not. To prove it, take the pairwise [disjoint](../../../../disjoint-sets.md) [intervals](../../../../interval-mathematics.md)

$$
I_k=\left[k\pi-\frac\pi3,\ k\pi+\frac\pi3\right],\qquad k\geq1.
$$

On $I_k$, $|\cos x|\geq1/2$, the length is $2\pi/3$, and $x\leq(k+1)\pi$. Hence

$$
\int_{I_k}\frac{|\cos x|}{\sqrt x}\,dx
\geq\frac{\pi}{3\sqrt{(k+1)\pi}}
=\frac{\sqrt\pi}{3\sqrt{k+1}}.
$$

The [p-series](../../../../p-series.md) with exponent $1/2$ diverges, so $\int_1^\infty|\cos x|/\sqrt x\,dx=\infty$.

If $f$ were [Lebesgue integrable](../../../../lebesgue-integrable-function.md) on this tail, subtracting its integrable first summand would make $\cos x/\sqrt x$ integrable as well, a contradiction. Therefore

$$
\boxed{f\in L^1((0,1)),\qquad f\notin L^1((1,\infty)).}
$$

This uses the general fact that [an integrable perturbation cannot repair nonintegrability](../../../../an-integrable-perturbation-cannot-repair-nonintegrability.md). The conclusion concerns [absolute integrability](../../../../integrability.md); oscillatory cancellation in an [improper integral](../../../../improper-integral.md) is a separate issue.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2014](../../../2014-split.md)
4. [Past exam of the integration course of the University of Oxford](../../../split.md)
5. [Integration course of the University of Oxford](../../../../integration-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
