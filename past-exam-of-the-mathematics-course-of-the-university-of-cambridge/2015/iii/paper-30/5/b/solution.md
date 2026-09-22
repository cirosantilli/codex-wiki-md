<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The angle is a bounded [local martingale](../../../../../../local-martingale.md), hence a [uniformly integrable martingale](../../../../../../uniformly-integrable-martingale.md). The [martingale convergence theorem](../../../../../../martingale-convergence-theorem.md) gives an almost sure and $L^1$ limit $\Theta_\infty\in[-\pi/2,\pi/2]$ with

$$
\mathbb E\Theta_\infty=\arctan x.
$$

It must lie at an endpoint. Indeed, the [Itô isometry](../../../../../../ito-isometry.md) and boundedness give

$$
\mathbb E\int_0^\infty\cos^2\Theta_s\,ds
=\lim_{t\to\infty}\mathbb E[(\Theta_t-\Theta_0)^2]
\leq\pi^2<\infty.
$$

Thus the bracket integral is finite almost surely. If the angle converged to an interior point, its squared cosine would eventually be bounded below by a positive constant, forcing this integral to be infinite. Consequently

$$
\boxed{\Theta_\infty\in\{-\pi/2,\pi/2\}\quad\text{almost surely}.}
$$

This proves [endpoint convergence of a bounded angle diffusion](../../../../../../endpoint-convergence-of-a-bounded-angle-diffusion.md).

Let $p_x=\mathbb P(\Theta_\infty=\pi/2)$. Since $X_t=\tan\Theta_t$, this is exactly $\mathbb P(X_t\to+\infty)$, and the other endpoint means $X_t\to-\infty$. Taking expectations gives

$$
\arctan x=\frac\pi2p_x-\frac\pi2(1-p_x),
\qquad
\boxed{\mathbb P(X_t\to+\infty)=\frac12+\frac{\arctan x}{\pi}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
