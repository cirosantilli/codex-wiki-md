<h1 id="8c/solution">Solution</h1>

↑ **Parent:** [8C](../8c.md)

Consider $G(z)=(e^{iz}-1)/(iz)$, extending it at zero by $G(0)=1$. It is [holomorphic](../../../../../complex-differentiability-at-a-point.md) in the upper half-plane and on its boundary, and on large upper semicircles $G(z)=O(1/|z|)$ because $|e^{iz}|\leq1$. For real $t$, indent the upper-half-plane contour above the pole of $G(z)/(z-t)$. The clockwise indentation contributes $-i\pi G(t)$, while the large semicircle contributes zero in the limit. The [Cauchy integral theorem](../../../../../cauchy-s-integral-theorem.md) gives

$$
\operatorname{PV}\int_{-\infty}^{\infty}\frac{G(\tau)}{\tau-t}\,d\tau=i\pi G(t).
$$

With the stated [Hilbert transform](../../../../../hilbert-transform.md) convention this is $\mathcal HG(t)=-iG(t)$. But

$$
G(t)=\frac{\sin t}{t}+i\frac{1-\cos t}{t}.
$$

Taking real parts yields the [Hilbert transform of the sinc function](../../../../../hilbert-transform-of-the-sinc-function.md):

$$
\boxed{\mathcal H\!\left(\frac{\sin t}{t}\right)=\frac{1-\cos t}{t}.}
$$

At $t=0$ the right side has limit zero; the same value follows by oddness of the principal-value integrand. The apparent singularity of $G$ at zero is removable, so the contour calculation is valid there too.

## ↑ Ancestors (10)

1. [8C](../8c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
