<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For $\mathbf1=(1,1,1)^T$, the entries of $P^T\mathbf1$ are the column sums of $P$. Hence

$$
P^T\mathbf1=\begin{pmatrix}1\\1\\1\end{pmatrix}=\mathbf1,
$$

so $1$ is an [eigenvalue](../../../../../eigenvalue.md) of $P^T$, with [eigenvector](../../../../../eigenvector.md) $\mathbf1$.

The [determinant](../../../../../determinant.md) is unchanged by [matrix transposition](../../../../../transpose.md), so

$$
\det(P-I)=\det((P-I)^T)=\det(P^T-I)=0.
$$

Thus $P-I$ has a nontrivial [null space](../../../../../kernel-of-a-linear-map-split.md), giving

$$
\boxed{1\text{ is also an eigenvalue of }P.}
$$

The same argument with $\lambda I$ shows that a [matrix](../../../../../matrix.md) and its transpose have the same [characteristic polynomial](../../../../../characteristic-polynomial.md). It does not say that they have the same [eigenvectors](../../../../../eigenvector.md): here $P\mathbf1=(0.9,1.2,0.9)^T\ne\mathbf1$.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [5](../../5.md)
3. [Digital systems, linear algebra, introduction to formal proof (resit)](../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
