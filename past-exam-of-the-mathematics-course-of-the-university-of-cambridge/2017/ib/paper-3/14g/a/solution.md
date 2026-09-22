<h1 id="14g/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

At a regular point, choose the unit normal $\mathbf n=(\sigma_x\times\sigma_y)/|\sigma_x\times\sigma_y|$. The [first fundamental form](../../../../../../first-fundamental-form.md) is the induced squared length

$$
I=E\,dx^2+2F\,dx\,dy+G\,dy^2,\quad E=\sigma_x\cdot\sigma_x,\ F=\sigma_x\cdot\sigma_y,\ G=\sigma_y\cdot\sigma_y.
$$

The [second fundamental form](../../../../../../second-fundamental-form-split.md) is

$$
II=e\,dx^2+2f\,dx\,dy+g\,dy^2,\quad e=\mathbf n\cdot\sigma_{xx},\ f=\mathbf n\cdot\sigma_{xy},\ g=\mathbf n\cdot\sigma_{yy}.
$$

The [Gaussian curvature](../../../../../../gaussian-curvature.md) is the determinant of the [shape operator](../../../../../../shape-operator.md), $K=(eg-f^2)/(EG-F^2)$, independent of the normal orientation.

For the given graph, $\sigma_x=(1,0,y)$ and $\sigma_y=(0,1,x)$, so with $S=1+x^2+y^2$,

$$
I=(1+y^2)\,dx^2+2xy\,dx\,dy+(1+x^2)\,dy^2,\qquad
\mathbf n=\frac{(-y,-x,1)}{\sqrt S},\qquad II=\frac{2\,dx\,dy}{\sqrt S}.
$$

Therefore

$$
\boxed{K(x,y)=-\frac1{(1+x^2+y^2)^2}.}
$$

The surface is regular everywhere. The printed description “hyperboloid” is a naming error: this graph is a [hyperbolic paraboloid](../../../../../../hyperbolic-paraboloid.md), and the computation uses the actual parametrization.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [14G](../../14g.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
