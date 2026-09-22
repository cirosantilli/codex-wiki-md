<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write

$$
\mu_+=\lim_{n\to\infty}\mathbb E_{F_+}T_n.
$$

If $X_+\sim F_+$, then $X_+-2b_1\sim F_-$ because $F_-(t)=F_+(t+2b_1)$. The [translation-invariant estimator](../../../../../../translation-invariant-estimator.md) property gives

$$
\mu_-:=\lim_{n\to\infty}\mathbb E_{F_-}T_n
=\mu_+-2b_1.
$$

For every real $u$,

$$
\max\{|u|,|u-2b_1|\}\geq b_1.
$$

Taking $u=\mu_+$ shows that every admissible estimator has maximum asymptotic bias at least $b_1$ on the pair $\{F_+,F_-\}$. Therefore

$$
\inf_{\{T_n\}\subset\mathcal T}
\sup_{F\in\mathcal P_\varepsilon^K(\Phi)\cap\mathcal M}
b(\{T_n\},F)\geq b_1.
$$

Together with part a, this proves the [minimax asymptotic bias](../../../../../../minimax-asymptotic-bias.md) optimality of the median.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 223](../../../paper-223-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
