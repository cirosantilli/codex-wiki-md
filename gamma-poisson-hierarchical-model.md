<h1 id="gamma-poisson-hierarchical-model">Gamma–Poisson hierarchical model</h1>

↑ **Parent:** [Hierarchical Bayesian model](hierarchical-bayesian-model.md)

A [Gamma–Poisson hierarchical model](gamma-poisson-hierarchical-model.md) uses $Y_i\mid\theta_i\sim\operatorname{Poisson}(t_i\theta_i)$, $\theta_i\mid b\sim\operatorname{Gamma}(a,b)$, and $b\sim\operatorname{Gamma}(c,r)$, with [gamma distributions](gamma-distribution.md) in shape-rate convention. [Conditional independence](conditional-independence.md) gives [full conditional distributions](full-conditional-distribution.md) $\theta_i\mid b,y\sim\operatorname{Gamma}(a+y_i,b+t_i)$ and $b\mid\theta,y\sim\operatorname{Gamma}(c+na,r+\sum_i\theta_i)$.

**Table of contents**

- [Poisson–exponential posterior shrinkage formula](poisson-exponential-posterior-shrinkage-formula.md)
- [Gamma-integrated baseline Poisson likelihood](gamma-integrated-baseline-poisson-likelihood.md)

## ↑ Ancestors (7)

1. [Hierarchical Bayesian model](hierarchical-bayesian-model.md)
2. [Bayesian statistics](bayesian-statistics.md)
3. [Statistical inference](statistical-inference-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Gamma–Poisson hierarchical model](gamma-poisson-hierarchical-model.md)
- [Paired Poisson conditional likelihood](paired-poisson-conditional-likelihood.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-44/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-46/1/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-216/3/a/solution.md)
