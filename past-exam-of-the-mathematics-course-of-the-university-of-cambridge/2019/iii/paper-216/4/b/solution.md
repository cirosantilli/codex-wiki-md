<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $U_i=\{j:(i,j)\notin O\}$ and let $x_{i,O}$ denote the observed entries in row $i$. Conditional on the parameters, different rows of the missing design are independent, while the missing entries within one row are coupled by its Gaussian response. For $z\in\{0,1\}^{U_i}$,

$$
\Pr(X_{i,U_i}=z\mid Y,X_O,\beta,\pi)
\propto
\exp\left[-\frac{(Y_i-x_i(z)^T\beta)^2}{2\sigma^2}\right]
\prod_{j\in U_i}\pi_j^{z_j}(1-\pi_j)^{1-z_j}.
$$

Normalizing this expression over the $2^{|U_i|}$ configurations and multiplying over rows gives the full conditional distribution of $X_U$.

## ↑ Ancestors (11)

1. [B](../b.md)
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
