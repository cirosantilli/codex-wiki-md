<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Under the corrected hypothesis, $N_t=X_t-1$ is a [continuous local martingale](../../../../../../continuous-local-martingale.md) with $N_0=0$, $[N]_t=A_t=\int_0^te^{2B_s}ds$, and $A_\infty=\infty$ [almost surely](../../../../../../almost-sure-convergence.md). The [Dambis-Dubins-Schwarz theorem](../../../../../../dambis-dubins-schwarz-theorem.md) states that, for such a process,

$$
\tau_u=\inf\{t\geq0:[N]_t>u\},\qquad W_u=N_{\tau_u}
$$

defines a standard [Brownian motion](../../../../../../brownian-motion-split.md) relative to the [filtration](../../../../../../filtration-probability-theory.md) $\mathcal F_{\tau_u}$, and $N_t=W_{[N]_t}$. The divergence of the [quadratic variation](../../../../../../quadratic-variation.md) ensures every $\tau_u$ is finite, so no extension of the [probability space](../../../../../../probability-space.md) is needed. Here $A$ is continuous and strictly increasing because its derivative is $e^{2B_t}>0$, so the inverse is particularly straightforward. Consequently,

$$
\boxed{X_t=1+W_{\int_0^te^{2B_s}ds}.}
$$

The constructed [Brownian motion](../../../../../../brownian-motion-split.md) need not be independent of its random clock. Under the literal PDF assumptions $X$ need not be a [local martingale](../../../../../../local-martingale.md), as the counterexample in part (a) shows, so this [Dambis-Dubins-Schwarz theorem](../../../../../../dambis-dubins-schwarz-theorem.md) conclusion cannot be asserted without the correction.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
