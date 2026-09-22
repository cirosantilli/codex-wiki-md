<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the graph of a differentiable function, the [arc length](../../../../../../arc-length.md) is $L=\int\sqrt{1+(y')^2}\,dx$. Since $y'=2x$,

$$
L=\int_0^1\sqrt{1+4x^2}\,dx.
$$

Use the [hyperbolic substitution](../../../../../../hyperbolic-substitution.md) $2x=\sinh t$: then $dx=\tfrac12\cosh t\,dt$ and $\sqrt{1+4x^2}=\cosh t$. The [hyperbolic functions](../../../../../../hyperbolic-function.md) $\cosh^2t=(1+\cosh2t)/2$ yields

$$
L=\left[\frac{x}{2}\sqrt{1+4x^2}+\frac14\operatorname{arsinh}(2x)\right]_0^1
=\boxed{\frac{\sqrt5}{2}+\frac14\ln(2+\sqrt5).}
$$

Here $\operatorname{arsinh}t=\ln(t+\sqrt{1+t^2})$ is the [inverse hyperbolic sine](../../../../../../inverse-hyperbolic-sine.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [Mathematics III resit](../../../mathematics-iii-resit-split.md)
4. [Prelims](../../../split.md)
5. [Undated](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
