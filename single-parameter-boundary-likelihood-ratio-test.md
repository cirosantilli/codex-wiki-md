# Single-parameter boundary likelihood-ratio test

↑ **Parent:** [Likelihood-ratio test](likelihood-ratio-test.md)

For a scalar parameter restricted to $\psi\ge0$, test $\psi=0$ against $\psi>0$ with identifiable interior [nuisance parameters](nuisance-parameter.md). A locally quadratic regular likelihood has an efficient null score $Z\sim N(0,1)$, and the constrained fit projects the unconstrained local maximizer onto the nonnegative half-line. Consequently

$$
2(\ell_{\rm full}-\ell_{\rm null})\Rightarrow(\max(0,Z))^2
\sim\tfrac12\delta_0+\tfrac12\chi^2_1.
$$

For a positive statistic, its asymptotic upper-tail [p-value](p-value.md) is half the ordinary one-degree chi-squared tail. Its 5% critical value is the 90th chi-squared percentile, approximately 2.7055. Additional boundary [nuisance parameters](nuisance-parameter.md) or nonidentified mixture parameters can change this law.

## ↑ Ancestors (8)

1. [Likelihood-ratio test](likelihood-ratio-test.md)
2. [Statistical hypothesis test](statistical-hypothesis-test.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
