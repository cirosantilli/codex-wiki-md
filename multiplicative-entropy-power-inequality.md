# Multiplicative entropy power inequality

↑ **Parent:** [Entropy power inequality](entropy-power-inequality.md)

For independent positive [random variables](random-variable-split.md) $Y_1,Y_2$ with densities, finite [differential entropies](differential-entropy.md) and finite $\mu_i=\mathbb E\log_2Y_i$, applying the [entropy power inequality](entropy-power-inequality.md) to $Z_i=\ln Y_i$ gives

$$
2^{2h(Y_1Y_2)}\geq2^{2\mu_2}2^{2h(Y_1)}+2^{2\mu_1}2^{2h(Y_2)}.
$$

Indeed $h(Z_i)=h(Y_i)-\mu_i$, while $h(Y_1Y_2)=h(Z_1+Z_2)+\mu_1+\mu_2$, provided the sum's [differential entropy](differential-entropy.md) is defined. Positivity alone does not ensure these expressions exist: $Y=e^T$ with $T$ having [Cauchy distribution](cauchy-distribution.md) has undefined $\mathbb E\log_2Y$.

// Target: algebra.bigb

## ↑ Ancestors (9)

1. [Entropy power inequality](entropy-power-inequality.md)
2. [Entropy power](entropy-power.md)
3. [Differential entropy](differential-entropy.md)
4. [Information entropy](information-entropy.md)
5. [Information theory](information-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-30/2/solution.md)
