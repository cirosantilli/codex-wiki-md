<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The displayed [orthogonal matrix](../../../../orthogonal-matrix.md) transforms the coordinates of a fixed [vector](../../../../vector.md), rather than actively moving that vector. Write $\theta=\arctan(1/2)$. Then $P=R(-\theta)$, so the new unit basis vectors, expressed in the old [orthonormal basis](../../../../orthonormal-basis.md), are the columns of $P^T$:

$$
\boxed{\mathbf e'_1=\frac{(2,1)}{\sqrt5},\qquad
\mathbf e'_2=\frac{(-1,2)}{\sqrt5}.}
$$

The axes have rotated counterclockwise through $\theta$, while the coordinate column transforms by the opposite rotation. For the example point $\mathbf r=(1,0)$, its new [coordinates](../../../../coordinate-linear-algebra.md) are $(2,-1)/\sqrt5$. Reconstruction gives $(2\mathbf e'_1-\mathbf e'_2)/\sqrt5=(1,0)$, confirming that the point is unchanged. The middle panel of the figure in part [1](../../1.md) shows these axes and the signed projections. Since $P^TP=I$ and $\det P=1$, lengths and orientation of the basis are preserved.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [5](../../5.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the mathematical methods I course of the University of Oxford](../../../split.md)
5. [Mathematical methods I course of the University of Oxford](../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
