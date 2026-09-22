<h1 id="a/2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For positive times the transformed process is centered and jointly Gaussian, and

$$
\mathbb E(X_sX_t)=st\min(1/s,1/t)=\min(s,t).
$$

Its paths are continuous away from zero. To verify continuity at zero, we need $B_u/u\to0$ almost surely as $u\to\infty$. The [strong law of large numbers](../../../../../strong-law-of-large-numbers.md) applied to the independent increments $B_{n+1}-B_n$ gives $B_n/n\to0$. On the unit interval after $n$, the [Doob L2 maximal inequality](../../../../../doob-l2-maximal-inequality.md) gives

$$
\mathbb P\left(\sup_{0\leq v\leq1}|B_{n+v}-B_n|>\varepsilon n\right)\leq\frac4{\varepsilon^2n^2}.
$$

The [Borel-Cantelli first lemma](../../../../../borel-cantelli-first-lemma.md), first for each positive rational $\varepsilon$, shows that these between-integer fluctuations divided by $n$ tend to zero. Hence $B_u/u\to0$ for all real $u\to\infty$, and $tB_{1/t}\to0$ as $t\downarrow0$.

The [Gaussian-process characterization of Brownian motion](../../../../../gaussian-process-characterization-of-brownian-motion.md) now proves **$X$ is standard Brownian motion**, with respect to its natural filtration. This is [time inversion of Brownian motion](../../../../../time-inversion-of-brownian-motion.md); the transformed process need not be adapted to the original forward filtration.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [2](../../2.md)
3. [A](../../../a.md)
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
