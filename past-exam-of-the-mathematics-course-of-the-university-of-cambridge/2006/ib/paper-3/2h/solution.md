<h1 id="2h/solution">Solution</h1>

↑ **Parent:** [2H](../2h.md)

Parametrize the surface by $r(x,y)=(x,y,xy)$. Its tangent vectors are $r_x=(1,0,y)$ and $r_y=(0,1,x)$. Choose the upward [unit normal](../../../../../unit-normal.md)

$$
N=\frac{(-y,-x,1)}{\sqrt{1+x^2+y^2}}.
$$

The [first fundamental form](../../../../../first-fundamental-form.md) coefficients are

$$
E=1+y^2,\qquad F=xy,\qquad G=1+x^2,
\qquad EG-F^2=1+x^2+y^2.
$$

Since $r_{xx}=r_{yy}=0$ and $r_{xy}=(0,0,1)$, the [second fundamental form](../../../../../second-fundamental-form-split.md) coefficients are $e=g=0$ and $f=(1+x^2+y^2)^{-1/2}$. The determinant of the [shape operator](../../../../../shape-operator.md) gives the [Gaussian curvature](../../../../../gaussian-curvature.md):

$$
\boxed{K=\frac{eg-f^2}{EG-F^2}=-\frac1{(1+x^2+y^2)^2}.}
$$

Changing the normal's sign changes both second-form factors and leaves this determinant unchanged. Although the question calls the surface a hyperboloid, $z=xy$ is a [hyperbolic paraboloid](../../../../../hyperbolic-paraboloid.md); the calculation uses the stated surface equation.

## ↑ Ancestors (10)

1. [2H](../2h.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
