# Hazard derivative for a mixture of exponential distributions

↑ **Parent:** [Population hazard of a survival mixture](population-hazard-of-a-survival-mixture.md)

For a finite mixture with positive weights $p_i$ and rates $\lambda_i>0$, the [survivor function](survival-function.md) is $S(t)=\sum_i p_i e^{-\lambda_i t}$ and the [hazard function](hazard-function.md) is the surviving-population mean of the component rates. Write $w_i(t)=p_i e^{-\lambda_i t}/S(t)$. Differentiation gives $w_i'=w_i(h-\lambda_i)$ and therefore $h'=h^2-\sum_iw_i\lambda_i^2=-\operatorname{Var}(\Lambda\mid T>t)$. The hazard is decreasing, strictly so when distinct rates have positive weights. For finitely many rates it tends to the smallest rate with positive weight. This is [survival selection](survival-selection-in-a-heterogeneous-population.md) even though each individual component has a constant hazard.

## ↑ Ancestors (8)

1. [Population hazard of a survival mixture](population-hazard-of-a-survival-mixture.md)
2. [Hazard function](hazard-function.md)
3. [Survival function](survival-function.md)
4. [Survival analysis](survival-analysis-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-41/5/a/solution.md)
- [Survival selection in a heterogeneous population](survival-selection-in-a-heterogeneous-population.md)
