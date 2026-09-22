<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $n=T-t$ and define the finite [geometric series](../../../../../../geometric-series.md)

$$
A_0=0,\qquad A_j=\sum_{k=0}^{j-1}\beta^k
=\begin{cases}(1-\beta^j)/(1-\beta),&\beta\ne1,\\j,&\beta=1.\end{cases}
$$

Starting the [autoregressive process of order one](../../../../../../autoregressive-process-of-order-one.md) at time $t$ gives $r_{t+k}=\beta^kr_t+\sum_{j=1}^k\beta^{k-j}\xi_{t+j}$. Consequently

$$
\sum_{k=1}^n r_{t+k}=\beta A_nr_t+\sum_{j=1}^nA_{n-j+1}\xi_{t+j},\qquad
\frac{B_t}{B_T}=\exp\left(-\sum_{k=1}^nr_{t+k}\right).
$$

The future innovations are [independent and identically distributed random variables](../../../../../../independent-and-identically-distributed-random-variables.md), independent of $\mathcal F_t$. Factorizing their exponential [conditional expectation](../../../../../../conditional-expectation.md) and using the [cumulant-generating function](../../../../../../cumulant-generating-function.md) $K$ yields

$$
P(t,T)=e^{-\beta A_nr_t}\prod_{j=1}^n\mathbb E[e^{-A_{n-j+1}\xi_1}]
=\exp\left(-\beta A_nr_t+\sum_{j=1}^nK(-A_j)\right).
$$

Thus the [exponential-affine bond pricing](../../../../../../exponential-affine-bond-pricing.md) coefficients are

$$
\boxed{Q(t,T)=-\beta A_{T-t},\qquad R(t,T)=\sum_{j=1}^{T-t}K(-A_j).}
$$

They vanish at maturity, giving $P(T,T)=1$. Everywhere finiteness of $K$ ensures that each [zero-coupon bond](../../../../../../zero-coupon-bond.md) price is positive and finite, including when $\beta$ is zero, negative, or one.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
