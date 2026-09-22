<h1 id="9/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

By [linearity of expectation](../../../../../linearity-of-expectation.md), **$\mathbb E[Z]=\sum_i\mathbb E[X_i]=0$**. Expanding the square and again using [linearity of expectation](../../../../../linearity-of-expectation.md) gives

$$
\begin{aligned}
\operatorname{Var}(Z)
&=\mathbb E[Z^2]
=\sum_i\mathbb E[X_i^2]+2\sum_{i<j}\mathbb E[X_iX_j]\\
&=\boxed{\sum_i\sigma_i^2+2\sum_{i<j}\operatorname{Cov}(X_i,X_j)}.
\end{aligned}
$$

Here the zero means imply $\mathbb E[X_i^2]=\sigma_i^2$ and $\mathbb E[X_iX_j]=\operatorname{Cov}(X_i,X_j)$. The [covariance](../../../../../covariance.md) expansion itself does not require [independence](../../../../../independent-random-variables.md). Under the additional [independence](../../../../../independent-random-variables.md) stated here, $\mathbb E[X_iX_j]=\mathbb E[X_i]\mathbb E[X_j]=0$, so it simplifies further to **$\operatorname{Var}(Z)=\sum_i\sigma_i^2$**.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [9](../../9.md)
3. [Discrete mathematics, continuous mathematics, and probability](../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
