<h1 id="37a/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let the sphere have radius $a$; set $a=1$ for the unit sphere implicit in the question. Since

$$
\boldsymbol\Phi=\frac{\alpha\mathbf U}{r},
\qquad
\chi=\beta\mathbf U\mathbin{\cdot}\nabla\frac1r
=-\beta\frac{\mathbf U\mathbin{\cdot}\mathbf x}{r^3},
$$

one finds

$$
\mathbf u
=\left(-\frac\alpha r-\frac\beta{r^3}\right)\mathbf U
+\left(-\frac\alpha{r^3}+\frac{3\beta}{r^5}\right)
(\mathbf U\mathbin{\cdot}\mathbf x)\mathbf x.
$$

On $r=a$, the [no-slip boundary condition](../../../../../../no-slip-boundary-condition.md) requires $\mathbf u=\mathbf U$ for every surface normal. The coefficient of  
$(\mathbf U\mathbin{\cdot}\mathbf n)\mathbf n$ must vanish, while the coefficient of $\mathbf U$ must equal one:

$$
-\frac\alpha a+\frac{3\beta}{a^3}=0,
\qquad
-\frac\alpha a-\frac\beta{a^3}=1.
$$

Solving,

$$
\boxed{\alpha=-\frac{3a}{4},\qquad
\beta=-\frac{a^3}{4}.}
$$

For a unit sphere,

$$
\boxed{\alpha=-\frac34,\qquad\beta=-\frac14.}
$$

Substitution reproduces the standard [translating sphere in Stokes flow](../../../../../../translating-sphere-in-stokes-flow.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [37A](../../37a.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
