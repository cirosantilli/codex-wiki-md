<h1 id="2d/solution">Solution</h1>

↑ **Parent:** [2D](../2d.md)

The [orthogonal group](../../../../../orthogonal-group.md) is

$$
O(n)=\{Q\in M_n(\mathbb R):Q^TQ=I\}.
$$

The [special orthogonal group](../../../../../special-orthogonal-group.md) is its determinant-one subgroup

$$
SO(n)=\{Q\in O(n):\det Q=1\}.
$$

Every [eigenvalue](../../../../../eigenvalue.md) of an [orthogonal matrix](../../../../../orthogonal-matrix.md) has [modulus](../../../../../modulus.md) one. A real three-by-three matrix has at least one real eigenvalue, and nonreal eigenvalues occur in a [complex conjugate](../../../../../complex-conjugate.md) pair. If $Q\in SO(3)$ has such a pair $e^{\pm i\theta}$, their product is one, so the remaining eigenvalue is $\det Q=1$. If all three eigenvalues are real, each is $\pm1$ and their product is one; an odd number of three signs with product one must include $+1$. Hence every element of $SO(3)$ has an eigenvector of eigenvalue one and represents a [rotation in three dimensions](../../../../../rotation-in-three-dimensions.md) about its span.

**It is false** that every element of $O(3)$ is either a rotation or a plane reflection. For example,

$$
Q=\begin{pmatrix}
\cos\theta&-\sin\theta&0\\
\sin\theta&\cos\theta&0\\
0&0&-1
\end{pmatrix},
\qquad 0<\theta<\pi,
$$

is an [improper orthogonal transformation](../../../../../improper-orthogonal-transformation.md) combining a rotation with a reflection. Its eigenvalues are $e^{\pm i\theta}$ and $-1$, whereas a plane reflection has eigenvalues $1,1,-1$ and a rotation has determinant one.

## ↑ Ancestors (10)

1. [2D](../2d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
