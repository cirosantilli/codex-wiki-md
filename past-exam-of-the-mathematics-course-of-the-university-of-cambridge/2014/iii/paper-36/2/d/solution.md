<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Take the latent autoregression as the scalar state $S_t$. A [state-space model](../../../../../../state-space-model-time-series.md) is

$$
\boxed{\text{state: }S_t=\phi S_{t-1}+Z_t,\qquad\text{observation: }Y_t=S_t+W_t.}
$$

The transition and observation matrices are both scalar, $F=\phi$, $H=1$. State-noise [variance](../../../../../../variance-split.md) is $Q=\sigma_z^2$, observation-noise [variance](../../../../../../variance-split.md) is $R=\sigma_w^2$, and the cross-noise [covariance](../../../../../../covariance.md) is zero at every pair of times.

A complete stationary initialization is

$$
S_0=\sum_{j\geq0}\phi^jZ_{-j},\qquad\mathbb ES_0=0,\qquad\operatorname{Var}(S_0)=\frac{\sigma_z^2}{1-\phi^2}.
$$

It is orthogonal to future state noise and to all observation noise. This is the [stationary initialization of a scalar linear state-space model](../../../../../../stationary-initialization-of-a-scalar-linear-state-space-model.md). This specifies the initial state in terms of the actual given two-sided [white noise](../../../../../../white-noise.md) sequence, as well as its second-order law; simply starting from zero would give transient rather than stationary observations.

If a Gaussian state-space specification is intended, the complete specialization is $S_0\sim N(0,Q/(1-\phi^2))$, independent of the future iid Gaussian state and observation noises, themselves independent with variances $Q,R$. Under the printed assumptions alone, Gaussian distributions and independence cannot be deduced from [white noise](../../../../../../white-noise.md) orthogonality; the equations and stationary-series initialization above give the exact second-order representation without adding them.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
