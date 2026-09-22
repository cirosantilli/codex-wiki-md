<h1 id="11c/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Away from the origin the [gradients](../../../../../../../gradient.md) are $\nabla u=\widehat{\mathbf r}/a$ and $\nabla v=-\widehat{\mathbf r}/r^2$. The improper [volume integral](../../../../../../../volume-integral.md) is therefore

$$
\lim_{\varepsilon\downarrow0}\int_{\varepsilon<r<a}-\frac{1}{ar^2}\,dV
=-\frac{4\pi}{a}\lim_{\varepsilon\downarrow0}\int_\varepsilon^a dr=\boxed{-4\pi}.
$$

The function $v=1/r$ is a [harmonic function](../../../../../../../harmonic-function.md) only off the origin. It is singular inside the integration volume, so it does not meet part (a)'s regularity hypothesis. On the punctured ball, [Green's first identity](../../../../../../../green-s-first-identity.md) has outer flux $-4\pi$ and inner flux $4\pi\varepsilon/a$: the inner outward [unit normal](../../../../../../../unit-normal.md) is $-\widehat{\mathbf r}$, so $u\partial_n v=(\varepsilon/a)/\varepsilon^2$. Their sum is $-4\pi+4\pi\varepsilon/a$, exactly the integral before taking the limit. Equivalently the distributional [Laplacian](../../../../../../../laplacian.md) of $1/r$ is $-4\pi\delta_0$, rather than zero throughout the ball. This is [boundary flux from a singular harmonic potential](../../../../../../../boundary-flux-from-a-singular-harmonic-potential.md); it explains why applying part (a) across the origin would be invalid.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [11C](../../../11c.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ia](../../../../split.md)
6. [2008](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
