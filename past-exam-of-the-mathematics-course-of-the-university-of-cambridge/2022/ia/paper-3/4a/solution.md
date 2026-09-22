<h1 id="4a/solution">Solution</h1>

↑ **Parent:** [4A](../4a.md)

Use $x>0$ as the parameter of the [smooth curve](../../../../../smooth-curve.md):

$$
\mathbf r(x)=(x,\log x,0).
$$

Its [velocity vector](../../../../../velocity-vector.md) and speed are

$$
\mathbf r'(x)=\left(1,\frac1x,0\right),
\qquad
|\mathbf r'(x)|=\frac{\sqrt{x^2+1}}x.
$$

The [unit tangent vector](../../../../../unit-tangent-vector.md) is therefore

$$
\boxed{\mathbf t(x)=\frac{(x,1,0)}{\sqrt{x^2+1}}}.
$$

The parameter-independent formula for the [curvature of a space curve](../../../../../curvature-of-a-space-curve.md) gives

$$
\kappa(x)
=\frac{|\mathbf r'(x)\times\mathbf r''(x)|}
{|\mathbf r'(x)|^3}
=\boxed{\frac{x}{(x^2+1)^{3/2}}}.
$$

Differentiating,

$$
\kappa'(x)=\frac{1-2x^2}{(x^2+1)^{5/2}}.
$$

Hence $\kappa$ increases for $0<x<1/\sqrt2$ and decreases for $x>1/\sqrt2$. Its [global maximum](../../../../../global-maximum.md) occurs at $x=1/\sqrt2$ and equals

$$
\boxed{\kappa_{\max}=\frac{2}{3\sqrt3}}.
$$

The corresponding point is

$$
\boxed{\left(\frac1{\sqrt2},-\frac12\log2,0\right)}.
$$

## ↑ Ancestors (10)

1. [4A](../4a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
