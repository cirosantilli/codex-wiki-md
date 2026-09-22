<h1 id="3/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [Schur complement](../../../../../schur-complement.md) can be written

$$
s=\underbrace{k(x_n,x_n)-b^TA^{-1}b}_{v_{n-1}(x_n)}+\sigma^2>0,
$$

because the first term is a [conditional variance](../../../../../conditional-variance.md) and $\sigma^2>0$. Therefore $c_1=s^{-1}>0$ and the squared term is nonnegative, so

$$
\boxed{\operatorname{Var}_{n-1}(f_*)\geq\operatorname{Var}_n(f_*)}.
$$

Equality holds exactly when the remaining [conditional covariance](../../../../../conditional-covariance.md) $k(x_n,x_*)-b^TA^{-1}a$ is zero. In particular, the reduction need not be strict even at a previously unseen input.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the advanced topics in statistical machine learning course of the University of Oxford](../../../../split.md)
6. [Advanced topics in statistical machine learning course of the University of Oxford](../../../../../advanced-topics-in-statistical-machine-learning-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics and statistics course of the University of Oxford](../../../../../year-4-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
