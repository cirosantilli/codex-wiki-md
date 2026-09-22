<h1 id="6a/solution">Solution</h1>

↑ **Parent:** [6A](../6a.md)

Let $p_j^n$ be the probability of occupying site $ja$ after $n$ steps, with $p_j^0=\mathbf1_{\{j=0\}}$ and $\alpha+\beta=1$. The [master equation](../../../../../master-equation.md) is

$$
\boxed{p_j^{n+1}=\alpha p_{j-1}^n+\beta p_{j+1}^n.}
$$

Write $p_j^n\approx a p(ja,n\tau)$ so that the limiting $p$ is a [probability density](../../../../../probability-density.md). A [Taylor expansion](../../../../../taylor-expansion.md) of this [master equation](../../../../../master-equation.md) gives

$$
\tau p_t=(\beta-\alpha)a p_x+\frac{(\alpha+\beta)a^2}{2}p_{xx}+O(a^3,\tau^2).
$$

The weakly biased [diffusion limit of a weakly biased random walk](../../../../../diffusion-limit-of-a-weakly-biased-random-walk.md) keeps $a^2/\tau$ and $(\alpha-\beta)a/\tau$ finite as $a,\tau\to0$, so $\alpha-\beta=O(a)$. The limiting [advection-diffusion equation](../../../../../advection-diffusion-equation.md) is

$$
\boxed{p_t+Vp_x=Dp_{xx},\qquad V=\frac{a(\alpha-\beta)}\tau,\quad D=\frac{a^2(\alpha+\beta)}{2\tau}=\frac{a^2}{2\tau}.}
$$

Its initial condition is the [Dirac delta function](../../../../../dirac-delta-function.md) at the origin. At finite spacing, the exact variance gained per step is $a^2[1-(\alpha-\beta)^2]=4a^2\alpha\beta$. Thus a finite-step [central limit theorem](../../../../../central-limit-theorem.md) gives the variance-matched coefficient $2a^2\alpha\beta/\tau$; its difference from the displayed $D$ vanishes in the stated weak-bias [diffusion limit of a weakly biased random walk](../../../../../diffusion-limit-of-a-weakly-biased-random-walk.md). Keeping a fixed nonzero bias while taking diffusive space-time scaling would instead make $V$ diverge.

## ↑ Ancestors (10)

1. [6A](../6a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
