<h1 id="b/6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $d=|z_0|$, the initial distance from the annulus center, and $T=T_{A_{r,R}}$. The function $z\mapsto\log|z-z_0|$ is harmonic on the annulus, so its value along stopped planar [Brownian motion](../../../../../brownian-motion-split.md) is a [local martingale](../../../../../local-martingale.md) by [Itô's formula](../../../../../ito-s-lemma.md). It is bounded between $\log r$ and $\log R$ before exit, hence is a true bounded martingale.

By the assumed almost sure finiteness of $T$, continuity, and [dominated convergence](../../../../../dominated-convergence-theorem.md),

$$
\log d=p\log r+(1-p)\log R,
$$

where $p$ is the inner-boundary exit probability. Solving gives the [harmonic measure of an annulus](../../../../../harmonic-measure-of-an-annulus.md):

$$
\boxed{\mathbb P(|Z_T-z_0|=r)=\frac{\log(R/d)}{\log(R/r)},\qquad
\mathbb P(|Z_T-z_0|=R)=\frac{\log(d/r)}{\log(R/r)}.}
$$

The two probabilities sum to one, as the exit must lie on one of the two circles.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../split.md)
6. [Stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../../stochastic-differential-equations-and-brownian-motion-in-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
