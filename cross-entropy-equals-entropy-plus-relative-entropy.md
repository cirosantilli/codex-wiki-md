# Cross-entropy equals entropy plus relative entropy

↑ **Parent:** [Cross-entropy](cross-entropy.md)

For finite [probability mass functions](probability-mass-function.md), with $q_i>0$ whenever $p_i>0$, subtract the two [expectations](expected-value.md) of [logarithmic loss](logarithmic-loss.md):

$$
\begin{aligned}
H(P,Q)-H(P)
&=\sum_{i:p_i>0}p_i(\log_2 p_i-\log_2 q_i)\\
&=\sum_{i:p_i>0}p_i\log_2\frac{p_i}{q_i}
=D_{\mathrm{KL}}(P\Vert Q).
\end{aligned}
$$

The [Gibbs inequality](gibbs-inequality.md) makes the difference nonnegative and zero exactly when $P=Q$. If $Q$ assigns zero [probability](probability.md) to an outcome with positive [probability](probability.md) under $P$, both the [cross-entropy](cross-entropy.md) and the [Kullback-Leibler divergence](kullback-leibler-divergence.md) are infinite. The finite [information entropy](information-entropy.md) still leaves the displayed identity valid in the extended sense. In more general settings, undefined differences such as $\infty-\infty$ cannot be used as a derivation.

## ↑ Ancestors (7)

1. [Cross-entropy](cross-entropy.md)
2. [Information entropy](information-entropy.md)
3. [Information theory](information-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Cross-entropy](cross-entropy.md)
- [Relative entropy to a product law](relative-entropy-to-a-product-law.md)
