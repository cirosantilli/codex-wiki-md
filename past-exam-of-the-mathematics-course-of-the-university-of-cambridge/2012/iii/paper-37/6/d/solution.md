<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Keep baseline covariates fixed and put $q=1-\pi$, $\mu_j=e^{\beta_0+\beta^Tx_i+\alpha_j}$, and $r=1/\tau$ for $\tau>0$. Integration of a Poisson count over the Gamma component gives

$$
g_j(y)=\frac{\Gamma(r+y)}{\Gamma(r)y!}
\left(\frac{r}{r+\mu_j}\right)^r
\left(\frac{\mu_j}{r+\mu_j}\right)^y,\qquad y=0,1,\ldots.
$$

This [negative binomial distribution](../../../../../../negative-binomial-distribution.md) has mean $\mu_j$ and [variance](../../../../../../variance-split.md) $\mu_j+\tau\mu_j^2$. Therefore the unconditional one-term distribution is the [zero-inflated negative binomial distribution](../../../../../../zero-inflated-negative-binomial-model.md)

$$
\boxed{\mathbb P(Y_{ij}=y)=\pi\mathbf1_{\{y=0\}}+qg_j(y).}
$$

In particular its zero probability is $\pi+q(1+\tau\mu_j)^{-1/\tau}$, not simply $\pi$. As $\tau\downarrow0$ this becomes a [Zero-inflated Poisson distribution](../../../../../../zero-inflated-poisson-distribution.md).

The mixing effect has $\mathbb Eb_i=q$, $\mathbb Eb_i^2=q(1+\tau)$ and $\operatorname{Var}(b_i)=q(\tau+\pi)$. The [law of total variance](../../../../../../law-of-total-variance.md) and [law of total covariance](../../../../../../law-of-total-covariance.md) now give

$$
\boxed{\begin{aligned}
\mathbb EY_{ij}&=q\mu_j,\\
\operatorname{Var}(Y_{ij})&=q\mu_j+q(\tau+\pi)\mu_j^2,\\
\operatorname{Cov}(Y_{ij},Y_{ik})&=q(\tau+\pi)\mu_j\mu_k,\qquad j\ne k.
\end{aligned}}
$$

Equivalently, for $\mu=(\mu_1,\mu_2,\mu_3)^T$, $\mathbb EY_i=q\mu$ and $\operatorname{Cov}(Y_i)=\operatorname{diag}(q\mu)+q(\tau+\pi)\mu\mu^T$. This also supplies raw second moments by adding $(\mathbb EY_i)(\mathbb EY_i)^T$. Dependence arises from both shared heterogeneity and shared structural zeros, even when the positive [random effect](../../../../../../random-effect.md) is constant.

The printed moment [variance](../../../../../../variance-split.md) matches the hierarchical [variance](../../../../../../variance-split.md) at the same parameter values, but its printed off-diagonal [covariance](../../../../../../covariance.md) is $\tau\mu_j\mu_k$. Equality would require $\tau=q(\tau+\pi)$, or $\pi(\tau-q)=0$. It is therefore false to claim that the two approaches consistently estimate all the same parameters in general.

The precise distinction is between consistency of mean ratios and identification of structural parameters. In the hierarchical model, with $m_j=q\mu_j$, both the quadratic [variance](../../../../../../variance-split.md) coefficient and the [covariance](../../../../../../covariance.md) coefficient in terms of the marginal mean are

$$
\kappa=\frac{\tau+\pi}{q},\qquad
\operatorname{Var}(Y_j)=m_j+\kappa m_j^2,\quad
\operatorname{Cov}(Y_j,Y_k)=\kappa m_jm_k.
$$

For the moment parameterization, writing its parameters as $\pi_Q,\tau_Q,q_Q=1-\pi_Q$, these coefficients are $A_Q=(\pi_Q+\tau_Q)/q_Q$ and $B_Q=\tau_Q/q_Q^2$. Its intercept is identifiable from the mean only as $\gamma_{0Q}=\beta_{0Q}+\log q_Q$. Matching the true first two moments demands $A_Q=B_Q=\kappa$. One solution always is

$$
\pi_Q=0,\qquad\tau_Q=\kappa,\qquad\beta_{0Q}=\beta_0+\log q.
$$

For $\kappa>1$ there is also a solution $q_Q=1/\kappa$, $\pi_Q=1-1/\kappa$, $\tau_Q=1/\kappa$, with the corresponding shifted intercept. Indeed eliminating $\tau_Q$ gives $\pi_Q(\tau_Q-q_Q)=0$. This is [moment aliasing in a shared zero-inflated count model](../../../../../../moment-aliasing-in-a-shared-zero-inflated-count-model.md): matching the moments does not identify the actual structural-zero probability.

For a concrete counterexample take $\pi=0.2,\tau=0.3$. Then $q=0.8$ and $\kappa=0.625$. The only admissible moment-matching choice is $\pi_Q=0,\tau_Q=0.625$, with an intercept shifted by $\log0.8$; it cannot recover the true structural-zero proportion 0.2. **Correct marginal means can give consistent term and baseline-covariate slopes with sandwich [standard errors](../../../../../../standard-error.md); they do not justify consistent estimation of the intended $\pi,\tau$, or latent intercept.** Nor does a mean-only estimating equation identify $\pi$ at all. Full-distribution inference provides information beyond these first two moments.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [6](../../6.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
