<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the [local linear approximation](../../../../../../local-linear-approximation.md) from part (a), with $L=f'(c)$. Since $x_n\leq c\leq y_n$ and $x_n\ne y_n$, we have $y_n-x_n>0$, and subtraction gives

$$
\frac{f(y_n)-f(x_n)}{y_n-x_n}-L=\frac{\epsilon(y_n)(y_n-c)+\epsilon(x_n)(c-x_n)}{y_n-x_n}.
$$

The coefficients $(y_n-c)/(y_n-x_n)$ and $(c-x_n)/(y_n-x_n)$ are nonnegative and sum to one. Therefore

$$
\left|\frac{f(y_n)-f(x_n)}{y_n-x_n}-L\right|\leq\max\{|\epsilon(x_n)|,|\epsilon(y_n)|\}\longrightarrow0.
$$

Here $\epsilon(c)=0$ handles any endpoint of a secant that happens to equal $c$. Thus [secants straddling a differentiability point](../../../../../../secants-straddling-a-differentiability-point.md) satisfy

$$
\boxed{\lim_{n\to\infty}\frac{f(y_n)-f(x_n)}{y_n-x_n}=f'(c).}
$$

## ↑ Ancestors (12)

1. [B](../b.md)
2. [6](../../6.md)
3. [Mathematics II](../../../mathematics-ii-split.md)
4. [Prelims](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
