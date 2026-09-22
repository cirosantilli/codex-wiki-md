<h1 id="8e/solution">Solution</h1>

↑ **Parent:** [8E](../8e.md)

The removable singularities at zero are understood in

$$
\boxed{F^+(z)=\frac{e^{iz}-1}{2iz},\qquad F^-(z)=\frac{e^{-iz}-1}{2iz}}.
$$

These are [entire functions](../../../../../entire-function.md), with values $F^+(0)=1/2$ and $F^-(0)=-1/2$. On the real axis their difference is $\sin x/x$, including its continuous value at zero. In the [complex upper half-plane](../../../../../upper-half-plane-complex-analysis.md), $|e^{iz}|\leq1$, so $|F^+(z)|\leq1/|z|$ away from zero; the analogous bound for $F^-$ holds in the [lower half-plane](../../../../../lower-half-plane.md). This verifies analyticity, the required jump and the specified decay.

In the [Sokhotski–Plemelj formula](../../../../../sokhotski-plemelj-theorem.md), the boundary values may also be written

$$
F^\pm(x)=\pm\frac{\sin x}{2x}+\frac{\cos x-1}{2ix}.
$$

Indeed the [Cauchy principal value](../../../../../cauchy-principal-value.md) of $\sin t/[t(t-x)]$ is $\pi(\cos x-1)/x$: split $1/[t(t-x)]=x^{-1}((t-x)^{-1}-t^{-1})$, translate the first integral, and use $\int_{\mathbb R}\sin t/t\,dt=\pi$ and the oddness of $\cos t/t$. The limiting formula at zero follows continuously.

## ↑ Ancestors (10)

1. [8E](../8e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
