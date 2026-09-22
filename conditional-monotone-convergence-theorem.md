# Conditional monotone convergence theorem

↑ **Parent:** [Conditional expectation](conditional-expectation.md)

For nonnegative [random variables](random-variable-split.md) $Y_n\uparrow Y$, the corresponding nonnegative [conditional expectations](conditional-expectation.md) increase [almost surely](almost-sure-convergence.md) to $\mathbb E[Y\mid\mathcal G]$, allowing the extended value $+\infty$. When $Y$ is an [integrable random variable](integrable-random-variable.md), all [conditional expectations](conditional-expectation.md) can be taken in their ordinary finite sense.

To prove this integrable case, choose versions simultaneously ordered outside a single [null set](null-set.md), and put $V=\lim_n\mathbb E[Y_n\mid\mathcal G]$. This limit is $\mathcal G$-[measurable](measurability.md). For every $A\in\mathcal G$, the ordinary [monotone convergence theorem](monotone-convergence-theorem.md) twice gives

$$
\mathbb E[\mathbf1_AV]
=\lim_n\mathbb E[\mathbf1_A\mathbb E[Y_n\mid\mathcal G]]
=\lim_n\mathbb E[\mathbf1_AY_n]
=\mathbb E[\mathbf1_AY].
$$

In particular $\mathbb EV=\mathbb EY<\infty$, and this is exactly the defining property of [conditional expectation](conditional-expectation.md). For a general nonnegative $Y$, define its extended [conditional expectation](conditional-expectation.md) by increasing bounded truncations; the same nonnegative [integral](integral-split.md) argument proves the statement.

## ↑ Ancestors (7)

1. [Conditional expectation](conditional-expectation.md)
2. [Measure theory](measure-theory-split.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Measurable-factor rule for conditional expectation](measurable-factor-rule-for-conditional-expectation.md)
