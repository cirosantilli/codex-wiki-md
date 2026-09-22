<h1 id="40a/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $D=\operatorname{diag}(A)$. The [Jacobi method](../../../../../../../jacobi-method.md) is

$$
x_{k+1}=(I-D^{-1}A)x_k+D^{-1}b,
$$

so $H=I-D^{-1}A$ and $v=D^{-1}b$. If $A$ is strictly diagonally dominant, every Gershgorin disc of $H$ is centered at zero and has radius

$$
\sum_{j\ne i}\frac{|a_{ij}|}{|a_{ii}|}<1.
$$

Every [eigenvalue](../../../../../../../eigenvalue.md) therefore has [modulus](../../../../../../../modulus.md) below one, so $\rho(H)<1$ and part (i) proves convergence.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [40A](../../../40a.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
