<h1 id="2c/solution">Solution</h1>

↑ **Parent:** [2C](../2c.md)

A counterclockwise planar [rotation matrix](../../../../../rotation-matrix.md) has the form

$$
R_\theta=
\begin{pmatrix}
\cos\theta&-\sin\theta\\
\sin\theta&\cos\theta
\end{pmatrix},
\qquad\theta\in\mathbb R.
$$

To recover this form from preservation of the [Euclidean norm](../../../../../euclidean-norm.md), let $\mathbf u,\mathbf v$ be the columns of $R$. Applying the norm condition to the two coordinate [unit vectors](../../../../../unit-vector.md) gives $|\mathbf u|=|\mathbf v|=1$. Applying it to their sum gives

$$
2=|\mathbf u+\mathbf v|^2
=|\mathbf u|^2+2\mathbf u\cdot\mathbf v+|\mathbf v|^2,
$$

so $\mathbf u\cdot\mathbf v=0$. The columns are an [orthonormal basis](../../../../../orthonormal-basis.md), and $R^TR=I$: $R$ is an [orthogonal matrix](../../../../../orthogonal-matrix.md).

Write $\mathbf u=(\cos\theta,\sin\theta)^T$. There are two perpendicular [unit vectors](../../../../../unit-vector.md) available for $\mathbf v$, namely $\pm(-\sin\theta,\cos\theta)^T$. The first gives [determinant](../../../../../determinant.md) $1$, the second $-1$. The positive determinant hypothesis selects the first. **A norm-preserving planar map with positive determinant is a rotation.**

For the commutation condition, write

$$
A=\begin{pmatrix}a&b\\c&d\end{pmatrix}.
$$

Direct [matrix multiplication](../../../../../matrix-multiplication.md) gives

$$
AJ=\begin{pmatrix}b&-a\\d&-c\end{pmatrix},
\qquad
JA=\begin{pmatrix}-c&-d\\a&b\end{pmatrix}.
$$

Equality forces $c=-b$ and $d=a$, so, with $u=a$ and $v=-b$,

$$
A=\begin{pmatrix}u&-v\\v&u\end{pmatrix}=uI+vJ.
$$

If $u=v=0$, take $\lambda=0$ and $R=I$. Otherwise set $\lambda=\sqrt{u^2+v^2}>0$ and choose $\cos\theta=u/\lambda$, $\sin\theta=v/\lambda$. Then

$$
\boxed{A=\lambda R_\theta,\qquad\lambda=\sqrt{u^2+v^2}.}
$$

This describes the [centralizer of a planar quarter-turn](../../../../../centralizer-of-a-planar-quarter-turn.md). Its nonzero elements act as a rotation followed by a uniform scaling, just as multiplication by a nonzero [complex number](../../../../../complex-number.md) does.

## ↑ Ancestors (10)

1. [2C](../2c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
