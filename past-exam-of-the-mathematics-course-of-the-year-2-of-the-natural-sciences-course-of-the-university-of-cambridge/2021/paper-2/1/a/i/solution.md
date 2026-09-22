<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Two [integrations by parts](../../../../../../integration-by-parts.md) give the boundary form of the [Sturm-Liouville operator](../../../../../../sturm-liouville-operator.md):

$$
\langle f,Lg\rangle-\langle Lf,g\rangle=\left[p\left(f'^*g-f^*g'\right)\right]_a^b.
$$

The interior terms cancel because $p,q$ are real. Thus the required endpoint condition is

$$
\boxed{\left[p(f'^*g-f^*g')\right]_a^b=0\quad\text{for every }f,g\text{ in the operator domain}.}
$$

For a regular interval, a standard [self-adjoint](../../../../../../self-adjoint-operator.md) domain is specified by one real homogeneous [Robin boundary condition](../../../../../../robin-boundary-condition.md) at each endpoint:

$$
A_a y(a)+B_a p(a)y'(a)=0,\qquad A_b y(b)+B_b p(b)y'(b)=0,
$$

where neither pair of real constants is identically zero. At each end, these conditions force the two boundary data vectors of $f,g$ to be proportional, making the displayed form zero. [Dirichlet boundary conditions](../../../../../../dirichlet-boundary-condition.md) and [Neumann boundary conditions](../../../../../../neumann-boundary-condition.md) are the cases $B=0$ and $A=0$. Coupled conditions also work, for example $y(a)=y(b)$ and $p(a)y'(a)=p(b)y'(b)$, whose two endpoint contributions cancel. Self-adjointness uses the maximal common domain with these conditions, not an arbitrary smaller symmetric restriction.

The [weighted inner product](../../../../../../weighted-inner-product.md) must be nondegenerate. The usual interpretation is $w>0$ almost everywhere, allowing isolated endpoint zeros as in part (b), with the operator defined on its appropriate weighted domain. Merely allowing a weight that is zero on an entire interval would not by itself define the stated operator or a positive-definite [inner product](../../../../../../inner-product-split.md) on ordinary functions.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
