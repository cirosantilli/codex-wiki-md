<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

By [Dirichlet's theorem on Fourier series](../../../../../../dirichlet-s-theorem-on-fourier-series.md), a piecewise continuously differentiable [periodic function](../../../../../../periodic-function.md) has a [Fourier series](../../../../../../fourier-series-split.md) converging at each point to the average of its one-sided limits. In particular it converges to the [function](../../../../../../function-split.md) at every point of [continuity](../../../../../../continuous-function.md). Our [periodic extension](../../../../../../periodic-extension.md) satisfies these hypotheses, and $x=\pi/2$ is a point of [continuity](../../../../../../continuous-function.md) with $f(\pi/2)=\pi^2/4$.

At this point $\sin(n\pi/2)=0$ for even $n$. For $n=2j-1$,

$$
\sin\frac{(2j-1)\pi}{2}=(-1)^{j+1},\qquad
b_{2j-1}=\frac{2\pi}{2j-1}-\frac8{\pi(2j-1)^3}.
$$

Substituting in the [Fourier series](../../../../../../fourier-series-split.md) from part (c) proves

$$
\boxed{\frac{\pi^2}{4}=\sum_{j=1}^{\infty}(-1)^{j+1}\left[\frac{2\pi}{2j-1}-\frac8{\pi(2j-1)^3}\right].}
$$

The sum is taken in its displayed order. Discarding its zero even-indexed terms is valid and does not rearrange the remaining terms.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [4](../../4.md)
3. [Mathematics V](../../../mathematics-v-split.md)
4. [Prelims](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
