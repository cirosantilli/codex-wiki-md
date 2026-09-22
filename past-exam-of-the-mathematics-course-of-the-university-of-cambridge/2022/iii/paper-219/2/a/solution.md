<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The vector $(y_1,y_2,y_3)$ is [Jointly Gaussian](../../../../../../multivariate-normal-distribution.md). Assuming $R>0$, [Gaussian conditional independence](../../../../../../gaussian-conditional-independence.md) gives

$$
y_3\mathbin\perp y_1\mid y_2
\quad\Longleftrightarrow\quad
\operatorname{Cov}(y_1,y_3\mid y_2)
=R_{13}-\frac{R_{12}R_{23}}R=0.
$$

Thus the required condition is $RR_{13}=R_{12}R_{23}$. Under it, conditioning on $y_1$ supplies no further information after $y_2$, and the [Gaussian process regression posterior](../../../../../../gaussian-process-regression-posterior.md) is

$$
y_3\mid y_2,y_1
\sim N\!\left(
\mu+\frac{R_{23}}R(y_2-\mu),
R-\frac{R_{23}^2}R
\right).
$$

Both the [conditional expectation](../../../../../../conditional-expectation.md) and [conditional variance](../../../../../../conditional-variance.md) depend only on $y_2,t_2,t_3$; neither contains $y_1$ or $t_1$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
