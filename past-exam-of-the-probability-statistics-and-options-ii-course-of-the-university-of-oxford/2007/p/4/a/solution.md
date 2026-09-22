<h1 id="p/4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Gershgorin circle theorem](../../../../../gershgorin-circle-theorem.md) states that every complex [eigenvalue](../../../../../eigenvalue.md) of a square [matrix](../../../../../matrix.md) $A$ lies in at least one closed disc $D_i=\{z:|z-a_{ii}|\le\sum_{j\ne i}|a_{ij}|\}$. To prove it, take a nonzero [eigenvector](../../../../../eigenvector.md) $v$ for $\lambda$ and choose $i$ with $|v_i|$ maximal. The $i$th row of $Av=\lambda v$ gives

$$
|\lambda-a_{ii}|\,|v_i|
=\left|\sum_{j\ne i}a_{ij}v_j\right|
\le\sum_{j\ne i}|a_{ij}|\,|v_j|
\le\left(\sum_{j\ne i}|a_{ij}|\right)|v_i|.
$$

Division by $|v_i|>0$ proves the claim. The proof applies to real and complex [matrices](../../../../../matrix.md) alike.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [4](../../4.md)
3. [P](../../../p.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
