<h1 id="30d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [phase function](../../../../../../phase-function.md) $\cos t$ attains its global maximum $1$ on $[0,3\pi]$ at the stationary endpoint $t=0$ and at the interior point $t=2\pi$. At either point,

$$
\cos(t_0+u)=1-\frac{u^2}{2}+O(u^4).
$$

By [Laplace's method at a nondegenerate stationary endpoint](../../../../../../laplace-s-method-at-a-nondegenerate-stationary-endpoint.md), the endpoint contributes

$$
e^x\sqrt{\frac{\pi}{2x}}.
$$

By [Laplace's method](../../../../../../laplace-s-method.md), the interior maximum contributes

$$
e^{x+2\pi}\sqrt{\frac{2\pi}{x}}.
$$

The remaining parts of the interval are exponentially smaller. Summing the two contributions according to [Laplace's method with multiple global maxima](../../../../../../laplace-s-method-with-multiple-global-maxima.md) gives

$$
\boxed{
I(x)\sim e^x\sqrt{\frac{\pi}{2x}}
\left(1+2e^{2\pi}\right)}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [30D](../../30d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
