<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

The remaining [eigenvalues](../../../../../eigenvalue.md) are

$$
\boxed{\lambda_2=\frac35,\qquad\lambda_3=\frac12.}
$$

They have absolute value less than one. The three distinct [eigenvalues](../../../../../eigenvalue.md) give a [basis](../../../../../basis.md) of [eigenvectors](../../../../../eigenvector.md), which may be chosen as $v$, $u=(0,-1,1)^{\mathsf T}$ and $w=(-1,-1,2)^{\mathsf T}$, with $Pu=(3/5)u$ and $Pw=(1/2)w$. Write an arbitrary initial [probability vector](../../../../../probability-vector.md) as $x_0=cv+\alpha u+\beta w$. Summing its entries shows $c=1$, because the entries of $v$ sum to one and those of $u,w$ sum to zero. Therefore

$$
P^nx_0=v+\alpha\left(\frac35\right)^nu+\beta\left(\frac12\right)^nw\longrightarrow v.
$$

This proves [convergence](../../../../../convergence.md) for every initial [probability vector](../../../../../probability-vector.md), rather than merely identifying a possible limit. In particular,

$$
\boxed{\lim_{n\to\infty}x_n=(20\%,45\%,35\%)^{\mathsf T}.}
$$

For the given initial [probability vector](../../../../../probability-vector.md), $\alpha=1/4$ and $\beta=-1/5$; substituting $n=1,2$ also recovers the previous answers. The slowest decaying [eigenvector](../../../../../eigenvector.md) component has factor $(3/5)^n$.

## ↑ Ancestors (12)

1. [F](../f.md)
2. [1](../../1.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
