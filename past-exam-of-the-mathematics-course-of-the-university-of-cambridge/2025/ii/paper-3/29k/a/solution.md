<h1 id="29k/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [European call option](../../../../../../european-call-option.md) with maturity $N$ and strike $K$ pays

$$
(S_N-K)^+
$$

at time $N$. Let $q$ be the risk-neutral conditional probability of the factor $1+b$. The discounted stock must be a martingale, so

$$
q(1+b)+(1-q)(1+a)=1+r,
$$

and therefore

$$
q=\frac{r-a}{b-a},
\qquad
1-q=\frac{b-r}{b-a}.
$$

Both probabilities are strictly positive. At every node these are the unique probabilities satisfying the martingale condition, so the [fundamental theorem of asset pricing](../../../../../../fundamental-theorem-of-asset-pricing.md) gives a unique no-arbitrage price.

If exactly $n$ of the $N$ moves use the factor $1+a$, then

$$
S_N=S_0(1+a)^n(1+b)^{N-n},
$$

and there are $\binom Nn$ such paths. Discounted risk-neutral expectation now gives

$$
\operatorname{EC}(N,K)
=\sum_{n=0}^N w(n,N)
\left(S_0(1+a)^n(1+b)^{N-n}-K\right)^+,
$$

where

$$
\boxed{
w(n,N)
=\frac1{(1+r)^N}\binom Nn
\left(\frac{b-r}{b-a}\right)^n
\left(\frac{r-a}{b-a}\right)^{N-n}}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [29K](../../29k.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
