<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [characteristic polynomial](../../../../../characteristic-polynomial.md) is $\det(\lambda I-A)=\lambda^2-\lambda-1$. Its distinct [eigenvalues](../../../../../eigenvalue.md) are $\alpha=(1+\sqrt5)/2$ and $\beta=(1-\sqrt5)/2$. For either [eigenvalue](../../../../../eigenvalue.md) $\lambda$, the [vector](../../../../../vector.md) $(\lambda,1)^\top$ is an [eigenvector](../../../../../eigenvector.md), since $A(\lambda,1)^\top=(\lambda+1,\lambda)^\top=\lambda(\lambda,1)^\top$.

Choose

$$
\boxed{S=\begin{pmatrix}\alpha&\beta\\1&1\end{pmatrix},\qquad D=\begin{pmatrix}\alpha&0\\0&\beta\end{pmatrix}.}
$$

The [determinant](../../../../../determinant.md) of $S$ is $\alpha-\beta=\sqrt5\ne0$, so

$$
S^{-1}=\frac1{\sqrt5}\begin{pmatrix}1&-\beta\\-1&\alpha\end{pmatrix}.
$$

Its columns being [eigenvectors](../../../../../eigenvector.md) gives $AS=SD$, and left multiplication by $S^{-1}$ proves $S^{-1}AS=D$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
