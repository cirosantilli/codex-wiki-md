<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

With $y=\dot x$, the feedback system is

$$
\dot x=y,\qquad \dot y=x^2-(q+x)y-z,\qquad
\dot z=y+p-z-z^3.
$$

For $p=0$, $(x,y,z)=(0,0,0)$ is an [equilibrium](../../../../../../equilibrium-point-of-a-dynamical-system.md). Its [stability matrix](../../../../../../stability-matrix.md) and characteristic polynomial are

$$
J=\begin{pmatrix}0&1&0\\0&-q&-1\\0&1&-1\end{pmatrix},\qquad
\det(rI-J)=r\bigl(r^2+(q+1)r+q+1\bigr).
$$

Thus **there is always a zero [eigenvalue](../../../../../../eigenvalue.md)**, with [eigenvector](../../../../../../eigenvector.md) $(1,0,0)$, so it is a [nonhyperbolic equilibrium](../../../../../../nonhyperbolic-equilibrium.md). If $q\ne-1$, the other two [eigenvalues](../../../../../../eigenvalue.md) are off the imaginary axis: for $q>-1$ their real parts are negative, while for $q<-1$ their product is negative. At $q=-1$, all three [eigenvalues](../../../../../../eigenvalue.md) are zero, explaining the exclusion in the next part.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 78](../../../paper-78-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
