<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $Z_t=\langle\kappa_t\rangle$, where the angle brackets average only over walk paths, and use $\mathbb E$ only for the environment. Every nearest-neighbor path of length $t$ has probability $(2d)^{-t}$, so the finite path sum is exactly the walk expectation. It depends only on environment layers through time $t$, and hence is $\mathcal F_t$-measurable. Its factors lie in $[1-\varepsilon,1+\varepsilon]$, so $Z_t$ is positive and integrable at each fixed time.

For any fixed path through time $t+1$, the environment variable $h(t+1,\xi_{t+1})$ is [independent](../../../../../../independent-random-variables.md) of $\mathcal F_t$ and has [mean](../../../../../../expected-value.md) zero. [Conditional expectation](../../../../../../conditional-expectation.md) therefore removes its last factor. Summing over the $2d$ possible last steps of each length-$t$ path cancels the extra factor $2d$ in the path probability. Thus

$$
\boxed{\mathbb E[Z_{t+1}\mid\mathcal F_t]=Z_t,\qquad Z_0=1,\qquad \mathbb EZ_t=1.}
$$

This is the [positive random-environment path-weight martingale](../../../../../../positive-random-environment-path-weight-martingale.md). It is nonnegative and bounded in $L^1$, so the [martingale convergence theorem](../../../../../../martingale-convergence-theorem.md) gives a finite limit $\zeta\ge0$ almost surely. At this stage one can conclude $\mathbb E\zeta\le1$ by [Fatou's lemma](../../../../../../fatou-s-lemma.md), but not yet equality; the second-moment bound in part (b) will prevent loss of [mean](../../../../../../expected-value.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
