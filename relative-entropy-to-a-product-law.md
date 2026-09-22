# Relative entropy to a product law

↑ **Parent:** [Total correlation](total-correlation.md)

Let $P$ be a joint [probability distribution](probability-distribution-split.md) on a finite product [alphabet](alphabet.md), with marginals $P_i$. Compare it with a product model $Q=\bigotimes_iQ_i$, assuming $Q_i(x_i)>0$ wherever $P_i(x_i)>0$. Adding and subtracting the [logarithm](logarithm.md) of $\prod_iP_i(x_i)$ gives

$$
\boxed{D(P\Vert Q)=\operatorname{TC}(P)+\sum_i D(P_i\Vert Q_i).}
$$

The first term is the unavoidable error from discarding dependence; the other terms are errors in the individual marginal [probability distributions](probability-distribution-split.md). Averaging a term that depends only on $x_i$ under $P$ is the same as averaging it under $P_i$, which proves the identity directly.

Among product laws, the choice $Q_i=P_i$ minimizes this [relative entropy](kullback-leibler-divergence.md), leaving exactly [total correlation](total-correlation.md). The related [cross-entropy equals entropy plus relative entropy](cross-entropy-equals-entropy-plus-relative-entropy.md) identity interprets this as extra average [logarithmic loss](logarithmic-loss.md) from using the independent model. It is a statement about a specified joint law and loss function, not a claim that fitting a finite sample automatically recovers that law.

## ↑ Ancestors (6)

1. [Total correlation](total-correlation.md)
2. [Information theory](information-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
