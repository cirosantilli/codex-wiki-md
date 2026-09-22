<h1 id="8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

The second coordinate is already an [eigenvector](../../../eigenvector.md) with [eigenvalue](../../../eigenvalue.md) $-2$. On the first and third coordinates the [characteristic polynomial](../../../characteristic-polynomial.md) is

$$
\det\begin{pmatrix}2-\lambda&2\\2&-1-\lambda\end{pmatrix}
=\lambda^2-\lambda-6=(\lambda-3)(\lambda+2).
$$

Thus the full [eigenvalues](../../../eigenvalue.md) are $3,-2,-2$. A corresponding [orthonormal eigenbasis](../../../orthonormal-eigenbasis.md) is

$$
\boxed{\begin{array}{c|c}
\lambda=3 & \mathbf v_3=(2,0,1)/\sqrt5\\
\lambda=-2 & \mathbf v_{-2}=(1,0,-2)/\sqrt5,\quad\mathbf e_2=(0,1,0).
\end{array}}
$$

Their pairwise dot products vanish and each has norm one. Substitution checks $A\mathbf v_3=3\mathbf v_3$ and $A\mathbf v_{-2}=-2\mathbf v_{-2}$. The two-dimensional repeated [eigenspace](../../../eigenspace.md) permits any orthonormal pair spanning the same plane; the displayed choice is convenient because it separates the second coordinate.

## ↑ Ancestors (11)

1. [8](../8.md)
2. [2013](../../2013-split.md)
3. [Past exam of the mathematical methods I course of the University of Oxford](../../split.md)
4. [Mathematical methods I course of the University of Oxford](../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
