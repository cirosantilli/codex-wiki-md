<h1 id="11/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Multiplication by each column of $B$ gives

$$
AB=B\operatorname{diag}(-1,2,1).
$$

Since $B$ is invertible, its columns are an [eigenbasis](../../../../eigenbasis.md) and the [similarity transformation](../../../../similarity-transformation.md) gives

$$
\boxed{D=B^{-1}AB=\operatorname{diag}(-1,2,1),\qquad(d_1,d_2,d_3)=(-1,2,1).}
$$

There is an important source variant: the alternative scanned copy supplies an erroneous inverse with an extra factor $1/6$ and a different top-right entry. Calling that supplied matrix $C$, direct multiplication gives $(CB)_{22}=1/6$, so it cannot be $B^{-1}$. Inverting $B$ instead gives

$$
B^{-1}=\begin{pmatrix}-1&-2&2\\-2&2&2\\3&0&-3\end{pmatrix}.
$$

This is the inverse in the cleaner copy used here. Using the scanned erroneous matrix would make $CAB$ nondiagonal, so correcting the inverse is necessary before applying the stated diagonalization. The [inverse-matrix verification test](../../../../inverse-matrix-verification-test.md) catches the error without assuming the claimed outcome.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [11](../../11.md)
3. [2015 resit](../../../2015-resit-split.md)
4. [Past exam of the mathematical methods I course of the University of Oxford](../../../split.md)
5. [Mathematical methods I course of the University of Oxford](../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
