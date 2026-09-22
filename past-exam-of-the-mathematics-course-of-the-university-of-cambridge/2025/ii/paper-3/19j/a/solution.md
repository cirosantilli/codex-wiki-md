<h1 id="19j/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write

$$
g=\begin{pmatrix}a&b\\-\bar b&\bar a\end{pmatrix}\in SU_2,
\qquad |a|^2+|b|^2=1.
$$

The [homogeneous polynomial representation of SU2](../../../../../../homogeneous-polynomial-representation-of-su2.md) is the symmetric-power action determined by

$$
g\cdot x=ax-\bar b y,\qquad
g\cdot y=bx+\bar a y,
$$

and extended multiplicatively to $V_n$.

In the ordered basis $(x^3,x^2y,xy^2,y^3)$, the matrix for $g$ is

$$
\begin{pmatrix}
a^3&a^2b&ab^2&b^3\\
-3a^2\bar b&a^2\bar a-2ab\bar b&2ab\bar a-b^2\bar b&3b^2\bar a\\
3a\bar b^2&b\bar b^2-2a\bar a\bar b&a\bar a^2-2b\bar a\bar b&3b\bar a^2\\
-\bar b^3&\bar a\bar b^2&-\bar b\bar a^2&\bar a^3
\end{pmatrix}.
$$

The character of a representation $(V,\rho)$ is $\chi_V(g)=\operatorname{tr}\rho(g)$. Every $g\in SU_2$ is conjugate to $\operatorname{diag}(z,z^{-1})$ with $|z|=1$, and hence the [character of the homogeneous polynomial representation of SU2](../../../../../../character-of-the-homogeneous-polynomial-representation-of-su2.md) is

$$
\chi_n(g)=z^n+z^{n-2}+\cdots+z^{-n}.
$$

For $z=e^{i\theta}$ this is $\sin((n+1)\theta)/\sin\theta$, interpreted by continuity when $\sin\theta=0$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [19J](../../19j.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
