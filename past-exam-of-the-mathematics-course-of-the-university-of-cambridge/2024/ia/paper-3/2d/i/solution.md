<h1 id="2d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [special orthogonal group](../../../../../../special-orthogonal-group.md) is

$$
SO(n)=\{A\in M_n(\mathbb R):A^TA=I,\ \det A=1\}.
$$

If

$$
A=\begin{pmatrix}a&b\\c&d\end{pmatrix}\in SO(2),
$$

its first column is a unit [vector](../../../../../../vector.md), say $(\cos\theta,\sin\theta)^T$. The second column is the unique unit [vector](../../../../../../vector.md) perpendicular to it that gives positive [determinant](../../../../../../determinant.md), namely $(-\sin\theta,\cos\theta)^T$. Thus

$$
A=\begin{pmatrix}
\cos\theta&-\sin\theta\\
\sin\theta&\cos\theta
\end{pmatrix},
$$

so $A$ is rotation through $\theta$ about the origin.

For $A\in SO(3)$, its real characteristic [polynomial](../../../../../../polynomial-split.md) of odd degree has a real [eigenvalue](../../../../../../eigenvalue.md). Every [eigenvalue](../../../../../../eigenvalue.md) of an orthogonal [matrix](../../../../../../matrix.md) has [modulus](../../../../../../modulus.md) one, so every real [eigenvalue](../../../../../../eigenvalue.md) is $\pm1$. Nonreal [eigenvalues](../../../../../../eigenvalue.md) occur in conjugate pairs whose product is one, while $\det A=1$; if all [eigenvalues](../../../../../../eigenvalue.md) are real, their product likewise forces at least one to be $+1$. Hence $A$ fixes a nonzero [vector](../../../../../../vector.md) $u$. The plane $u^\perp$ is $A$-invariant, and the restriction to it is an orientation-preserving orthogonal map. By the $SO(2)$ result it is a planar rotation. Therefore $A$ is a rotation about the axis $\mathbb Ru$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2D](../../2d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
