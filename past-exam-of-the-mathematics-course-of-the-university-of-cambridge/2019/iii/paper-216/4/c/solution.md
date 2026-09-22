<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Ignoring constants, the complete-data log posterior is

$$
-\frac1{2\sigma^2}\|Y-X\beta\|^2
-\frac1{2\sigma_\beta^2}\|\beta\|^2
+\sum_{i,j}\{X_{ij}\log\pi_j+(1-X_{ij})\log(1-\pi_j)\}.
$$

Take conditional expectations under $(\beta^{(t)},\pi^{(t)})$. Define

$$
A=\frac1{2\sigma^2}\mathbb E[X^TX\mid Y,X_O,\theta^{(t)}]
+\frac1{2\sigma_\beta^2}I,
$$



$$
d=A^{-1}\frac{\mathbb E[X\mid Y,X_O,\theta^{(t)}]^TY}{2\sigma^2},
\quad
r_j=\sum_i\mathbb E[X_{ij}\mid\cdots],
\quad q_j=n-r_j.
$$

Completing the square gives

$$
Q=-(\beta-d)^TA(\beta-d)
+\sum_j\{r_j\log\pi_j+q_j\log(1-\pi_j)\}
+\text{constant}.
$$

For $v\ne0$,

$$
v^TAv=\frac1{2\sigma^2}\mathbb E\|Xv\|^2
+\frac1{2\sigma_\beta^2}\|v\|^2>0,
$$

so $A$ is positive definite. Exact rowwise expectations require summing over $2^{|U_i|}$ states. Thus the cost is exponential in the largest number of missing covariates in one row, more precisely $\sum_i2^{|U_i|}$ times a polynomial factor for accumulating first and second moments.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 216](../../../paper-216-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
