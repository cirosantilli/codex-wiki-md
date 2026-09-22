<h1 id="b/6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Assume $0<r<1<R$, as required for the annulus and logarithms. The [logarithmic radius of planar Brownian motion](../../../../../logarithmic-radius-of-planar-brownian-motion.md) is a local martingale. Stopping at $T=T_{r,R}$ keeps it between the constants $\log r$ and $\log R$, so the stopped process is a bounded [martingale](../../../../../martingale-split.md). The exit time is finite almost surely because the annulus is bounded and Brownian motion eventually exits its containing disk.

The [optional stopping theorem](../../../../../optional-sampling-theorem-for-a-supermartingale.md) followed by [dominated convergence](../../../../../dominated-convergence-theorem.md) gives $\mathbb E\log|Z_T|=\log|Z_0|=0$. Continuity puts the exit radius at either $r$ or $R$. If $p$ is the inner-exit probability, then $p\log r+(1-p)\log R=0$. Hence

$$
\boxed{p=\frac{\log R}{\log R-\log r}.}
$$

Stopping before taking expectations matters: the unstopped logarithmic-radius process is a [strict local martingale](../../../../../strict-local-martingale.md), so one cannot assume its unrestricted expectation is constant.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../split.md)
6. [Stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../../stochastic-differential-equations-and-brownian-motion-in-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
