# Cause-specific hazard to cumulative incidence formula

↑ **Parent:** [Cumulative incidence function](cumulative-incidence-function.md)

For absolutely continuous first-event time $T$ with event type $J$, the event-free [survivor function](survival-function.md) satisfies $S(t)=\exp(-\int_0^t\sum_jh_j(u)\,du)$. The [cause-specific hazard](cause-specific-hazard.md) definition gives unconditional event-type density $S(t)h_j(t)$, so $F_j(t)=\int_0^tS(u)h_j(u)\,du$. Consequently $\sum_jF_j(t)=1-S(t)$ for exhaustive disjoint causes. [Independent](independent-random-variables.md) latent cause times are unnecessary. Substituting $1-e^{-\int h_j}$ instead estimates a hypothetical net risk and generally overstates observed incidence.

## ↑ Ancestors (8)

1. [Cumulative incidence function](cumulative-incidence-function.md)
2. [Competing risks model](competing-risks-model.md)
3. [Competing risks](competing-risks.md)
4. [Survival analysis](survival-analysis-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-207/6/a/solution.md)
