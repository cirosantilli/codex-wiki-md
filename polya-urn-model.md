<h1 id="polya-urn-model">Pólya urn model</h1>

↑ **Parent:** [Stochastic process](stochastic-process-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pólya_urn_model)

Begin with positive counts of two colours. At each step select one ball uniformly and replace it together with one new ball of its colour. If the total initial count is $m$, the blue proportion satisfies $X_{n+1}-X_n=(I_{n+1}-X_n)/(m+n+1)$, where the next blue indicator has conditional mean $X_n$. Thus $X_n$ is a bounded [martingale](martingale-split.md) and converges almost surely and in $L^2$ to a random proportion. If uniforms generate the draws, the update from time $n$ to $n+1$ must use the fresh $U_{n+1}$ relative to $\mathcal F_n=\sigma(U_1,\ldots,U_n)$.

**Table of contents**

- [Positivity of the limiting Pólya urn proportion](positivity-of-the-limiting-polya-urn-proportion.md)

## ↑ Ancestors (6)

1. [Stochastic process](stochastic-process-split.md)
2. [Probability theory](probability-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
