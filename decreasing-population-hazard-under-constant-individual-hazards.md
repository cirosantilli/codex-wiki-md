# Decreasing population hazard under constant individual hazards

↑ **Parent:** [Population hazard of a survival mixture](population-hazard-of-a-survival-mixture.md)

For a nonnegative random constant individual hazard $\Lambda$, write $M_k(t)=\mathbb E[\Lambda^ke^{-\Lambda t}]$. The population survivor function is $M_0$ and its hazard is $M_1/M_0$. Under the integrability needed to differentiate, $M_k'=-M_{k+1}$, so

$$
\overline h'=\frac{-M_2M_0+M_1^2}{M_0^2}=-\operatorname{Var}(\Lambda\mid T>t).
$$

The conditional distribution is weighted by $e^{-\Lambda t}$. This proves decreasing population hazard without any decrease in individual hazards and explains [survival selection in a heterogeneous population](survival-selection-in-a-heterogeneous-population.md).

## ↑ Ancestors (8)

1. [Population hazard of a survival mixture](population-hazard-of-a-survival-mixture.md)
2. [Hazard function](hazard-function.md)
3. [Survival function](survival-function.md)
4. [Survival analysis](survival-analysis-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-46/5/b/solution.md)
