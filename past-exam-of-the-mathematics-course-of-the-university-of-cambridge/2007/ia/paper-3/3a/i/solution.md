<h1 id="3a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a regular differentiable curve $\mathbf x(t)$, its speed is $ds/dt=|\mathbf x'(t)|>0$, where $s$ is [arc length](../../../../../../arc-length.md). The oriented [unit tangent vector](../../../../../../unit-tangent-vector.md) is $\widehat{\mathbf T}=\mathbf x'/|\mathbf x'|$. The [curvature of a space curve](../../../../../../curvature-of-a-space-curve.md) is $\kappa=|d\widehat{\mathbf T}/ds|$. Equivalently, for a twice differentiable regular curve,

$$
\kappa=\frac{|\mathbf x'\times\mathbf x''|}{|\mathbf x'|^3}.
$$

For the [helix](../../../../../../helix.md), differentiation gives $\mathbf x'=(-a\sin t,a\cos t,b)$ and speed $v=\sqrt{a^2+b^2}$. Consequently

$$
\boxed{\widehat{\mathbf T}(t)=\frac{(-a\sin t,a\cos t,b)}{\sqrt{a^2+b^2}},\qquad\kappa=\frac{|a|}{a^2+b^2}.}
$$

Indeed $d\widehat{\mathbf T}/dt=(-a\cos t,-a\sin t,0)/v$ has magnitude $|a|/v$, and division by $ds/dt=v$ gives the result. This requires $(a,b)\ne(0,0)$; the excluded constant curve has no well-defined [unit tangent vector](../../../../../../unit-tangent-vector.md). For $a=0,b\ne0$ the curve is a straight line with zero [curvature of a space curve](../../../../../../curvature-of-a-space-curve.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3A](../../3a.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
