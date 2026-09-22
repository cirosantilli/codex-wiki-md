<h1 id="40c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Gershgorin circle theorem](../../../../../../gershgorin-circle-theorem.md) states that every [eigenvalue](../../../../../../eigenvalue.md) $\lambda$ of a complex matrix $A=(a_{ij})$ lies in at least one disk

$$
\boxed{
|\lambda-a_{ii}|
\leq\sum_{j\ne i}|a_{ij}|}.
$$

To prove it, choose a nonzero [eigenvector](../../../../../../eigenvector.md) $x$ for $\lambda$ and an index $i$ such that $|x_i|=\max_j|x_j|>0$. The $i$th component of $Ax=\lambda x$ gives

$$
(\lambda-a_{ii})x_i
=\sum_{j\ne i}a_{ij}x_j.
$$

Taking absolute values and using $|x_j|\leq|x_i|$ yields

$$
|\lambda-a_{ii}|\,|x_i|
\leq\sum_{j\ne i}|a_{ij}|\,|x_j|
\leq |x_i|\sum_{j\ne i}|a_{ij}|.
$$

Division by $|x_i|$ proves the theorem.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [40C](../../40c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
