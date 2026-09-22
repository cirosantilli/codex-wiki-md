<h1 id="5b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The first coordinate of the [vector triple product](../../../../../../vector-triple-product.md) is

$$
[a\times(b\times c)]_1=a_2(b_1c_2-b_2c_1)-a_3(b_3c_1-b_1c_3)
=b_1(a\cdot c)-c_1(a\cdot b).
$$

The other two coordinates follow by cyclically permuting the indices, proving the identity.

A point on the line has the form $r=b+s m$. Substituting in the [plane](../../../../../../plane.md) equation gives $s(m\cdot n)=(a-b)\cdot n$. When $m\cdot n\ne0$ the parameter, and therefore the intersection point, is unique. The [vector triple product](../../../../../../vector-triple-product.md) gives $n\times(b\times m)=(n\cdot m)b-(n\cdot b)m$, so **the unique intersection is**

$$
\boxed{r=b+\frac{(a-b)\cdot n}{m\cdot n}m
=\frac{(a\cdot n)m+n\times(b\times m)}{m\cdot n}.}
$$

For the parallel case $m\cdot n=0$, the line is entirely in the [plane](../../../../../../plane.md) if $(b-a)\cdot n=0$, and otherwise has no intersection. As usual, a genuine line and [plane](../../../../../../plane.md) require nonzero direction and normal vectors. This is the [line-plane intersection criterion](../../../../../../line-plane-intersection-criterion.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5B](../../5b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
