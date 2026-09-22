<h1 id="3/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Choose the following consistent sign convention. The [Givens rotation](../../../../../givens-rotation.md) $J(i,j,\theta)$ equals the [identity matrix](../../../../../identity-matrix.md) except for the block on coordinates $i,j$:

$$
J\big|_{i,j}=\begin{pmatrix}\cos\theta&\sin\theta\\-\sin\theta&\cos\theta\end{pmatrix}.
$$

Thus it changes only the $i$th and $j$th coordinates of a [vector](../../../../../vector.md). Write $c=\cos\theta$, $s=\sin\theta$. Its two-coordinate block satisfies

$$
\begin{pmatrix}c&-s\\s&c\end{pmatrix}
\begin{pmatrix}c&s\\-s&c\end{pmatrix}
=\begin{pmatrix}c^2+s^2&0\\0&c^2+s^2\end{pmatrix}=I_2.
$$

All remaining coordinates are unchanged, so $J^TJ=I_n$. Hence **every such [Givens rotation](../../../../../givens-rotation.md) is an [orthogonal matrix](../../../../../orthogonal-matrix.md)**. With this convention the two-coordinate [rotation matrix](../../../../../rotation-matrix.md) rotates through angle $-\theta$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the numerical analysis course of the University of Oxford](../../../../split.md)
6. [Numerical analysis course of the University of Oxford](../../../../../numerical-analysis-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
