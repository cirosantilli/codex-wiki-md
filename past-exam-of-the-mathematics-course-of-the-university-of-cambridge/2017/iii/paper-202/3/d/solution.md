<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Define a [probability measure](../../../../../../probability-measure.md) on the same full measurable space by

$$
\boxed{\frac{d\mathbb P^T}{d\mathbb P}=Z_T=\exp(\mu B_T-\mu^2T/2).}
$$

The [Radon-Nikodym derivative](../../../../../../radon-nikodym-derivative.md) is positive and has [expectation](../../../../../../expected-value.md) one, so this is a [probability measure](../../../../../../probability-measure.md) and even equivalent to $\mathbb P$, in particular $\mathbb P^T\ll\mathbb P$. For $t\leq T$ its density on $\mathcal F_t$ is $\mathbb E[Z_T\mid\mathcal F_t]=Z_t$.

The finite-horizon [Girsanov theorem](../../../../../../girsanov-theorem.md) says that if $W$ is a [Brownian motion](../../../../../../brownian-motion-split.md) and $\mathcal E(\int h\,dW)$ is a true [martingale](../../../../../../martingale-split.md) through $T$ defining the density, then $W_t-\int_0^th_sds$ is a [Brownian motion](../../../../../../brownian-motion-split.md) under that density for $t\leq T$. Here $h_s=\mu$, and the [stochastic exponential](../../../../../../doleans-dade-exponential.md) is exactly $Z$. The previous part verifies the necessary [martingale](../../../../../../martingale-split.md) property; alternatively the [Novikov condition](../../../../../../novikov-s-condition.md) is $e^{\mu^2T/2}<\infty$. Hence $B_t-\mu t$ is a standard [Brownian motion](../../../../../../brownian-motion-split.md) on $[0,T]$ relative to the same [filtration](../../../../../../filtration-probability-theory.md) under $\mathbb P^T$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
