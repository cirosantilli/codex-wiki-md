# Grouped proportional-hazards model

↑ **Parent:** [Proportional hazards model](proportional-hazards-model.md)

When event times are observed only in intervals and the [covariate](covariate.md) vector is constant within an interval, a [proportional hazards model](proportional-hazards-model.md) gives $p_{ij}=1-\exp[-\Delta H_{0j}\exp(\beta^Tz_i)]$. Thus the interval event probability has a complementary log-log link, with $\alpha_j=\log\Delta H_{0j}$ an interval-specific intercept. The person-period Bernoulli [likelihood](likelihood-function.md) models several events in one interval directly, without inventing their order. It needs appropriate [independent censoring](independent-censoring.md) assumptions and a consistent account of interval entry and observation.

## ↑ Ancestors (6)

1. [Proportional hazards model](proportional-hazards-model.md)
2. [Survival analysis](survival-analysis-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-41/3/b/solution.md)
