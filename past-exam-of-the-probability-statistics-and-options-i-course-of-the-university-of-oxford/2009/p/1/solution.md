<h1 id="p/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

[Gershgorin circle theorem](../../../../gershgorin-circle-theorem.md) places every complex [eigenvalue](../../../../eigenvalue.md) of $A$ in at least one disk $D_i=\{z:|z-a_{ii}|\leq\sum_{j\ne i}|a_{ij}|\}$. To prove it, take a nonzero [eigenvector](../../../../eigenvector.md) $v$ and choose $i$ with $|v_i|=\max_j|v_j|>0$. The $i$th [eigenvector](../../../../eigenvector.md) equation gives

$$
|\lambda-a_{ii}|\,|v_i|=\left|\sum_{j\ne i}a_{ij}v_j\right|
\leq\sum_{j\ne i}|a_{ij}|\,|v_i|.
$$

Division by $|v_i|$ proves the disk bound.

Here $C=I$, and the three disks for $B+\mu I$ have real centres $2+\mu$, $3+\mu$, $4+\mu$ and radii $2,3,4$ respectively. Every point in every disk has real part at least $\mu>0$. Hence zero cannot be an [eigenvalue](../../../../eigenvalue.md), proving **$B+\mu C$ is nonsingular for every $\mu>0$**.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [P](../../p.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options I course of the University of Oxford](../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
