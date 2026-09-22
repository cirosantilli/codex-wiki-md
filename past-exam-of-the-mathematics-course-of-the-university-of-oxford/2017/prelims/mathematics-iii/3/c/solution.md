<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $F=x+y+z^2$ and $g=x^2+y^2+z^2$. The [unit sphere](../../../../../../unit-sphere.md) is [compact](../../../../../../compact-space.md), so the [continuous function](../../../../../../continuous-function.md) $F$ has a [global maximum](../../../../../../global-maximum.md) and [global minimum](../../../../../../global-minimum.md). Since $\nabla g\ne0$ on the [unit sphere](../../../../../../unit-sphere.md), all such points satisfy the [Lagrange multiplier](../../../../../../lagrange-multiplier.md) equations

$$
1=2\lambda x,\qquad1=2\lambda y,\qquad2z=2\lambda z,\qquad x^2+y^2+z^2=1.
$$

Thus $x=y$ and either $z=0$ or $\lambda=1$.

If $z=0$, then $x=y=\pm1/\sqrt2$, giving $F=\pm\sqrt2$. If $\lambda=1$, then $x=y=1/2$ and $z=\pm1/\sqrt2$, giving $F=3/2$. These exhaust the candidates, so

$$
\boxed{\min F=-\sqrt2\text{ at }(-1/\sqrt2,-1/\sqrt2,0),\qquad
\max F=\frac32\text{ at }(1/2,1/2,\pm1/\sqrt2).}
$$

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
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
