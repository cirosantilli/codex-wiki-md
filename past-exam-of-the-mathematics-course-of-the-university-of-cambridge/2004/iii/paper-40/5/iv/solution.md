<h1 id="5/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

The full conditional log [probability density functions](../../../../../../probability-density-function.md) of the effects are, up to constants,

$$
\begin{aligned}
\ell_\alpha(a_2)&=Ra_2-I\theta(1+e^{b_2})e^{a_2}-\frac{a_2^2}{2\sigma_1^2},\\
\ell_\beta(b_2)&=Cb_2-I\theta(1+e^{a_2})e^{b_2}-\frac{b_2^2}{2\sigma_2^2}.
\end{aligned}
$$

These are [Gaussian-prior Poisson log-effect conditional](../../../../../../gaussian-prior-poisson-log-effect-conditional.md) [probability density functions](../../../../../../probability-density-function.md). The exponential [likelihood](../../../../../../likelihood-function.md) term prevents a standard [normal distribution](../../../../../../normal-distribution.md) conjugate update. A [Metropolis-within-Gibbs algorithm](../../../../../../metropolis-within-gibbs-algorithm.md) conveniently updates one effect at a time without computing its conditional [normalizing constant](../../../../../../normalizing-constant.md).

For example, propose $a_2'=a_2+s_\alpha Z$ with $Z\sim N(0,1)$, and accept with

$$
\boxed{\min\{1,\exp(\ell_\alpha(a_2')-\ell_\alpha(a_2))\}.}
$$

Use an analogous [normal distribution](../../../../../../normal-distribution.md) random-walk proposal for $b_2$. The proposal is symmetric and lives on the appropriate unrestricted real parameter space, so no proposal ratio is needed. It makes local moves compatible with a unimodal conditional [probability density function](../../../../../../probability-density-function.md). Tune the positive scale in a pilot or freeze it after warm-up; a scale far too large causes rejection and a scale far too small moves slowly.

A useful scale can be inferred from the conditional curvature: $\ell_\alpha''(a_2)=-I\theta(1+e^{b_2})e^{a_2}-\sigma_1^{-2}<0$, with the analogous formula for $b_2$. A normal proposal near the conditional mode with [variance](../../../../../../variance-split.md) approximately $-1/\ell''$ is another sensible choice, but an asymmetric or state-dependent proposal must include its full reverse-to-forward proposal-density ratio. Metropolis–Hastings is convenient, not logically mandatory; these [concave](../../../../../../concave-function.md) conditionals also admit other specialized samplers.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [5](../../5.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
