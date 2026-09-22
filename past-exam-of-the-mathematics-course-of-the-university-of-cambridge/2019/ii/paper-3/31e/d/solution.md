<h1 id="31e/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

An interior [equilibrium point of a dynamical system](../../../../../../equilibrium-point-of-a-dynamical-system.md) must satisfy

$$
x-by=1,
\qquad
y-ax=1.
$$

If $ab\ne1$, the unique candidate is

$$
(x_*,y_*)=
\left(\frac{1+b}{1-ab},
\frac{1+a}{1-ab}\right).
$$

It belongs to $\Lambda$ precisely in either of the two cases

$$
a>-1, b>-1, ab<1,
\qquad\text{or}\qquad
a<-1, b<-1, ab>1.
$$

At this equilibrium the [Jacobian matrix](../../../../../../jacobian-matrix.md) has determinant

$$
\det DF(x_*,y_*)=r x_*y_*(1-ab).
$$

In the first region the equilibrium has [Poincaré index](../../../../../../poincare-index.md) $+1$, so index considerations alone do not rule out a periodic orbit. In the second region it is a [saddle equilibrium](../../../../../../saddle-equilibrium.md) of index $-1$. Everywhere else there is no interior equilibrium, except at $a=b=-1$, where the segment $x+y=1$ consists of equilibria.

Every simple closed curve in the convex set $\Lambda$ bounds a region contained in $\Lambda$. A periodic orbit has index $+1$, equal to the sum of the indices of the equilibria that it encloses. Thus a region with no equilibrium has total index zero, while the region with the single saddle has total index $-1$; both contradict the [index of a planar periodic orbit](../../../../../../index-of-a-planar-periodic-orbit.md). At $a=b=-1$, a periodic orbit cannot cross the equilibrium segment and must lie in one of its two complementary convex regions, where it encloses no equilibrium, giving the same contradiction. Therefore index considerations exclude periodic orbits except possibly when

$$
\boxed{a>-1,\qquad b>-1,\qquad ab<1.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [31E](../../31e.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
