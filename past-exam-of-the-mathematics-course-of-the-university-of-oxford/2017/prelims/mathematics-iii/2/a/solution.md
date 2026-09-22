<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In [Cartesian coordinates](../../../../../../cartesian-coordinate-system.md), a [parametrization](../../../../../../parametric-equation.md) of the [curve](../../../../../../curve.md) is

$$
x(\theta)=f(\theta)\cos\theta,\qquad y(\theta)=f(\theta)\sin\theta.
$$

Differentiate using the [product rule](../../../../../../product-rule.md):

$$
x'=f'\cos\theta-f\sin\theta,\qquad y'=f'\sin\theta+f\cos\theta.
$$

Squaring and adding cancels the mixed terms, giving $(x')^2+(y')^2=(f')^2+f^2$. The [arc length](../../../../../../arc-length.md) is the integral of the speed, so

$$
\boxed{L=\int_0^{2\pi}\sqrt{f(\theta)^2+f'(\theta)^2}\,d\theta.}
$$

This assumes the [parametrization](../../../../../../parametric-equation.md) is piecewise continuously differentiable and counts length with multiplicity if the [curve](../../../../../../curve.md) is retraced.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [Mathematics III](../../../mathematics-iii-split.md)
4. [Prelims](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
