<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [stochastic process](../../../../../../stochastic-process-split.md) $W$ starts from zero and has continuous paths. Its increments on disjoint intervals are [independent](../../../../../../independent-random-variables.md), since the corresponding pairs of [Brownian motion](../../../../../../brownian-motion-split.md) increments are [independent](../../../../../../independent-random-variables.md), and

$$
W_t-W_s\sim N\bigl(0,(\rho^2+1-\rho^2)(t-s)\bigr)=N(0,t-s).
$$

Thus **$W$ is a standard [Brownian motion](../../../../../../brownian-motion-split.md), including $\rho=\pm1$.** Here the intended [filtration](../../../../../../filtration-probability-theory.md) is the joint natural [filtration](../../../../../../filtration-probability-theory.md), or another [filtration](../../../../../../filtration-probability-theory.md) relative to which the pair is a two-dimensional [Brownian motion](../../../../../../brownian-motion-split.md); [independence](../../../../../../independent-random-variables.md) of their path laws alone would not justify arbitrary extra information in a larger [filtration](../../../../../../filtration-probability-theory.md).

By bilinearity of [quadratic covariation](../../../../../../quadratic-covariation.md) and part (i),

$$
\boxed{\langle W,B\rangle_t=\rho\langle B\rangle_t+\sqrt{1-\rho^2}\langle\widetilde B,B\rangle_t=\rho t.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
