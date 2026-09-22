<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $E(t)=\delta A/\delta x(t)$ for the [functional derivative](../../../../../../functional-derivative.md) of the [action](../../../../../../action.md). Under [time reversal in classical mechanics](../../../../../../time-reversal-in-classical-mechanics.md), $\dot x$ changes sign whereas $E$ is even by assumption. Thus the forward and reversed [Gaussian white noise](../../../../../../gaussian-white-noise.md) histories associated with the same geometric path are

$$
f_F=\zeta\dot x-E,\qquad f_B=-\zeta\dot x-E,
\qquad f_F^2-f_B^2=-4\zeta\dot xE.
$$

The [Onsager--Machlup path probability](../../../../../../onsager-machlup-path-probability.md) therefore gives

$$
\log\frac{\mathbb P_F}{\mathbb P_B}
=-\frac1{2\sigma^2}\int_{t_1}^{t_2}(f_F^2-f_B^2)\,dt,
\qquad
\boxed{\frac{\mathbb P_F}{\mathbb P_B}
=\exp\!\left[\frac{2\zeta}{\sigma^2}\int_{t_1}^{t_2}\dot x\frac{\delta A}{\delta x(t)}\,dt\right]}.
$$

Here the [path probabilities](../../../../../../path-probability.md) are densities conditional on their respective initial states; they are not separately normalized bridges conditioned on both endpoints. The noise-to-path [Jacobian determinant](../../../../../../jacobian-determinant.md) must be treated with a consistent discretization: it cancels when it is invariant under [time reversal in classical mechanics](../../../../../../time-reversal-in-classical-mechanics.md). This is the usual additive-noise [Langevin dynamics](../../../../../../langevin-dynamics.md) convention, including a constant-mass [Underdamped Langevin dynamics](../../../../../../underdamped-langevin-dynamics.md) or the [time-reversal invariance of a path Jacobian](../../../../../../time-reversal-invariance-of-a-path-jacobian.md) in midpoint [overdamped Langevin dynamics](../../../../../../overdamped-langevin-dynamics.md). A completely arbitrary velocity-dependent [Lagrangian](../../../../../../lagrangian.md) would require specifying that measure rather than deducing its cancellation solely from the parity of $E$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 344](../../../paper-344-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
