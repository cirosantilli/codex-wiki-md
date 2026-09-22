<h1 id="4/h/solution">Solution</h1>

↑ **Parent:** [H](../h.md)

Let $T_{0i}=e^{\mu_{0i}}$ denote the child's latent true baseline titre. With the constrained slopes, the conditional mean of log follow-up titre is

$$
\mu_i(t)=\alpha_i-\log t+\mu_{0i}.
$$

Exponentiating this log-scale center gives

$$
\boxed{\frac{e^{\mu_i(t)}}{T_{0i}}=\frac{e^{\alpha_i}}t.}
$$

Thus the conditional median, or geometric-mean titre, expressed as a fraction of true baseline titre, decays inversely with elapsed time; the child-specific intercept supplies the proportionality constant. It is not an exponential decay in time, and the formula is a follow-up model for $t>0$, not an extrapolation to the immunisation instant $t=0$.

For the arithmetic conditional mean, the [lognormal distribution](../../../../../../log-normal-distribution.md) correction gives

$$
\frac{\mathbb E\{T_i(t)\mid\alpha_i,\mu_{0i},\sigma^2\}}{T_{0i}}
=\frac{e^{\alpha_i+\sigma^2/2}}t.
$$

The correction changes the constant but not the inverse-time dependence when the residual variance is constant. Averaging over random intercepts similarly preserves the time factor whenever the required expectation is finite.

## ↑ Ancestors (11)

1. [H](../h.md)
2. [4](../../4.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
