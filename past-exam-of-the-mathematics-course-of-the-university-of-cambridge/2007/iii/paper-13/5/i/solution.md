<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the induced [square lattice](../../../../../../square-lattice.md) rectangle with lattice spacings as its side lengths. An open left-to-right crossing and a top-to-bottom crossing of closed dual bonds are mutually exclusive: their embedded paths must intersect, and a primal open bond cannot have its crossing dual bond closed. They are exhaustive. Indeed, explore all vertices connected to the left side by open paths. If that exploration does not reach the right side, the interface separating the explored set from the right side supplies a top-to-bottom path of closed dual bonds. This is the planar crossing alternative for [dual bond percolation](../../../../../../dual-bond-percolation.md).

For a primal rectangle of width $m$ and height $n$, the dual crossing can be represented using the dual columns at $1/2,3/2,\ldots,m-1/2$ and the exterior rows at $-1/2,n+1/2$. The terminal portions can be moved horizontally along the wired top and bottom boundary, so the random edges involved have exactly the law of a vertical crossing of a rectangle of width $m-1$ and height $n+1$. Consequently

$$
h_p(m,n)+h_{1-p}(n+1,m-1)=1.
$$

This is why the boundary offset is needed; one cannot simply assert that a finite square has crossing probability exactly one half. For $m=n+1$ and $p=1/2$, the second term is the same as the first after rotation and translation. Therefore

$$
\boxed{h_{1/2}(n+1,n)=1/2.}
$$

Shortening a rectangle can only help a horizontal crossing, so $h_{1/2}(n,n)\geq1/2$ as well.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5](../../5.md)
3. [Paper 13](../../../paper-13-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
