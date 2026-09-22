<h1 id="26j/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

By [Poisson thinning](../../../../../../poisson-thinning.md), the first arrival times of the coupon types are independent [exponential distribution](../../../../../../exponential-distribution.md) $T_j$ of rates $\lambda p_j$. Completion requires all those arrivals, so $T=\max_jT_j$ and

$$
\boxed{\mathbb P(T<t)=\prod_{j=1}^m(1-e^{-\lambda p_jt})}.
$$

To relate time to count rigorously, let $E_k$ be the successive independent exponential waiting times of mean $1/\lambda$. The completion count $L$ depends only on the coupon labels, which are independent of all $E_k$. Therefore

$$
T=\sum_{k\ge1}E_k\mathbf1_{\{L\ge k\}},\qquad
\mathbb ET=\sum_{k\ge1}\frac1\lambda\mathbb P(L\ge k)=\frac{\mathbb EL}{\lambda}.
$$

Nonnegative integration justifies the sum, avoiding any unproved optional-stopping assertion. Thus the [Poissonized coupon completion time and count](../../../../../../poissonized-coupon-completion-time-and-count.md) identity is **$\lambda\mathbb ET=\mathbb EL$**. Changing variables $s=\lambda t$ in the tail integral gives

$$
\mathbb EL=\int_0^\infty\left[1-\prod_j(1-e^{-p_js})\right]ds,
$$

which depends only on the type probabilities, not $\lambda$. These expectations are finite when all $p_j>0$; a missing type makes both infinite and completion impossible.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [26J](../../26j.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
