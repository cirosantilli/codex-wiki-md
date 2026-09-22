<h1 id="11f/solution">Solution</h1>

↑ **Parent:** [11F](../11f.md)

Use the positive-support [geometric distribution](../../../../../geometric-distribution.md), $\mathbb P(X=j)=p(1-p)^{j-1}$ for $j\geq1$, $0<p\leq1$. Differentiating the geometric series supplies

$$
\boxed{\mathbb E[X]=\frac1p,\qquad
\mathbb E[X^2]=\frac{2-p}{p^2},\qquad
\operatorname{Var}(X)=\frac{1-p}{p^2}}.
$$

For the jar, let $W_r$ be the waiting time to remove one red ball when exactly $r$ red balls remain. Every draw has success [probability](../../../../../probability.md) $r/n$, so $W_r$ is geometric with that parameter. The $W_r$ are independent: after each success, fresh independent draws begin a new stage, and its conditional waiting distribution depends only on the deterministic count $r$, not on earlier waiting times. Replacing a green ball leaves that stage's count unchanged.

Thus the [coupon collector problem](../../../../../coupon-collector-problem.md) decomposition is $T=\sum_{r=1}^nW_r$, and

$$
\boxed{\mathbb E[T]=n\sum_{r=1}^n\frac1r},\qquad
\boxed{\operatorname{Var}(T)=n^2\sum_{r=1}^n\frac1{r^2}-n\sum_{r=1}^n\frac1r}.
$$

This is the [coupon collector waiting-time variance](../../../../../coupon-collector-waiting-time-variance.md). For $n=1$, the formula correctly gives zero [variance](../../../../../variance-split.md) and a deterministic one-minute completion.

## ↑ Ancestors (10)

1. [11F](../11f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
