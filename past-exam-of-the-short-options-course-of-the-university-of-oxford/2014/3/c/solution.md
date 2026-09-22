<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use part (a) to put the four [projective points](../../../../projective-point.md) at

$$
[1:0:0],\quad[0:1:0],\quad[0:0:1],\quad[1:1:1].
$$

A [quadratic polynomial](../../../../quadratic-polynomial.md) vanishing at the first three has no square terms, and vanishing at the fourth gives

$$
q=Axy+Bxz+Cyz,\qquad A+B+C=0.
$$

These form a two-dimensional [vector space](../../../../vector-space-split.md). Choose the two members

$$
q_0=xy+xz-2yz,\qquad q_1=xy-2xz+yz.
$$

Their coefficient triples are independent and both satisfy the relation. Their symmetric [bilinear form](../../../../bilinear-form-split.md) matrices are of the form

$$
B(A,B,C)=\frac12\begin{pmatrix}0&A&B\\A&0&C\\B&C&0\end{pmatrix},\qquad
\det B(A,B,C)=\frac{ABC}{4}.
$$

For $(A,B,C)=(1,1,-2)$ and $(1,-2,1)$, both determinants are $-1/2$, so both selected conics are nonsingular. Any coefficient triple with zero sum is uniquely a [linear combination](../../../../linear-combination.md) of these two. Hence every conic through the four points has matrix

$$
\boxed{\lambda B_0+\mu B_1,\qquad(\lambda,\mu)\ne(0,0).}
$$

Undoing the [projective transformation](../../../../projective-linear-transformation.md) carries the entire family back to the original four points, preserving nonsingularity. This is a [pencil of conics through four points](../../../../pencil-of-conics-through-four-points.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2014](../../../2014-split.md)
4. [Past exam of the short options course of the University of Oxford](../../../split.md)
5. [Short options course of the University of Oxford](../../../../short-options-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
