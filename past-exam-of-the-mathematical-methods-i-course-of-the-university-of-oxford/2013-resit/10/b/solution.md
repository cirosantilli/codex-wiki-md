<h1 id="10/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The first operation acts nearest the column vector, so the composite [rotation matrix](../../../../rotation-matrix.md) is $M=R_z(\alpha)R_x(\beta)$:

$$
\boxed{M=\begin{pmatrix}
\cos\alpha&-\sin\alpha\cos\beta&\sin\alpha\sin\beta\\
\sin\alpha&\cos\alpha\cos\beta&-\cos\alpha\sin\beta\\
0&\sin\beta&\cos\beta
\end{pmatrix}.}
$$

At $\alpha=\beta=\pi/2$ this reduces to

$$
M=\begin{pmatrix}0&0&1\\1&0&0\\0&1&0\end{pmatrix},\qquad
(x,y,z)\mapsto(z,x,y).
$$

Solving $M\mathbf v=\mathbf v$ gives $v_x=v_y=v_z$. Normalization yields the fixed-axis [unit vectors](../../../../unit-vector.md)

$$
\boxed{\mathbf v=\pm\frac1{\sqrt3}(1,1,1).}
$$

Both signs describe the same unoriented axis. The operation is a cyclic permutation, and $M^3=I$; it is not generally obtained by reversing the multiplication order.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [10](../../10.md)
3. [2013 resit](../../../2013-resit-split.md)
4. [Past exam of the mathematical methods I course of the University of Oxford](../../../split.md)
5. [Mathematical methods I course of the University of Oxford](../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
