<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Jordan–Chevalley decomposition](../../../../../../jordan-chevalley-decomposition.md) is characterized by

$$
\boxed{X=X_s+X_n,\quad X_s\text{ diagonalizable},\quad X_n\text{ nilpotent},\quad[X_s,X_n]=0.}
$$

Over $\mathbb C$, a semisimple [linear operator](../../../../../../linear-operator.md) is a diagonalizable one. These conditions determine the two parts uniquely. Concretely, on the [generalized eigenspace](../../../../../../generalized-eigenspace.md) for an [eigenvalue](../../../../../../eigenvalue.md) $\lambda$, the semisimple part is $\lambda I$ and the nilpotent part is $X-\lambda I$; both are polynomials in $X$. To see uniqueness, any commuting candidate parts preserve each generalized eigenspace; diagonalize the proposed semisimple part there, and nilpotence then forces its eigenvalue to be the sole eigenvalue $\lambda$ of $X$ on that space.

For the displayed matrix, $\det(tI-X)=(t-1)^2$ and

$$
N=X-I=\begin{pmatrix}1&1\\-1&-1\end{pmatrix},\qquad N^2=0.
$$

Since $I$ is semisimple and commutes with $N$, the required parts are

$$
\boxed{X_s=I_2,\qquad X_n=\begin{pmatrix}1&1\\-1&-1\end{pmatrix}.}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5](../../5.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
