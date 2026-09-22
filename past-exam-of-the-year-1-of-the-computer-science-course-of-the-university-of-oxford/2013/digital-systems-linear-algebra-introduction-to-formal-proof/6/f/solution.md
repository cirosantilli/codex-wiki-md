<h1 id="6/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

The other [eigenvalues](../../../../../eigenvalue.md) are $1/2$ and $0$. Their magnitudes are strictly less than one. All three [eigenvalues](../../../../../eigenvalue.md) are distinct, so their [eigenvectors](../../../../../eigenvector.md) form a [basis](../../../../../basis.md) and the [matrix](../../../../../matrix.md) is [diagonalizable](../../../../../diagonalizable-matrix.md). Every component outside the stationary direction therefore decays under repeated application of $P$.

For an explicit justification, choose

$$
w=(0,1,-1)^{\mathsf T},\qquad u=(-2,1,1)^{\mathsf T}.
$$

Then $Pw=w/2$, $Pu=0$, and

$$
x(0)=10v-\frac72w+2u.
$$

The zero-[eigenvalue](../../../../../eigenvalue.md) component disappears after one step. For every $n\geq1$,

$$
\boxed{x(n)=\begin{pmatrix}5\\5/2-(7/2)2^{-n}\\5/2+(7/2)2^{-n}\end{pmatrix}\ \longrightarrow\ \begin{pmatrix}5\\5/2\\5/2\end{pmatrix}.}
$$

Thus the shares converge to $v$ and the resource [vector](../../../../../vector.md) converges to $10v$, since the conserved total is ten. For any other initial resource [vector](../../../../../vector.md) of total $T$, the same [eigenvector](../../../../../eigenvector.md) argument gives the limit $Tv$.

## ↑ Ancestors (12)

1. [F](../f.md)
2. [6](../../6.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
