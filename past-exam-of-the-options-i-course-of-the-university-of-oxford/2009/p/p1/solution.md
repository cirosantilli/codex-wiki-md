<h1 id="p/p1/solution">Solution</h1>

↑ **Parent:** [P1](../p1.md)

The [Gershgorin circle theorem](../../../../gershgorin-circle-theorem.md) states that every complex [eigenvalue](../../../../eigenvalue.md) $\lambda$ of $A=(a_{ij})$ belongs to at least one closed disc

$$
D_i=\left\{z\in\mathbb C:|z-a_{ii}|\leq\sum_{j\ne i}|a_{ij}|\right\}.
$$

To prove it, take an [eigenvector](../../../../eigenvector.md) $v\ne0$ and choose $i$ with $|v_i|=\max_j|v_j|>0$. The $i$th row of $Av=\lambda v$ gives

$$
|\lambda-a_{ii}|\,|v_i|
=\left|\sum_{j\ne i}a_{ij}v_j\right|
\leq\sum_{j\ne i}|a_{ij}|\,|v_j|
\leq|v_i|\sum_{j\ne i}|a_{ij}|.
$$

Division by $|v_i|$ proves the assertion. The proof works for real matrices even when their eigenvalues or eigenvectors are complex.

For $B+\mu I$, the three discs have centres $2+\mu,3+\mu,4+\mu$ and radii $2,3,4$. Every point in their [union](../../../../set-union.md) has real part at least $\mu$. Thus for $\mu>0$ no disc contains zero, and zero cannot be an [eigenvalue](../../../../eigenvalue.md). Hence **$B+\mu C$ is nonsingular**.

## ↑ Ancestors (12)

1. [P1](../p1.md)
2. [P](../../p.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
