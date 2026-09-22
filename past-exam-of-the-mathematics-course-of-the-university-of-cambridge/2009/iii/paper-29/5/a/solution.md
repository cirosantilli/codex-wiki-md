<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Apply the [Itô formula](../../../../../../ito-s-lemma.md) to $Y_t=e^{B_t+t/2}$. The time derivative contributes $Y_tdt/2$, and the quadratic-variation correction contributes another $Y_tdt/2$. Thus

$$
\boxed{dY_t=Y_t\,dB_t+Y_t\,dt,\qquad Y_0=1.}
$$

Both the drift $b(y)=y$ and diffusion coefficient $\sigma(y)=y$ are globally Lipschitz. The [global existence theorem for stochastic differential equations with Lipschitz coefficients](../../../../../../global-existence-theorem-for-stochastic-differential-equations-with-lipschitz-coefficients.md) gives a unique [strong stochastic solution](../../../../../../strong-solution-of-a-stochastic-differential-equation.md) for a fixed driving [Brownian motion](../../../../../../brownian-motion-split.md) and initial value; in particular [pathwise uniqueness](../../../../../../pathwise-uniqueness.md) holds. The explicit solution is strictly positive.

Write $N_t=\int_0^tY_s\,dB_s$. This is a [continuous local martingale](../../../../../../continuous-local-martingale.md) with

$$
[N]_t=H_t=\int_0^tY_s^2ds=\int_0^te^{2B_s+s}ds.
$$

The [strong law for Brownian motion](../../../../../../strong-law-for-brownian-motion.md) gives $B_t/t\to0$ almost surely, so $\log Y_t/t\to1/2$, $Y_t\to\infty$, and $H_t\to\infty$. The [Dambis-Dubins-Schwarz theorem](../../../../../../dambis-dubins-schwarz-theorem.md) therefore supplies a [Brownian motion](../../../../../../brownian-motion-split.md) $\beta$ in the inverse-clock filtration with $N_t=\beta_{H_t}$ for all $t$. Finally $dH_s=Y_s^2ds$, hence $Y_sds=Y_s^{-1}dH_s$. Integrating the stochastic equation gives

$$
\boxed{Y_t=1+\beta_{H_t}+\int_0^t\frac1{Y_s}\,dH_s.}
$$

The infinite clock lifetime verifies that this [Brownian motion](../../../../../../brownian-motion-split.md) is defined for every nonnegative clock time without an additional extension.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
