<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $\xi_j=B_{\sigma_1^j}-B_{\sigma_1^{j-1}}$. Continuity makes each displacement equal to $+1$ or $-1$. Reflection symmetry of a fresh [Brownian motion](../../../../../../brownian-motion-split.md) gives [probability](../../../../../../probability.md) one half to each sign, and the [Strong Markov property](../../../../../../strong-markov-property.md) makes these signs independent across successive exits. Thus $B_{\sigma_1^n}=\sum_{j=1}^n\xi_j$.

For the normalized position, the [characteristic function](../../../../../../characteristic-function.md) is

$$
\mathbb E\exp\left(iu\frac{B_{\sigma_1^n}}{\sqrt n}\right)
=\left[\cos(u/\sqrt n)\right]^n\longrightarrow e^{-u^2/2},
$$

since $\log\cos z=-z^2/2+O(z^4)$ near zero. By the [Lévy continuity theorem](../../../../../../levy-continuity-theorem.md), this proves

$$
\boxed{B_{\sigma_1^n}/\sqrt n\ \Rightarrow\ N(0,1).}
$$

This is the [Gaussian limit of a Brownian exit skeleton](../../../../../../gaussian-limit-of-a-brownian-exit-skeleton.md).

Compare along the subsequence $n=2^{2m}$ with $\tau_m=\sigma_{2^{-m}}^{2^{2m}}$. Joint [Brownian scaling](../../../../../../brownian-scaling.md) of the successive exits gives

$$
B_{\tau_m}\ \stackrel d=\ 2^{-m}B_{\sigma_1^{2^{2m}}}.
$$

The right-hand side converges weakly to $N(0,1)$. The preceding part and path continuity give $B_{\tau_m}\to B_C$ almost surely on the original Brownian [probability](../../../../../../probability.md) space. Hence its weak limit is also the law $N(0,C)$. Uniqueness of the weak limit forces **$C=1$**, so finally **$\mathbb E\sigma_a=a^2$**. [Independence](../../../../../../independent-random-variables.md) of the position and its random clock was not assumed in this comparison.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
