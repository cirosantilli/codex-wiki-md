<h1 id="14f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Consider the filled [hyperbolic triangle](../../../../../../hyperbolic-triangle.md) with vertices $A,B,C$. Every point $P$ is on some [geodesic segment](../../../../../../geodesic-segment.md) $Aw$ with $w\in BC$: for instance, in the [Beltrami-Klein model](../../../../../../beltrami-klein-model.md) these are the ordinary straight segments filling a convex triangle. For any other point $Q$ of the triangle, apply part (b) first on $Aw$ and then on $BC$:

$$
d(Q,P)\le\max\{d(Q,A),d(Q,w)\}
\le\max\{d(Q,A),d(Q,B),d(Q,C)\}.
$$

Applying the same argument to $Q$, with each vertex held fixed, bounds every term on the right by the maximum of the three side lengths. The endpoints of a longest side attain that bound. Thus **the [diameter](../../../../../../diameter.md) is exactly the longest side length**:

$$
\boxed{\operatorname{diam}(ABC)=\max\{d(A,B),d(B,C),d(C,A)\}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [14F](../../14f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
