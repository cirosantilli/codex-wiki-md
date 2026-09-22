<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Write the [diffusion process](../../../../../markov-diffusion.md) as $dX_t=b(X_t)dt+\sigma(X_t)dB_t$, with $a=\sigma\sigma^{\mathsf T}$. Its [diffusion generator](../../../../../diffusion-generator.md) is

$$
L\varphi=\frac12\sum_{i,j}a^{ij}\partial_{ij}\varphi+\sum_i b^i\partial_i\varphi.
$$

The [Itô formula](../../../../../ito-s-lemma.md) says that $\varphi(X_t)-\varphi(X_0)-\int_0^tL\varphi(X_s)ds$ is a [local martingale](../../../../../local-martingale.md), and is a true [martingale](../../../../../martingale-split.md) when the stopped terms are integrable. Taking [expectations](../../../../../expected-value.md) gives [Dynkin formula for a diffusion](../../../../../dynkin-formula-for-a-diffusion.md). This is the bridge from infinitesimal stochastic dynamics to differential equations.

For the [transition semigroup](../../../../../markov-semigroup.md) $P_tg(x)=\mathbb E_xg(X_t)$, the [Markov property](../../../../../markov-property.md) gives $P_{t+s}=P_tP_s$. On a smooth generator domain where differentiation is valid, differentiating the semigroup identity yields the [Kolmogorov backward equation](../../../../../kolmogorov-backward-equation.md) $\partial_tP_tg=L(P_tg)$, with initial value $g$. If a transition density $p(t,x,y)$ exists, integration against smooth compactly supported tests and integration by parts give the [Fokker-Planck equation](../../../../../fokker-planck-equation.md)

$$
\partial_tp=L_y^*p,
\qquad
L^*p=\frac12\sum_{i,j}\partial_{ij}(a^{ij}p)-\sum_i\partial_i(b^ip).
$$

The backward equation acts on the starting point, while this forward equation describes the evolving probability density.

Here is a full representation proof with a source and potential. Suppose $X$ is nonexplosive, $V\ge0$ is bounded, $f,g$ are bounded, and $u$ is a bounded [classical solution](../../../../../classical-solution.md) on a finite slab of

$$
u_t+Lu-Vu=-f,\qquad u(T,x)=g(x).
$$

For a process started from $x$ at time $t$, put $D_s=\exp(-\int_t^sV(X_r)dr)$. The [Itô product rule](../../../../../ito-product-rule.md) gives

$$
d(D_su(s,X_s))=-D_sf(s,X_s)ds+D_s\nabla u(s,X_s)\sigma(X_s)dB_s.
$$

Therefore $D_su(s,X_s)+\int_t^sD_rf(r,X_r)dr$ is a [local martingale](../../../../../local-martingale.md). It is bounded in absolute value by $\|u\|_\infty+(T-t)\|f\|_\infty$, so it is a true [martingale](../../../../../martingale-split.md), without requiring a global derivative bound. Its endpoint [expectations](../../../../../expected-value.md) give the [parabolic Feynman-Kac formula with a source](../../../../../parabolic-feynman-kac-formula-with-a-source.md)

$$
\boxed{u(t,x)=\mathbb E_{t,x}\left[e^{-\int_t^TV(X_r)dr}g(X_T)
+\int_t^Te^{-\int_t^sV(X_r)dr}f(s,X_s)ds\right]}.
$$

This proves uniqueness in the bounded classical class. Setting $V=f=0$ recovers the backward heat or diffusion representation; the minus sign in the killing term produces the negative exponential.

For an elliptic problem, stop at the first exit $\tau$ from a bounded regular domain $D$. Suppose $\mathbb E_x\tau<\infty$, $u\in C^2(D)\cap C(\bar D)$ is bounded and solves $(L-V)u=-f$ with boundary data $g$. The same calculation, stopped at $t\wedge\tau$, gives a [martingale](../../../../../martingale-split.md) dominated by $\|u\|_\infty+\|f\|_\infty\tau$. Continuity puts $X_\tau$ on the boundary. Taking the limit and using [dominated convergence](../../../../../dominated-convergence-theorem.md) gives the [elliptic Feynman-Kac formula](../../../../../elliptic-feynman-kac-formula.md)

$$
\boxed{u(x)=\mathbb E_x\left[e^{-\int_0^\tau V(X_r)dr}g(X_\tau)
+\int_0^\tau e^{-\int_0^sV(X_r)dr}f(X_s)ds\right]}.
$$

For $V=f=0$, harmonic functions for $L$ give stopped [martingales](../../../../../martingale-split.md) and are averages of their exit-boundary values. For [Brownian motion](../../../../../brownian-motion-split.md) $L=\tfrac12\Delta$, this is the probabilistic solution of the [Dirichlet problem](../../../../../dirichlet-problem.md). Suitable smooth coefficients and uniform ellipticity give familiar settings where the required diffusion, exit-time integrability and [classical solutions](../../../../../classical-solution.md) exist. The representation itself follows from the stated regularity and integrability conditions, rather than claiming classical solvability for arbitrary coefficients.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 38](../../paper-38-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
