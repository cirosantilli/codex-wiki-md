<h1 id="29k/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Under a [risk-neutral measure](../../../../../../risk-neutral-probability-in-a-binomial-market.md), the discounted stock must be a [martingale](../../../../../../martingale-split.md). If $q$ is the probability of the factor $1+b$, this condition is

$$
q(1+b)+(1-q)(1+a)=1+r,
$$

so

$$
\boxed{q=\frac{r-a}{b-a}}.
$$

The hypothesis $a<r<b$ ensures $0<q<1$, making this equivalent to the original probability measure. Since the $N$ returns are independent under $Q$, the number of up moves has a [binomial distribution](../../../../../../binomial-distribution.md), and hence

$$
\boxed{
Q\!\left(S_N=S_0(1+b)^i(1+a)^{N-i}\right)
=\binom Niq^i(1-q)^{N-i}}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [29K](../../29k.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
