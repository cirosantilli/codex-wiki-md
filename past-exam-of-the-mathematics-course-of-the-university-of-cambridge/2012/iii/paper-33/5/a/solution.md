<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $\tau=T_r\wedge T_R$. First establish almost sure finiteness. The [Itô formula](../../../../../../ito-s-lemma.md) gives the [martingale](../../../../../../martingale-split.md) $|B_t|^2-2t$ for planar [Brownian motion](../../../../../../brownian-motion-split.md). Stop it at $t\wedge T_R$. The stopped path has norm at most $R$, so

$$
2\mathbb E(t\wedge T_R)=\mathbb E|B_{t\wedge T_R}|^2-|x|^2\leq R^2-|x|^2.
$$

By [monotone convergence](../../../../../../monotone-convergence-theorem.md), $\mathbb E T_R<\infty$, and hence $\tau<\infty$ almost surely.

The function $h(y)=\log|y|$ is a [harmonic function](../../../../../../harmonic-function.md) away from $0$: in polar coordinates its [Laplacian](../../../../../../laplacian.md) is $h''(\rho)+h'(\rho)/\rho=-\rho^{-2}+\rho^{-2}=0$. The [Itô formula](../../../../../../ito-s-lemma.md) shows $h(B_{t\wedge\tau})$ is a [local martingale](../../../../../../local-martingale.md). It is bounded between $\log r$ and $\log R$, so it is a true [martingale](../../../../../../martingale-split.md) and passage to $\tau$ is justified by [dominated convergence](../../../../../../dominated-convergence-theorem.md). Writing $p=\mathbb P_x(T_r<T_R)$ and using continuity at exit gives

$$
\log|x|=\mathbb E_x\log|B_\tau|=p\log r+(1-p)\log R.
$$

Solving yields the [planar Brownian annulus hitting probability](../../../../../../planar-brownian-annulus-hitting-probability.md)

$$
\boxed{\mathbb P_x(T_r<T_R)=\frac{\log R-\log|x|}{\log R-\log r}.}
$$

The stopping argument stays away from the singularity of the logarithm until the calculation is complete.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
