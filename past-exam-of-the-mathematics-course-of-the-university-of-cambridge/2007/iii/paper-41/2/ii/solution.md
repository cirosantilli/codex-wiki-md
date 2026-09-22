<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Suppose under the physical measure $P$ the up indicators are independent with probability $p\in(0,1)$. If $N_k$ is the number of up moves through date $k$, a particular history has probability $p^{N_k}(1-p)^{k-N_k}$ under $P$ and $q^{N_k}(1-q)^{k-N_k}$ under $Q$. Thus the [binomial-market probability density](../../../../../../binomial-market-probability-density.md), the [Radon-Nikodym derivative](../../../../../../radon-nikodym-derivative.md) on $\mathcal F_k$, is

$$
\boxed{L_k=\left.\frac{dQ}{dP}\right|_{\mathcal F_k}=\left(\frac qp\right)^{N_k}\left(\frac{1-q}{1-p}\right)^{k-N_k}.}
$$

It is strictly positive. Its next multiplier has conditional expectation $p(q/p)+(1-p)((1-q)/(1-p))=1$, so $L_k$ is a mean-one [martingale](../../../../../../martingale-split.md) and $L_k=\mathbb E_P[L_n\mid\mathcal F_k]$. These facts verify normalization and equivalence of the two probability measures.

The [state-price density](../../../../../../state-price-density.md) for terminal cash is $\zeta_n=L_n/B_n=b^{-n}L_n$. In particular $V_0=\mathbb E_P[\zeta_nH]$. At an intermediate date the conditional change-of-measure identity gives

$$
V_k=\frac{B_k}{L_k}\mathbb E_P\left[\frac{L_nH}{B_n}\ \middle|\ \mathcal F_k\right].
$$

If physical up probabilities depend on the past, replace the constant-probability expression by the product over periods of $q/p_k$ on an up move and $(1-q)/(1-p_k)$ on a down move. Each multiplier still has conditional mean one, provided $0<p_k<1$, and the pricing measure retains conditional up probability $q$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 41](../../../paper-41-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
