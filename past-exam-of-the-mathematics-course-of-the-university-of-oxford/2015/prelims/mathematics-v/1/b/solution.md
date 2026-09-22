<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $r=\sqrt{x^2+y^2}>0$. The [cylindrical coordinates](../../../../../../cylindrical-coordinate-system.md) give $\mathbf e_\theta=(-y/r,x/r,0)$ and $\mathbf e_r=(x/r,y/r,0)$, so the [vector components](../../../../../../coordinate-linear-algebra.md) of the [vector field](../../../../../../vector-field.md) are

$$
F_x=-\frac{yf(z)}r,\qquad F_y=\frac{xf(z)}r,\qquad F_z=0.
$$

The first two components of the [curl](../../../../../../curl.md), calculated in [Cartesian coordinates](../../../../../../cartesian-coordinate-system.md), are $-xf'(z)/r$ and $-yf'(z)/r$. For the third component, the [chain rule](../../../../../../chain-rule.md) gives

$$
\partial_x(x/r)=\frac1r-\frac{x^2}{r^3},\qquad
\partial_y(y/r)=\frac1r-\frac{y^2}{r^3},
$$

and hence

$$
(\nabla\times\mathbf F)_z=f(z)\left(\frac2r-\frac{x^2+y^2}{r^3}\right)=\frac{f(z)}r.
$$

Combining these [vector components](../../../../../../coordinate-linear-algebra.md) in the [cylindrical basis](../../../../../../cylindrical-basis.md) yields

$$
\boxed{\nabla\times\mathbf F=\frac{f(z)}r\mathbf e_z-f'(z)\mathbf e_r,\qquad r>0.}
$$

The restriction $r>0$ matters because the [cylindrical basis](../../../../../../cylindrical-basis.md) is undefined on the axis.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [Mathematics V](../../../mathematics-v-split.md)
4. [Prelims](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
