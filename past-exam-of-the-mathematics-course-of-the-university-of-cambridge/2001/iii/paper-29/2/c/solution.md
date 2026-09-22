<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For individual $i$, let $\pi_i=\pi_i(\psi)$, $q_i(t)$ be the known baseline [hazard function](../../../../../../hazard-function.md), and $r_i(t;\phi)$ the extra hazard. Put

$$
Q_i(t)=\int_0^tq_i(s)ds,\qquad R_i(t;\phi)=\int_0^tr_i(s;\phi)ds.
$$

The class-specific [survival functions](../../../../../../survival-function.md) are $e^{-Q_i(t)}$ and $e^{-Q_i(t)-R_i(t)}$. Consequently the unconditional survivor and failure density are

$$
F_i(t)=e^{-Q_i(t)}[\pi_i+(1-\pi_i)e^{-R_i(t)}],
$$



$$
f_i(t)=e^{-Q_i(t)}[\pi_iq_i(t)+(1-\pi_i)(q_i(t)+r_i(t))e^{-R_i(t)}].
$$

Mixture [probabilities](../../../../../../probability.md) must be summed before taking a logarithm; a weighted average of class log-likelihoods would be a different, complete-data calculation. Substitution into the right-censored [survival likelihood](../../../../../../survival-likelihood.md) gives

$$
\boxed{\begin{aligned}
\ell(\phi,\psi)=\sum_i\bigl[&-Q_i(x_i)
+v_i\log\{\pi_iq_i(x_i)+(1-\pi_i)[q_i(x_i)+r_i(x_i;\phi)]e^{-R_i(x_i;\phi)}\}\\
&+(1-v_i)\log\{\pi_i+(1-\pi_i)e^{-R_i(x_i;\phi)}\}\bigr]+\text{constant}.
\end{aligned}}
$$

Equivalently, this [additive excess-hazard mixture likelihood](../../../../../../additive-excess-hazard-mixture-likelihood.md) has contribution

$$
L_i=e^{-Q_i(x_i)}\{\pi_iq_i(x_i)^{v_i}+(1-\pi_i)[q_i(x_i)+r_i(x_i)]^{v_i}e^{-R_i(x_i)}\}.
$$

Here $q_i$ and $q_i+r_i$ must be nonnegative hazards. The factor $-Q_i(x_i)$ can be dropped when maximizing over $\phi,\psi$ because $q_i$ is known. Factoring out [censoring](../../../../../../censoring-statistics.md) presumes a common parameter-free [censoring](../../../../../../censoring-statistics.md) mechanism independent of failure and latent class, conditional on the observed [covariates](../../../../../../covariate.md); unmodelled class-specific [censoring](../../../../../../censoring-statistics.md) would change these mixture contributions.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
