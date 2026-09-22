<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\phi$ be a [test function](../../../../../../test-function.md) supported in $[-R,R]$. Symmetric cancellation gives

$$
\operatorname{PV}\frac1x(\phi)=\int_0^R\frac{\phi(x)-\phi(-x)}x\,dx.
$$

The integrand is bounded by $2\|\phi'\|_\infty$, so the limit exists and

$$
\left|\operatorname{PV}\frac1x(\phi)\right|\leq2R\|\phi'\|_\infty.
$$

This is a continuous linear functional on every fixed-support test space, hence a [distribution](../../../../../../distribution-mathematical-analysis.md). It also specifies its local order as at most one.

For the boundary value, split the ordinary complex denominator:

$$
\frac1{x+i\varepsilon}=\frac{x}{x^2+\varepsilon^2}-i\frac{\varepsilon}{x^2+\varepsilon^2},\qquad\varepsilon>0.
$$

The real part paired with $\phi$ is

$$
\int_0^R\frac{x[\phi(x)-\phi(-x)]}{x^2+\varepsilon^2}\,dx.
$$

It converges to the principal value by [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md), using the same bound $2\|\phi'\|_\infty$. In the second part set $x=\varepsilon t$:

$$
\int_\mathbb R\frac{\varepsilon\phi(x)}{x^2+\varepsilon^2}\,dx=\int_\mathbb R\frac{\phi(\varepsilon t)}{1+t^2}\,dt\longrightarrow\pi\phi(0).
$$

Here $\|\phi\|_\infty/(1+t^2)$ is an integrable majorant. The correct [Sokhotski–Plemelj formula](../../../../../../sokhotski-plemelj-theorem.md) is therefore

$$
\boxed{\frac1{x+i0}=\operatorname{PV}\frac1x-i\pi\delta.}
$$

The resulting functional is continuous, with bound $2R\|\phi'\|_\infty+\pi\|\phi\|_\infty$, so it too is a [distribution](../../../../../../distribution-mathematical-analysis.md).

**The printed PDF has the wrong sign on its delta term.** For a real even nonnegative [test function](../../../../../../test-function.md) with $\phi(0)>0$, the principal value is zero while the imaginary part of every regularized integral is negative. Its limit is $-\pi\phi(0)$, disproving the printed plus sign directly. A plus sign instead belongs to the boundary value $(x-i0)^{-1}$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
