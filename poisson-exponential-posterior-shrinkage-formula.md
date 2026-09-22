<h1 id="poisson-exponential-posterior-shrinkage-formula">Poisson–exponential posterior shrinkage formula</h1>

↑ **Parent:** [Gamma–Poisson hierarchical model](gamma-poisson-hierarchical-model.md)

For $Y_i\mid\theta_i\sim\operatorname{Poisson}(\theta_i)$ and $\theta_i\mid\psi\sim\operatorname{Exp}(\psi)$, a [scale-invariant prior](scale-invariant-prior.md) $d\psi/\psi$ induces the [Haldane prior](haldane-prior.md) on $\phi=(1+\psi)^{-1}$. Integrating out each local mean gives $p(y_i\mid\phi)=(1-\phi)\phi^{y_i}$. Thus $\phi\mid y\sim\operatorname{Beta}(s,n)$ for $s=\sum_i y_i>0$. The gamma [full conditional distribution](full-conditional-distribution.md) has mean $(y_i+1)\phi$, so the [tower property](law-of-total-expectation.md) gives $(y_i+1)s/(s+n)$, equal to the displayed [partial pooling](partial-pooling.md) formula. For $s=0$, the posterior is improper and this expectation is undefined.

## ↑ Ancestors (8)

1. [Gamma–Poisson hierarchical model](gamma-poisson-hierarchical-model.md)
2. [Hierarchical Bayesian model](hierarchical-bayesian-model.md)
3. [Bayesian statistics](bayesian-statistics.md)
4. [Statistical inference](statistical-inference-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-44/2/g/solution.md)
