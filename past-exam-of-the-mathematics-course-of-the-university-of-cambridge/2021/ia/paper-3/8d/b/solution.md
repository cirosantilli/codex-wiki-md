<h1 id="8d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

If $Q\in O(2)$, then $Q^TQ=I$, so

$$
(\det Q)^2=1
$$

and $\det Q=\pm1$. If $\det Q=1$, its first column is $(\cos\theta,\sin\theta)^T$ for some $\theta$, and orthonormality plus positive orientation force

$$
Q=
\begin{pmatrix}
\cos\theta&-\sin\theta\\
\sin\theta&\cos\theta
\end{pmatrix}.
$$

Thus every element of $SO(2)$ is a rotation.

Let $J=\operatorname{diag}(1,-1)$. If $\det Q=-1$, then $QJ\in SO(2)$ and $Q=(QJ)J\in SO(2)J$. Conversely every matrix in $SO(2)J$ has determinant $-1$. Therefore the union is disjoint and

$$
\boxed{O(2)=SO(2)\sqcup SO(2)J}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [8D](../../8d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
