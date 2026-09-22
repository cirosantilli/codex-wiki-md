<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

A [Hermitian matrix](../../../../hermitian-operator.md) satisfies $A^\dagger=\overline A^T=A$. If $Av=\lambda v$ with $v\ne0$, then $v^\dagger Av=\lambda v^\dagger v$ is real because its conjugate equals $v^\dagger A^\dagger v=v^\dagger Av$. Since $v^\dagger v>0$, its [eigenvalue](../../../../eigenvalue.md) $\lambda$ is real. If $Aw=\mu w$ with $\mu\ne\lambda$, then

$$
\mu v^\dagger w=v^\dagger Aw=(Av)^\dagger w=\lambda v^\dagger w,
$$

so $v^\dagger w=0$: distinct eigenspaces are [orthogonal](../../../../orthogonal-vectors.md) for the standard complex [inner product](../../../../inner-product-split.md).

The converse is false. For example $\begin{pmatrix}1&1\\0&2\end{pmatrix}$ has the two real [eigenvalues](../../../../eigenvalue.md) one and two but is not a [Hermitian matrix](../../../../hermitian-operator.md). It can be embedded as a block in a $3\times3$ example if desired.

For Hermitian $A,B$, $(AB)^\dagger=B^\dagger A^\dagger=BA$. Thus $AB$ is Hermitian exactly when $AB=BA$, equivalently when their [commutator](../../../../commutator.md) vanishes. Also $(AB+BA)^\dagger=AB+BA$, so a value that works for every such pair is

$$
\boxed{c=1.}
$$

This sum is their [anticommutator](../../../../anticommutator.md).

## ↑ Ancestors (12)

1. [6](../6.md)
2. [Paper 1](../../paper-1-split.md)
3. [2008](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
