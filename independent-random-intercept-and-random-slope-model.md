# Independent random-intercept and random-slope model

↑ **Parent:** [Gaussian linear mixed model](gaussian-linear-mixed-model.md)

Independent Gaussian [random intercepts](random-intercept.md) $u_j$ and [random slopes](random-slope.md) $v_j$ give marginal within-group [covariance](covariance.md) $\tau_0^2+\tau_1^2t_{ij}t_{kj}+\sigma^2\mathbf1_{\{i=k\}}$. In `lme4`, separate terms `(1 | group)` and `(0 + x | group)` impose zero intercept-slope covariance; `(1 + x | group)` estimates it. This independence restriction depends on the predictor origin: replacing $t$ by $t-c$ transforms the intercept effect to $u_j+cv_j$, generally correlated with $v_j$.

## ↑ Ancestors (9)

1. [Gaussian linear mixed model](gaussian-linear-mixed-model.md)
2. [Generalized linear mixed model](generalized-linear-mixed-model.md)
3. [Generalized linear model](generalized-linear-model.md)
4. [Statistical modelling](statistical-modelling-split.md)
5. [Statistical model](statistical-model-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Correlated random-intercept and random-slope model](correlated-random-intercept-and-random-slope-model.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-206/6/a/solution.md)
