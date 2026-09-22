<h1 id="9/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Label $\mathbf a$ opposite $\mathbf x_0$, $\mathbf b$ opposite $\mathbf x_1$, $\mathbf c$ opposite $\mathbf x_2$ and $\mathbf d$ opposite $\mathbf x_3$. Since the [tetrahedron](../../../../tetrahedron.md) is nondegenerate, its [scalar triple product](../../../../scalar-triple-product.md) $T=\mathbf u_1\cdot(\mathbf u_2\times\mathbf u_3)$ is nonzero. Put $s=T/|T|$ to handle either [orientation of a vector space](../../../../orientation-of-a-vector-space.md). Then the required outward [vectors](../../../../vector.md) are

$$
\boxed{\begin{aligned}
\mathbf a&=s(\mathbf u_2-\mathbf u_1)\times(\mathbf u_3-\mathbf u_1),\\
\mathbf b&=-s\,\mathbf u_2\times\mathbf u_3,\\
\mathbf c&=-s\,\mathbf u_3\times\mathbf u_1,\\
\mathbf d&=-s\,\mathbf u_1\times\mathbf u_2.
\end{aligned}}
$$

Each [cross product](../../../../cross-product.md) has magnitude twice the area of its triangular face. The signs are fixed geometrically: $\mathbf b\cdot\mathbf u_1=-|T|<0$, so $\mathbf b$ points away from the opposite vertex; the same test with $\mathbf u_2$ and $\mathbf u_3$ handles $\mathbf c$ and $\mathbf d$. For the remaining face, the displacement toward its opposite vertex is $-\mathbf u_1$, and $\mathbf a\cdot(-\mathbf u_1)=-|T|<0$, again outward.

Expand the first [cross product](../../../../cross-product.md):

$$
\mathbf a=s(\mathbf u_2\times\mathbf u_3+\mathbf u_3\times\mathbf u_1+\mathbf u_1\times\mathbf u_2)
=-\mathbf b-\mathbf c-\mathbf d.
$$

Therefore

$$
\boxed{\mathbf a+\mathbf b+\mathbf c+\mathbf d=\mathbf0.}
$$

This is [closure of outward face area vectors](../../../../closure-of-outward-face-area-vectors.md), with every face area multiplied by the same factor two. Omitting $s$ would orient all four faces inward when $T<0$.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [9](../../9.md)
3. [2021 resit](../../../2021-resit-split.md)
4. [Past exam of the mathematical methods I course of the University of Oxford](../../../split.md)
5. [Mathematical methods I course of the University of Oxford](../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
