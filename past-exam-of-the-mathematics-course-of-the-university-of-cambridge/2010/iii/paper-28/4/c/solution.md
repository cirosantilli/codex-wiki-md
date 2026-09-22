<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $U_m$ be the average over all $d=p+1$ coordinate tuples in part (a), and $V_m$ the distinct-tuple average in part (b). Every product summand lies in $[0,1]$. A proportion $\alpha_m=(N)_d/N^d$, where $N=m+1$, of all tuples have distinct coordinates. Thus

$$
U_m=\alpha_mV_m+(1-\alpha_m)W_m,
$$

where $W_m\in[0,1]$ is the average over the remaining tuples. If there are no remaining tuples, the error is zero. Hence $|U_m-V_m|\leq1-\alpha_m$.

For $d$ independent uniform choices from $N$ indices, any particular pair coincides with [probability](../../../../../../probability.md) $1/N$. A [union bound](../../../../../../boole-s-inequality.md) over the $\binom d2$ pairs gives

$$
\boxed{|U_m-V_m|\leq1-\frac{(N)_d}{N^d}\leq\frac{\binom d2}{N}\longrightarrow0.}
$$

This deterministic [sampling with and without replacement comparison for bounded products](../../../../../../sampling-with-and-without-replacement-comparison-for-bounded-products.md) is the needed link between the two averages.

Part (a) identifies the almost-sure limit of $U_m$ as $\prod_{k=0}^p\mathbb E[\mathbf1_{A_k}(X_k)\mid\mathcal S]$. By part (b) and the [reverse martingale convergence theorem](../../../../../../reverse-martingale-convergence-theorem.md), $V_m$ converges almost surely to $\mathbb E[\prod_{k=0}^p\mathbf1_{A_k}(X_k)\mid\mathcal S]$. Their difference vanishes, so

$$
\boxed{\mathbb E\!\left[\prod_{k=0}^p\mathbf1_{A_k}(X_k)\mid\mathcal S\right]
=\prod_{k=0}^p\mathbb E[\mathbf1_{A_k}(X_k)\mid\mathcal S]\quad\text{almost surely}.}
$$

This is precisely [conditional independence](../../../../../../conditional-independence.md). Exchangeability also makes the single-coordinate conditional laws identical, by applying a coordinate transposition and testing against invariant events. The result is the [De Finetti theorem](../../../../../../de-finetti-theorem.md), established here by finite symmetrization and the vanishing collision fraction.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
