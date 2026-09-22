<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Put $D_j=\widetilde H(x_j)-\widetilde H(x_{j-1})$, with $\widetilde H(x_0)=0$. Then

$$
\sum_{i=1}^n\widetilde H(x_i)
=\sum_{j=1}^n(n-j+1)D_j.
$$

The natural local calibration is therefore

$$
(n-j+1)D_j=v_j,
\qquad
D_j=\frac{v_j}{n-j+1}.
$$

Taking $\widetilde H$ to be the right-continuous step function with these increments gives

$$
\widetilde H(t)=\sum_{j:x_j\leq t}\frac{v_j}{n-j+1}.
$$

Because $n-j+1$ is exactly the risk-set size $r_j$, this is the estimator from part c and automatically satisfies $\sum_i\{v_i-\widetilde H(x_i)\}=0$.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [4](../../4.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
