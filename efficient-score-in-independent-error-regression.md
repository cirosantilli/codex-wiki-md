# Efficient score in independent-error regression

↑ **Parent:** [Efficient score](efficient-score.md)

With unknown independent covariate and centered error distributions, take the regular [mean-preserving error tangent space](mean-preserving-error-tangent-space.md), let $h=\partial_\theta g_\theta$, $\rho=-f'/f$ and $\tau^2=E_f\varepsilon^2>0$. Under $E_f\rho=0$, $E_f(\varepsilon\rho)=1$ and finite second [moments](moment.md), [orthogonal projection](orthogonal-projection.md) removes $(E_vh)(\rho-\varepsilon/\tau^2)$ from $h\rho$. Thus the [efficient score](efficient-score.md) and [efficient information](efficient-information.md) are $\widetilde\ell=(h-E_vh)\rho+(E_vh)\varepsilon/\tau^2$ and $\widetilde I=\operatorname{Var}_v(h)E_f\rho^2+(E_vh)^2/\tau^2$. The reduction to $h\varepsilon/\tau^2$ is valid for a [normal distribution](normal-distribution.md) of errors or for constant $h$, but need not hold otherwise. Centered covariates and [logistic distribution](logistic-distribution.md) errors give the counterexample $\widetilde\ell=X\tanh(\varepsilon/2)$.

## ↑ Ancestors (8)

1. [Efficient score](efficient-score.md)
2. [Nuisance tangent space](nuisance-tangent-space.md)
3. [Semiparametric statistics](semiparametric-statistics.md)
4. [Statistical inference](statistical-inference-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-36/4/d/solution.md)
