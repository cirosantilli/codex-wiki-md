<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Averaging the slow propensities over the conditional Poisson distribution uses $\mathbb E[Y(Y-1)\mid X=x]=q(x)^2$. Thus the effective birth and death rates of $X$ are

$$
\boxed{\lambda_1(x)=\frac{\alpha_1}{V}q(x)^2
=\frac{\alpha_1\alpha_3^2V^3}{\alpha_4^2x^2},}
$$



$$
\boxed{\lambda_2(x)=\frac{\alpha_2}{V}x(x-1).}
$$

Consequently

$$
\boxed{\partial_tp_0(x,t)
=([E_x^{-1}-1]\lambda_1(x)
+[E_x^{+1}-1]\lambda_2(x))p_0(x,t).}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 356](../../../paper-356-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
