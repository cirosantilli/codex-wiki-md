<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the first [order statistic](../../../../../order-statistic.md) and correct its bias:

$$
\widehat\theta(\mathbf X)=X_{(1)}-\frac1{n+1},\qquad X_{(1)}=\min_{1\leq i\leq n}X_i.
$$

This is a [measurable function](../../../../../measurable-function.md) of the sample. Under $U_\theta^n$, write $Z=X_{(1)}-\theta$. It lies in $[0,1]$, and [independence](../../../../../independent-random-variables.md) gives

$$
\mathbb P_\theta(Z>u)
=\prod_{i=1}^n\mathbb P_\theta(X_i>\theta+u)
=(1-u)^n,\qquad0\leq u\leq1.
$$

For a bounded nonnegative [random variable](../../../../../random-variable-split.md), integrating the identities $Z=\int_0^1\mathbf1_{\{Z>u\}}\,du$ and $Z^2=\int_0^1 2u\mathbf1_{\{Z>u\}}\,du$ proves the [tail integral formula for moments](../../../../../tail-integral-formula-for-moments.md) by [Tonelli's theorem](../../../../../tonelli-theorem.md). Hence

$$
\begin{aligned}
\mathbb E_\theta Z&=\int_0^1(1-u)^n\,du=\frac1{n+1},\\
\mathbb E_\theta Z^2&=2\int_0^1u(1-u)^n\,du
=2\left(\frac1{n+1}-\frac1{n+2}\right)
=\frac2{(n+1)(n+2)}.
\end{aligned}
$$

Thus $\widehat\theta$ is an [unbiased estimator](../../../../../unbiased-estimator.md). Its [quadratic risk](../../../../../quadratic-risk.md) is the [variance](../../../../../variance-split.md) of $Z$, independent of $\theta$:

$$
\mathbb E_\theta(\widehat\theta-\theta)^2
=\frac2{(n+1)(n+2)}-\frac1{(n+1)^2}
=\frac{n}{(n+1)^2(n+2)}.
$$

Taking the [supremum](../../../../../supremum.md) over all real $\theta$ and then the [infimum](../../../../../infimum.md) over [estimators](../../../../../estimator.md) gives

$$
\boxed{m_n\leq\frac{n}{(n+1)^2(n+2)}\leq\frac1{n^2},\qquad C'=1.}
$$

The final inequality follows from $n^3\leq(n+1)^2(n+2)$. Together with part (i), this proves that the [minimax risk](../../../../../minimax-risk.md) has order $n^{-2}$ for all $n\geq1$. In the last line of the source, the request for the upper-bound constant calls it $C$; here it is denoted $C'$ consistently with the upper-bound inequality.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the algorithmic foundations of learning course of the University of Oxford](../../../../split.md)
6. [Algorithmic foundations of learning course of the University of Oxford](../../../../../algorithmic-foundations-of-learning-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
