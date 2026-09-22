<h1 id="3b/solution">Solution</h1>

↑ **Parent:** [3B](../3b.md)

The boundary ray has $y/x=3/5$, and its intersection with the [hyperbola](../../../../../hyperbola.md) is $(5/4,3/4)$. Under the given [change of variables](../../../../../change-of-variables-formula.md), $x^2-y^2=r^2$ and $y/x=\tanh\theta$. Thus the region becomes

$$
0\leq r\leq1,\qquad 0\leq\theta\leq\operatorname{artanh}(3/5)=\log2.
$$

The [hyperbolic functions](../../../../../hyperbolic-function.md) satisfy $\cosh^2\theta-\sinh^2\theta=1$, so the [Jacobian determinant](../../../../../jacobian-determinant.md) is

$$
\det\frac{\partial(x,y)}{\partial(r,\theta)}
=\det\begin{pmatrix}\cosh\theta&r\sinh\theta\\\sinh\theta&r\cosh\theta\end{pmatrix}=r.
$$

It is positive in the interior. The coordinate degeneracy at $r=0$ is a boundary set of area zero and does not affect the [change of variables formula](../../../../../change-of-variables-formula.md). Therefore

$$
\int_A y\,dx\,dy
=\int_0^{\log2}\int_0^1 r^2\sinh\theta\,dr\,d\theta
=\frac13(\cosh(\log2)-1)
=\boxed{\frac1{12}}.
$$

Here $\cosh(\log2)=5/4$. The PDF specifies two line segments and one hyperbolic arc; the duplicated $y=0$ line in the TeX is not an extra boundary condition.

## ↑ Ancestors (10)

1. [3B](../3b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
