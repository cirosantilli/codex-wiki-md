<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Choose the [holomorphic square root](../../../../../../holomorphic-square-root.md) in the [complex upper half-plane](../../../../../../upper-half-plane-complex-analysis.md) whose boundary value is positive on $0<x<1$. Its primitive has [derivative](../../../../../../derivative.md) $F_1'(z)=1/\sqrt{z(1-z^2)}$. The integral from the boundary basepoint zero is well-defined by a limiting path: the local singularity is only $z^{-1/2}$.

The three finite [prevertices](../../../../../../prevertex-of-a-schwarz-christoffel-map.md) $-1,0,1$ have [derivative](../../../../../../derivative.md) exponent $-1/2$, hence image angle $\pi/2$. At infinity $F_1'(z)=O(z^{-3/2})$, so the local coordinate $1/z$ also gives image angle $\pi/2$. These are the four corners of a [Schwarz-Christoffel mapping](../../../../../../schwarz-christoffel-mapping.md) to a [rectangle](../../../../../../rectangle.md). To establish that it is a [square](../../../../../../square.md) rather than a general [rectangle](../../../../../../rectangle.md), put

$$
A=\int_0^1\frac{dx}{\sqrt{x(1-x^2)}}.
$$

The length along $(-1,0)$ is also $A$ by $x\mapsto-x$. The length along $(1,\infty)$ is

$$
\int_1^\infty\frac{dx}{\sqrt{x(x^2-1)}}=A,
$$

by $x=1/t$, and the fourth side has the same length by [symmetry](../../../../../../symmetry-physics.md). With the chosen branch, the boundary [derivatives](../../../../../../derivative.md) on the intervals $(-\infty,-1),(-1,0),(0,1),(1,\infty)$ have phases $-1,-i,1,i$, respectively. Therefore

$$
F_1(-1)=iA,\quad F_1(0)=0,\quad F_1(1)=A,\quad F_1(\infty)=A+iA.
$$

The extended real boundary maps continuously and once around this [square](../../../../../../square.md). Each side is traversed monotonically, and the four corner limits are finite. The [argument principle](../../../../../../argument-principle.md), applied after small indentations around the boundary singularities, counts one inverse image of each interior value and zero of each exterior value. Since $F_1'$ never vanishes in the [complex upper half-plane](../../../../../../upper-half-plane-complex-analysis.md), those interior inverse images are simple. Thus

$$
\boxed{F_1:\mathbb H\longrightarrow\{u+iv:0<u<A,\ 0<v<A\}\text{ is conformal and bijective}.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
