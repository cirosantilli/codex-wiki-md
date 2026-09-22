<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $u(z)=|z|^{2-d}$. For a radial function $r^{2-d}$, the [Laplacian](../../../../../../laplacian.md) is

$$
u''(r)+\frac{d-1}{r}u'(r)=(2-d)(1-d)r^{-d}+(d-1)(2-d)r^{-d}=0.
$$

Thus $u$ is a [harmonic function](../../../../../../harmonic-function.md) off zero. Fix $R>|x|$ and stop [Brownian motion](../../../../../../brownian-motion-split.md) when it reaches either sphere of radius $\varepsilon$ or $R$, at time $S_R$. This exit time is finite: stopping the [martingale](../../../../../../martingale-split.md) $|B_t|^2-dt$ at $S_R\wedge t$ yields $d\mathbb E(S_R\wedge t)\leq R^2-|x|^2$, and [monotone convergence](../../../../../../monotone-convergence-theorem.md) applies. By [Itô's formula](../../../../../../ito-s-lemma.md), $u(B_{t\wedge S_R})$ is a bounded [martingale](../../../../../../martingale-split.md). [Optional stopping](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) and [dominated convergence](../../../../../../dominated-convergence-theorem.md) therefore give

$$
u(x)=q_R\varepsilon^{2-d}+(1-q_R)R^{2-d},\qquad
q_R=\mathbb P_x(T_\varepsilon<T_R)=\frac{|x|^{2-d}-R^{2-d}}{\varepsilon^{2-d}-R^{2-d}}.
$$

The events $\{T_\varepsilon<T_R\}$ increase to $\{T_\varepsilon<\infty\}$ as $R\to\infty$: a continuous path up to any finite hitting time is bounded. Since $d\geq3$, $R^{2-d}\to0$, proving the [Brownian hitting probability of a ball](../../../../../../brownian-hitting-probability-of-a-ball.md)

$$
\boxed{\mathbb P_x(T_\varepsilon<\infty)=(\varepsilon/|x|)^{d-2}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
