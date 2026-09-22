<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Introduce a latent indicator $Z_i=1$ for a structural zero. In this parametrization $P(Z_i=1)=\pi_i$, and conditional on $Z_i=0$ the response has a [Poisson distribution](../../../../../../poisson-distribution.md) with mean $\mu_i$. The [zero-inflated Poisson regression](../../../../../../zero-inflated-poisson-regression.md) uses

$$
\log\mu_i=\beta_0+\beta_1x_i,\qquad
\log\frac{\pi_i}{1-\pi_i}=\gamma_0+\gamma_1x_i.
$$

Its observed [probability mass function](../../../../../../probability-mass-function.md) is $\pi_i+(1-\pi_i)e^{-\mu_i}$ at zero and $(1-\pi_i)e^{-\mu_i}\mu_i^{y_i}/y_i!$ at a positive count. The zero-mixing probability here is explicitly $\pi_i$; it is distinct from the weight of the count component.

For the [expectation-maximization algorithm](../../../../../../expectation-maximization-algorithm.md), start with positive $\mu_i$ and $0<\pi_i<1$. At iteration $k$, the E-step computes

$$
\boxed{\tau_i^{(k)}=E(Z_i\mid y_i)=
\begin{cases}
\displaystyle\frac{\pi_i^{(k)}}{\pi_i^{(k)}+(1-\pi_i^{(k)})e^{-\mu_i^{(k)}}},&y_i=0,\\
0,&y_i>0.
\end{cases}}
$$

This distinguishes structural zeros from Poisson-generated zeros. Up to terms independent of the new parameters, the expected complete-data [log-likelihood](../../../../../../log-likelihood.md) is

$$
Q=\sum_i\{\tau_i\log\pi_i+(1-\tau_i)\log(1-\pi_i)\}
+\sum_i(1-\tau_i)\{y_i\log\mu_i-\mu_i\}.
$$

It separates into a fractional-response logistic fit and a weighted Poisson fit. Because treatment is binary, each component is saturated over its two treatment groups, so the M-step has closed forms.

For $j=0,1$, let $I_j=\{i:x_i=j\}$, $n_j=|I_j|$, $S_j=\sum_{i\in I_j}\tau_i$, and $C_j=\sum_{i\in I_j}y_i$. The M-step score equations give

$$
\boxed{\pi_j^{(k+1)}=\frac{S_j}{n_j},\qquad
\mu_j^{(k+1)}=\frac{C_j}{n_j-S_j}.}
$$

Here $\sum(1-\tau_i)y_i=C_j$, since every positive count has $\tau_i=0$. The explicit coefficient updates are

$$
\boxed{\begin{aligned}
\gamma_0^{(k+1)}&=\operatorname{logit}(\pi_0^{(k+1)}),\\
\gamma_1^{(k+1)}&=\operatorname{logit}(\pi_1^{(k+1)})-\gamma_0^{(k+1)},\\
\beta_0^{(k+1)}&=\log\mu_0^{(k+1)},\\
\beta_1^{(k+1)}&=\log\mu_1^{(k+1)}-\beta_0^{(k+1)}.
\end{aligned}}
$$

Iterate the E- and M-steps until the observed [log-likelihood](../../../../../../log-likelihood.md) and parameter estimates stabilize. This is the [EM algorithm for zero-inflated Poisson regression](../../../../../../em-algorithm-for-zero-inflated-poisson-regression.md) with explicit binary-group updates; merely naming two regression routines would not supply these expressions. Both treatment groups must be represented for both contrasts to be identifiable. Zero fitted group means or endpoint mixing probabilities are boundary solutions, interpreted through limits of the log or logit coefficients. As with other [mixture models](../../../../../../mixture-model.md), multiple starts help distinguish competing stationary solutions; EM increases the likelihood but does not guarantee a global maximum from an arbitrary start.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
