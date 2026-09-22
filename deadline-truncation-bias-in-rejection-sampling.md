# Deadline truncation bias in rejection sampling

↑ **Parent:** [Rejection sampling](rejection-sampling.md)

Stopping after a fixed number of [rejection sampling](rejection-sampling.md) proposals preserves the target law of accepted labels, conditional on the number accepted. Stopping instead after a fixed amount of elapsed computing time can change the finite-sample law if processing costs depend on the proposed state. The [deadline](deadline-truncation-bias-in-rejection-sampling.md) may censor precisely the expensive states.

For an exact counterexample, let both target and proposal be uniform on two states, so every proposal is accepted. Let processing cost be one time unit for the first state and two for the second. Stop between one and two units and retain only finished proposals. Conditional on obtaining an output, the first state is the only possible value, despite its target probability being one half. This proves that a runtime cutoff need not be an unbiased stopping rule for the realized finite output. It does not imply asymptotic [bias](bias-of-an-estimator.md) of the indefinitely growing completed sequence; it identifies a finite-horizon censoring effect.

## ↑ Ancestors (6)

1. [Rejection sampling](rejection-sampling.md)
2. [Monte Carlo method](monte-carlo-method-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Deadline truncation bias in rejection sampling](deadline-truncation-bias-in-rejection-sampling.md)
- [Solution](past-exam-of-the-probability-statistics-and-options-ii-course-of-the-university-of-oxford/2009/s/s2/e/solution.md)
