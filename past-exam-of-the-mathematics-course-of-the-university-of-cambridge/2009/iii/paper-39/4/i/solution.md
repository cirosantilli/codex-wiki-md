<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Treat the two-point prior for $\alpha$ as independent of the driving [Brownian motion](../../../../../../brownian-motion-split.md). On a partition $0=t_0<\cdots<t_n=t$, conditionally on $\alpha=\pm a$, the increments of $X$ are independent [normal distributions](../../../../../../normal-distribution.md) with means $\pm a\Delta t_j$ and variances $\Delta t_j$. Their [likelihood ratio](../../../../../../likelihood-ratio.md) is

$$
\frac{L_+}{L_-}
=\prod_{j=1}^n\exp\left[\frac{(\Delta X_j+a\Delta t_j)^2-(\Delta X_j-a\Delta t_j)^2}{2\Delta t_j}\right]
=\exp\left(2a\sum_{j=1}^n\Delta X_j\right)
=e^{2aX_t}.
$$

Thus every partition containing $t$ gives the same [Bayesian posterior](../../../../../../bayesian-posterior.md), depending only on the endpoint. Refine partitions through a dense set of observation times. Continuity makes their increasing observation fields generate the full path field $\mathcal X_t$, and convergence of bounded [conditional expectations](../../../../../../conditional-expectation.md) preserves that [Bayesian posterior](../../../../../../bayesian-posterior.md). Equal prior probabilities and the [Bayes' theorem](../../../../../../bayes-theorem.md) consequently give

$$
\boxed{q_t=P(\alpha=a\mid\mathcal X_t)=\frac{e^{aX_t}}{e^{aX_t}+e^{-aX_t}}.}
$$

Its conditional mean [drift](../../../../../../drift-coefficient.md) is

$$
E[\alpha\mid\mathcal X_t]=a(2q_t-1)=a\tanh(aX_t)=h(X_t).
$$

This is the [binary Brownian drift filter](../../../../../../binary-brownian-drift-filter.md).

Define the observed [innovation process](../../../../../../innovation-process.md)

$$
\widehat W_t=X_t-\int_0^t h(X_u)du.
$$

It is continuous and adapted to $\mathcal X_t$. For $s<t$, independence of future [Brownian motion](../../../../../../brownian-motion-split.md) increments from the past and the latent [drift](../../../../../../drift-coefficient.md) gives

$$
E[X_t-X_s\mid\mathcal X_s]=(t-s)E[\alpha\mid\mathcal X_s].
$$

For every $u\geq s$, the tower property of [conditional expectation](../../../../../../conditional-expectation.md) gives

$$
E[h(X_u)\mid\mathcal X_s]
=E\bigl[E[\alpha\mid\mathcal X_u]\mid\mathcal X_s\bigr]
=E[\alpha\mid\mathcal X_s].
$$

Since $|h|\leq a$, conditional integration is justified. Subtracting the integrated identities shows $E[\widehat W_t-\widehat W_s\mid\mathcal X_s]=0$. Thus $\widehat W$ is a square-integrable [martingale](../../../../../../martingale-split.md). Subtracting a continuous [finite variation](../../../../../../total-variation-of-a-function.md) process does not change [quadratic variation](../../../../../../quadratic-variation.md), so $[\widehat W]_t=[X]_t=[W]_t=t$. The [Lévy characterization of Brownian motion](../../../../../../levy-characterization-of-brownian-motion.md) now proves that $\widehat W$ is a [Brownian motion](../../../../../../brownian-motion-split.md) in the observation [filtration](../../../../../../filtration-probability-theory.md). Therefore

$$
\boxed{dX_t=d\widehat W_t+a\tanh(aX_t)dt.}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
