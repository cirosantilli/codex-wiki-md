# Piecewise-exponential mortality comparison

↑ **Parent:** [Piecewise-exponential survival model](piecewise-exponential-survival-model.md)

For specified exposure periods with constant death [hazard functions](hazard-function.md) $h_k$, the [integrated hazard](cumulative-hazard-function.md) through the endpoint is $\sum_kh_k\Delta t_k$. The displayed event [probability](probability.md) follows from the [survivor function](survival-function.md) identity. For different latent exposure schedules mixed with probabilities $w_j$, average the schedule-specific probabilities, $\sum_jw_j(1-e^{-H_j})$, rather than exponentiating the average [integrated hazard](cumulative-hazard-function.md). When the hazards are small, $1-e^{-H_j}\simeq H_j$ gives a [person-time](person-time.md) approximation. A comparison must specify the entire custody or treatment schedule; later changes to exposure cannot be inferred from an endpoint rate alone.

## ↑ Ancestors (6)

1. [Piecewise-exponential survival model](piecewise-exponential-survival-model.md)
2. [Survival analysis](survival-analysis-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
