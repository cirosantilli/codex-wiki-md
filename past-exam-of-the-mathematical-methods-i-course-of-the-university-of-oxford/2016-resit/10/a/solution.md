<h1 id="10/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The vector $(0,1,-1)$ is an [eigenvector](../../../../eigenvector.md) with [eigenvalue](../../../../eigenvalue.md) one. The other two orthogonal directions give eigenvalues two and five, leading to

$$
\boxed{V=\begin{pmatrix}
0&1/\sqrt3&2/\sqrt6\\
1/\sqrt2&1/\sqrt3&-1/\sqrt6\\
-1/\sqrt2&1/\sqrt3&-1/\sqrt6
\end{pmatrix},\qquad D=\operatorname{diag}(1,2,5).}
$$

Its columns are an [orthonormal eigenbasis](../../../../orthonormal-eigenbasis.md), so $V^{\mathsf T}V=I$ and $V^{\mathsf T}AV=D$. Multiplying by $V$ and $V^{\mathsf T}$ gives $\boxed{A=VDV^{\mathsf T}}$. Eigenvector signs and the joint order of columns and diagonal entries may be changed consistently.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [10](../../10.md)
3. [2016 resit](../../../2016-resit-split.md)
4. [Past exam of the mathematical methods I course of the University of Oxford](../../../split.md)
5. [Mathematical methods I course of the University of Oxford](../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
