<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the stated scale-parameterisation of the [Weibull distribution](../../../../../../weibull-distribution.md), its incubation [survivor function](../../../../../../survival-function.md) is $S_T(s)=\exp[-(s/\lambda)^\kappa]$ for $s\geq0$, with $\lambda,\kappa>0$. The continuous [back-calculation of infection incidence](../../../../../../back-calculation-of-infection-incidence.md) equation becomes

$$
\boxed{\mu(t)=\int_0^\infty h(t-s)\frac\kappa\lambda
\left(\frac s\lambda\right)^{\kappa-1}
\exp\!\left[-\left(\frac s\lambda\right)^\kappa\right]ds.}
$$

Set $h(t-s)=0$ before the infection process's start if one is specified. For the equal-width endpoint approximation, integrate the incubation density over each delay bin:

$$
q_\ell(\lambda,\kappa)
=\exp\!\left[-\left(\frac{(\ell-1)\Delta}\lambda\right)^\kappa\right]
-\exp\!\left[-\left(\frac{\ell\Delta}\lambda\right)^\kappa\right].
$$

Thus **the discrete Weibull equation is**

$$
\boxed{\mu_k(\theta,\lambda,\kappa)
=\sum_{i<k}h_i(\theta)q_{k-i}(\lambda,\kappa).}
$$

For unequal intervals replace $q_{k-i}$ by $S_T(\max\{0,t_{k-1}-t_i\})-S_T(\max\{0,t_k-t_i\})$. These are probabilities, not point evaluations of a density; no additional factor of $\Delta$ is needed after bin integration.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
