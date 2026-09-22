<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A **[weak solution of a stochastic differential equation](../../../../../../weak-solution-of-a-stochastic-differential-equation.md)** consists of a [filtered probability space](../../../../../../filtered-probability-space.md), an [adapted](../../../../../../adapted-process.md) continuous process $X$, and a [Brownian motion](../../../../../../brownian-motion-split.md) $B$ relative to that [filtration](../../../../../../filtration-probability-theory.md), with specified initial distribution, such that for every finite $t$ the coefficient integrals are finite and

$$
\boxed{X_t=X_0+\int_0^t\sigma(X_s)\,dB_s+\int_0^t b(X_s)\,ds\quad\text{almost surely for all }t.}
$$

In one dimension the integrability conditions are $\int_0^t\sigma(X_s)^2ds<\infty$ and $\int_0^t|b(X_s)|ds<\infty$. The noise integral is the [Itô integral](../../../../../../ito-integral.md). A solution on a prescribed stochastic basis with prescribed $B$ is distinguished from this weak construction.

A **[strong solution of a stochastic differential equation](../../../../../../strong-solution-of-a-stochastic-differential-equation.md)** uses the prescribed $B$ and initial variable, and is [adapted](../../../../../../adapted-process.md) to their augmented [natural filtration](../../../../../../natural-filtration.md); thus no additional randomness is needed. For deterministic $X_0=x$, each $X_t$ is determined by the driving [Brownian motion](../../../../../../brownian-motion-split.md) through time $t$. Merely being [adapted](../../../../../../adapted-process.md) to a larger [filtration](../../../../../../filtration-probability-theory.md) is insufficient for this definition.

**[Uniqueness in law](../../../../../../uniqueness-in-law.md)** means that any two [weak stochastic solutions](../../../../../../weak-solution-of-a-stochastic-differential-equation.md) with the same initial distribution have the same law of $X$ on continuous path space. **[Pathwise uniqueness](../../../../../../pathwise-uniqueness.md)** means that two solutions on one stochastic basis, with the same $B$ and almost surely equal initial values, are [indistinguishable stochastic processes](../../../../../../indistinguishability-of-stochastic-processes.md). The latter compares paths under the same noise, rather than just comparing their [probability distributions](../../../../../../probability-distribution.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
