<h1 id="4c/solution">Solution</h1>

↑ **Parent:** [4C](../4c.md)

For a regular [space curve](../../../../../space-curve.md) parametrized by [arc length](../../../../../arc-length.md) $s$, its [curvature](../../../../../curvature.md) is $\kappa=\|dT/ds\|$, where $T=dx/ds$ is the unit tangent. Differentiating the given parametrization gives

$$
x'(t)=\frac{e^t}{2}(\cos t-\sin t,\ \sin t+\cos t,\ \sqrt2),\qquad \|x'(t)\|=e^t.
$$

The curve approaches the origin as $t\to-\infty$; the origin is a limiting endpoint. Its [arc length](../../../../../arc-length.md) measured from that endpoint is $s=\int_{-\infty}^t e^u\,du=e^t$, so

$$
\boxed{x(s)=\left(\frac s2\cos\log s,\ \frac s2\sin\log s,\ \frac s{\sqrt2}\right),\qquad s>0.}
$$

This is a [logarithmic conical helix](../../../../../logarithmic-conical-helix.md). Its unit tangent and derivative are

$$
T(s)=\frac12(\cos\log s-\sin\log s,\ \sin\log s+\cos\log s,\ \sqrt2),\qquad T'(s)=\frac1{2s}(-\sin\log s-\cos\log s,\ \cos\log s-\sin\log s,\ 0).
$$

Consequently,

$$
\boxed{\kappa(s)=\frac1{\sqrt2\,s}.}
$$

The infinitely many turns near the limiting origin have finite total [arc length](../../../../../arc-length.md), while the [curvature](../../../../../curvature.md) diverges there.

## ↑ Ancestors (10)

1. [4C](../4c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
