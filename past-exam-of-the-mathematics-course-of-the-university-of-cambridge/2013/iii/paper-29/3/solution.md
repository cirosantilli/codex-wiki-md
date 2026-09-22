<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For the [Box-Muller transform](../../../../../box-muller-transform.md), draw [independent](../../../../../independent-random-variables.md) $U,V$ from the [uniform distribution](../../../../../continuous-uniform-distribution.md) on $(0,1)$ and set

$$
R=\sqrt{-2\log U},\qquad \Theta=2\pi V,\qquad
\boxed{G_1=R\cos\Theta,\quad G_2=R\sin\Theta.}
$$

The radial density is $r e^{-r^2/2}$ for $r>0$, with an [independent](../../../../../independent-random-variables.md) uniform angle. The polar-to-Cartesian [Jacobian determinant](../../../../../jacobian-determinant.md) is $r$, so the joint density of $(G_1,G_2)$ is

$$
\frac1{2\pi}\exp\left[-\frac{g_1^2+g_2^2}{2}\right]
=\frac{e^{-g_1^2/2}}{\sqrt{2\pi}}\frac{e^{-g_2^2/2}}{\sqrt{2\pi}}.
$$

This factorization proves that both outputs have the [standard normal distribution](../../../../../standard-normal-distribution.md) and are [independent](../../../../../independent-random-variables.md). Repeating the [Box-Muller transform](../../../../../box-muller-transform.md) with fresh [independent](../../../../../independent-random-variables.md) uniform pairs gives [independent](../../../../../independent-random-variables.md) normal outputs; discard one extra output if the desired sample size is odd.

For the prescribed binary probabilities, generate [independent](../../../../../independent-random-variables.md) standard normal values $G_i$ in this way and use

$$
\boxed{Y_i=\mathbf1_{\{G_i\leq x_i\}}.}
$$

The [standard normal distribution function](../../../../../standard-normal-distribution-function.md) gives $\mathbb P(Y_i=1)=\Phi(x_i)$, and [independence](../../../../../independent-random-variables.md) is preserved because each threshold uses a different [independent](../../../../../independent-random-variables.md) normal value.

For the [probit regression](../../../../../probit-model.md) posterior, introduce latent variables

$$
Z_i=\beta x_i+G_i,\qquad Y_i=\mathbf1_{\{Z_i>0\}}.
$$

Given $\beta$, these are [independent](../../../../../independent-random-variables.md) $N(\beta x_i,1)$ variables, and normal symmetry gives $\mathbb P(Z_i>0\mid\beta)=\Phi(\beta x_i)$. Thus this [data augmentation](../../../../../data-augmentation.md) has exactly the observed binary [likelihood](../../../../../likelihood-function.md). With the specified normal [prior distribution](../../../../../prior-probability.md), the augmented joint [posterior](../../../../../bayesian-posterior.md) is proportional to

$$
\exp\left[-\frac{\beta^2}{2}-\frac12\sum_i(z_i-\beta x_i)^2\right]
\prod_i\mathbf1_{\{z_i>0\text{ if }y_i=1;\ z_i\leq0\text{ if }y_i=0\}}.
$$

The [latent-normal Gibbs sampler for probit regression](../../../../../latent-normal-gibbs-sampler-for-probit-regression.md) alternates two blocks. First, given the current $\beta$, draw each $Z_i$ independently from its [truncated normal distribution](../../../../../truncated-normal-distribution.md), namely $N(\beta x_i,1)$ restricted to the sign fixed by $y_i$. One exact method is to use the [Box-Muller transform](../../../../../box-muller-transform.md) for $G_i$, form $\beta x_i+G_i$, and reject until the sign is correct. The probability of success is positive at every finite parameter value, so the method is valid, although it can be slow for a rare sign.

For direct [sign-truncated normal sampling](../../../../../sign-truncated-normal-sampling.md), let $\mu_i=\beta x_i$, $a_i=\Phi(-\mu_i)$ and draw $U_i\sim\operatorname{Unif}(0,1)$. An [inverse transform sampling](../../../../../inverse-transform-sampling.md) implementation is

$$
\boxed{Z_i=\mu_i+\Phi^{-1}(a_i+(1-a_i)U_i)\quad(y_i=1),\qquad
Z_i=\mu_i+\Phi^{-1}(a_iU_i)\quad(y_i=0).}
$$

Use suitable tail or survival-function evaluations when floating-point probabilities approach zero or one; the rejection construction remains a valid alternative.

Second, completing the square in $\beta$ yields its [full conditional distribution](../../../../../full-conditional-distribution.md):

$$
\boxed{\beta\mid z,y\sim N\left(\frac{\sum_i x_i z_i}{1+\sum_i x_i^2},\ \frac1{1+\sum_i x_i^2}\right).}
$$

Generate a fresh standard normal value by the [Box-Muller transform](../../../../../box-muller-transform.md), multiply by the conditional standard deviation, and add the conditional mean. Start from any finite $\beta$, alternate these steps, discard an initial transient and use the retained $\beta$ values to approximate its [posterior distribution](../../../../../bayesian-posterior.md). These are dependent [Markov chain Monte Carlo](../../../../../markov-chain-monte-carlo.md) samples, rather than [independent](../../../../../independent-random-variables.md) posterior draws. Each block is an exact [Gibbs sampling](../../../../../gibbs-sampler.md) update for the augmented [posterior](../../../../../bayesian-posterior.md), whose marginal in $\beta$ is the requested posterior.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 29](../../paper-29-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
