<h1 id="5c/solution">Solution</h1>

↑ **Parent:** [5C](../5c.md)

In the parametric description, $a$ is a point of the [straight line](../../../../../straight-line.md) and the nonzero [vector](../../../../../vector.md) $b$ gives its direction. The real parameter runs through every point of that line. For the [cross product](../../../../../cross-product.md) description, take another [cross product](../../../../../cross-product.md) with $c$ and use the [vector triple product identity](../../../../../vector-triple-product.md):

$$
c\times(x\times c)=|c|^2x-(c\cdot x)c=c\times d.
$$

Hence every solution has the representation

$$
\boxed{x=a+\lambda(x)b,\qquad
a=\frac{c\times d}{|c|^2},\qquad b=c,\qquad
\lambda(x)=\frac{c\cdot x}{|c|^2}.}
$$

Here $a\cdot b=0$ and $|b|=|c|$, as required. Conversely,

$$
(a+\lambda c)\times c
=\frac{(c\times d)\times c}{|c|^2}
=d-\frac{(c\cdot d)c}{|c|^2}=d.
$$

Thus the perpendicularity assumption is sufficient, and the solutions form a [straight line](../../../../../straight-line.md) parallel to $c$. When $d\ne0$, the [vector](../../../../../vector.md) $d$ is perpendicular both to $c$ and to every position [vector](../../../../../vector.md) on the line; it is the normal to the plane through the origin containing that line. The point $a=c\times d/|c|^2$ is the perpendicular foot from the origin. Its distance from the origin is $|d|/|c|$, since $c\cdot d=0$.

For a general parametric [straight line](../../../../../straight-line.md), minimize the squared [Euclidean distance](../../../../../euclidean-distance.md)

$$
|a+\lambda b-y|^2=|a-y|^2+2\lambda b\cdot(a-y)+\lambda^2|b|^2.
$$

This strictly convex [quadratic function](../../../../../quadratic-function.md) has its unique minimum at $\lambda=b\cdot(y-a)/|b|^2$, giving the [orthogonal projection](../../../../../orthogonal-projection.md)

$$
\boxed{x_{\rm nearest}=a+\frac{b\cdot(y-a)}{|b|^2}b.}
$$

For the [cross product](../../../../../cross-product.md) description, $a\cdot c=0$, so this becomes

$$
\boxed{x_{\rm nearest}=\frac{c\times d}{|c|^2}+\frac{c\cdot y}{|c|^2}c.}
$$

For the two planes, put $s=m\cdot n$ and $c=m\times n$. Nonparallel unit normals give $|s|<1$ and $|c|^2=1-s^2$. Seek the perpendicular foot in their span, $a=um+vn$. Its two [dot products](../../../../../dot-product.md) impose $u+sv=\mu$ and $su+v=\nu$. Solving gives both requested descriptions of the intersection:

$$
\boxed{x=\frac{(\mu-s\nu)m+(\nu-s\mu)n}{1-s^2}+\lambda(m\times n),\qquad\lambda\in\mathbb R,}
$$

and

$$
\boxed{x\times(m\times n)=\nu m-\mu n.}
$$

Indeed the [vector triple product identity](../../../../../vector-triple-product.md) gives $x\times(m\times n)=m(x\cdot n)-n(x\cdot m)$. Conversely, since $m,n$ are linearly independent, equality to $\nu m-\mu n$ forces both plane equations. Thus neither description introduces extra points.

## ↑ Ancestors (10)

1. [5C](../5c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
