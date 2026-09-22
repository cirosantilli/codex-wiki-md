<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Apply $A$ to the stated [linear combination](../../../../../linear-combination.md) and use each [eigenvector](../../../../../eigenvector.md) equation:

$$
\lambda_{k+1}z_{k+1}=Az_{k+1}=\sum_{i=1}^k\alpha_iAz_i=\sum_{i=1}^k\alpha_i\lambda_i z_i.
$$

Subtract $\lambda_{k+1}$ times the original relation. This gives

$$
\sum_{i=1}^k\alpha_i(\lambda_i-\lambda_{k+1})z_i=0.
$$

The assumed [linear independence](../../../../../linear-independence.md) implies $\alpha_i(\lambda_i-\lambda_{k+1})=0$ separately for every $i$. Since the [eigenvector](../../../../../eigenvector.md) $z_{k+1}$ is nonzero, not all $\alpha_i$ can vanish. Choose any $i$ with $\alpha_i\ne0$; division by that coefficient gives **$\lambda_i=\lambda_{k+1}$**. In fact every nonzero coefficient is attached to that same [eigenvalue](../../../../../eigenvalue.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [6](../../6.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
