<h1 id="5g/solution">Solution</h1>

↑ **Parent:** [5G](../5g.md)

Relative to the coordinate basis, the [linear map](../../../../../linear-map.md) has matrix

$$
F=\begin{pmatrix}1&3&-1\\0&2&1\\0&-4&-1\end{pmatrix}.
$$

Expanding $\det(tI-F)$ in its first column gives the monic [characteristic polynomial](../../../../../characteristic-polynomial.md)

$$
\boxed{\chi_f(t)=(t-1)(t^2-t+2)}.
$$

Its [eigenvalues](../../../../../eigenvalue.md) are $1$ and $(1\pm i\sqrt7)/2$, three distinct complex numbers. [Eigenvectors](../../../../../eigenvector.md) corresponding to distinct [eigenvalues](../../../../../eigenvalue.md) are linearly independent, so they form a basis of $\mathbb C^3$ and **$f$ is diagonalizable**.

Every annihilating [polynomial](../../../../../polynomial-split.md) must vanish at all three [eigenvalues](../../../../../eigenvalue.md): applying $p(f)$ to a corresponding [eigenvector](../../../../../eigenvector.md) gives $p(\lambda)v$. Conversely, in the eigenbasis the product of the three distinct linear factors annihilates $f$. Hence the [minimal polynomial](../../../../../minimal-polynomial.md) is

$$
\boxed{m_f(t)=(t-1)(t^2-t+2)}.
$$

If $af+bf^2=0$ with scalars $a,b$ not both zero, the nonzero [polynomial](../../../../../polynomial-split.md) $at+bt^2$ of degree at most two would annihilate $f$, contradicting this minimal degree of three. Thus **$f$ and $f^2$ are linearly independent [endomorphisms](../../../../../endomorphism.md)**.

## ↑ Ancestors (10)

1. [5G](../5g.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
