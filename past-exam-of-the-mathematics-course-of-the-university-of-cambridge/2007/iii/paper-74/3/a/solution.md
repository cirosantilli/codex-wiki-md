<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\mu_i=\langle X_i\rangle$. Applying the [Markov jump-process generator](../../../../../../markov-jump-process-generator.md) to either coordinate gives the exact [moment equations](../../../../../../moment-equation.md)

$$
\boxed{\dot\mu_1=\lambda-\beta\mu_1-C\langle X_1X_2\rangle,\qquad
\dot\mu_2=\lambda-\beta\mu_2-C\langle X_1X_2\rangle.}
$$

In each equation the joint reaction removes one molecule, at [reaction propensity function](../../../../../../reaction-propensity-function.md) $CX_1X_2$. Because the two reactants are different [chemical species](../../../../../../chemical-species.md), the propensity uses their product; no same-species factorial correction is needed. The exact identity $\langle X_1X_2\rangle=\mu_1\mu_2+\operatorname{Cov}(X_1,X_2)$ shows explicitly where the equations fail to close. Neglecting this covariance relative to the product of means is the small-fluctuation [moment closure](../../../../../../moment-closure.md). It gives the [mean-field joint removal of two chemical species](../../../../../../mean-field-joint-removal-of-two-chemical-species.md):

$$
\boxed{\dot\mu_1\approx\lambda-\beta\mu_1-C\mu_1\mu_2,\qquad
\dot\mu_2\approx\lambda-\beta\mu_2-C\mu_1\mu_2.}
$$

The difference equation $d(\mu_1-\mu_2)/dt=-\beta(\mu_1-\mu_2)$ actually holds exactly as well as after closure, because both the constant production and the joint removal terms cancel. The nonlinear [moment closure](../../../../../../moment-closure.md) will be used for the subsequent [phase plane](../../../../../../phase-plane.md) and stationary [linear noise approximation](../../../../../../linear-noise-approximation.md) calculations, as requested.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 74](../../../paper-74-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
