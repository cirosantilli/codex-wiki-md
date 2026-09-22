<h1 id="p/1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Gershgorin circle theorem](../../../../../gershgorin-circle-theorem.md) states that every [eigenvalue](../../../../../eigenvalue.md) of $A$ lies in at least one disc

$$
D_i=\left\{z\in\mathbb C:|z-a_{ii}|\leq\sum_{j\ne i}|a_{ij}|\right\}.
$$

For a nonzero complex [eigenvector](../../../../../eigenvector.md) $v$, choose an index $i$ with $|v_i|=\max_j|v_j|>0$. The $i$th row of $Av=\lambda v$ gives

$$
|\lambda-a_{ii}|\,|v_i|\leq\sum_{j\ne i}|a_{ij}|\,|v_j|
\leq\left(\sum_{j\ne i}|a_{ij}|\right)|v_i|.
$$

Dividing by $|v_i|$ proves membership in $D_i$. This is valid for real matrices even when the eigenvalues are complex.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [1](../../1.md)
3. [P](../../../p.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options I course of the University of Oxford](../../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
