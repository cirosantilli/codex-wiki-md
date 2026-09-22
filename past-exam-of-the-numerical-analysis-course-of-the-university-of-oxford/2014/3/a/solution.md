<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Gershgorin circle theorem](../../../../gershgorin-circle-theorem.md) states that every [eigenvalue](../../../../eigenvalue.md) of $A=(a_{ij})\in\mathbb R^{n\times n}$ belongs to at least one of the closed [Gershgorin discs](../../../../gershgorin-disc.md)

$$
\boxed{D_i=\left\{z\in\mathbb C:|z-a_{ii}|\leq r_i\right\},\qquad r_i=\sum_{j\ne i}|a_{ij}|.}
$$

The [eigenvalue](../../../../eigenvalue.md) may be complex even though the [matrix](../../../../matrix.md) is real. To prove the theorem, choose a nonzero complex [eigenvector](../../../../eigenvector.md) $v$ with $Av=\lambda v$ and an index $i$ at which $|v_i|$ is maximal. Then $|v_i|>0$, and the $i$th row gives

$$
(\lambda-a_{ii})v_i=\sum_{j\ne i}a_{ij}v_j.
$$

The [triangle inequality](../../../../triangle-inequality.md) yields

$$
|\lambda-a_{ii}|\leq\sum_{j\ne i}|a_{ij}|\frac{|v_j|}{|v_i|}\leq\sum_{j\ne i}|a_{ij}|=r_i.
$$

Thus $\lambda\in D_i$, proving the assertion without any symmetry assumption.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2014](../../../2014-split.md)
4. [Past exam of the numerical analysis course of the University of Oxford](../../../split.md)
5. [Numerical analysis course of the University of Oxford](../../../../numerical-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
