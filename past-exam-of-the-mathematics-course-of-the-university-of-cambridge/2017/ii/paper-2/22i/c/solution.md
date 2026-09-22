<h1 id="22i/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Homogenization gives $F=X^4+X^2Y^2+Y^2Z^2+Z^4$, with

$$
F_X=4X^3+2XY^2,\qquad F_Y=2Y(X^2+Z^2),\qquad F_Z=2ZY^2+4Z^3.
$$

If the characteristic is not $2$, a singular point with $Y=0$ would force $X=Z=0$, impossible. If $Y\ne0$, then $X^2+Z^2=0$. If either $X$ or $Z$ vanishes, both vanish, giving $[0:1:0]$. Otherwise the other two [derivative](../../../../../../derivative.md) equations require $Y^2=-2X^2=-2Z^2$, whence $X^2=Z^2$ and $2X^2=0$, again impossible. Thus

$$
\boxed{\operatorname{Sing}(X)=\{[0:1:0]\}\quad(\operatorname{char}k\ne2).}
$$

In the chart $Y=1$, the quadratic term is $X^2+Z^2$, the product of two distinct linear factors over $k$, so this is an [ordinary double point](../../../../../../ordinary-double-point.md).

In characteristic $2$,

$$
\boxed{F=(X^2+XY+YZ+Z^2)^2=((X+Z)(X+Y+Z))^2.}
$$

All first [derivatives](../../../../../../derivative.md) of this equation vanish. The equation defines a [nonreduced scheme](../../../../../../nonreduced-scheme.md), singular everywhere; it no longer satisfies the irreducible/reduced hypersurface premise. If “curve” means the associated reduced variety, it is the union of two distinct lines, and only their intersection $\boxed{[1:0:1]}$ is singular. These two interpretations must not be conflated.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [22I](../../22i.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
