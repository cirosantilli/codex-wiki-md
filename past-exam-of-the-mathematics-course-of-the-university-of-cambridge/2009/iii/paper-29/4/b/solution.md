<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $0\leq s\leq t$ and $E\in\mathcal F_s$, the definition of the [Radon-Nikodym derivative](../../../../../../radon-nikodym-derivative.md) gives

$$
\mathbb E_{\mathbb P}[\mathbf1_E Z_t]=\mathbb Q(E)=\mathbb E_{\mathbb P}[\mathbf1_E Z_s].
$$

The density is nonnegative and integrable; with the probability normalization used here its expectation is one. Hence

$$
\boxed{\mathbb E_{\mathbb P}[Z_t\mid\mathcal F_s]=Z_s,}
$$

so $Z$ is a [martingale](../../../../../../martingale-split.md). When $Z_t=h(X_t,t)$, the [Itô formula](../../../../../../ito-s-lemma.md) under Wiener measure gives

$$
dZ_t=h_x(X_t,t)dX_t+g(X_t,t)dt,\qquad g=h_t+\frac12h_{xx}.
$$

The first term is a [continuous local martingale](../../../../../../continuous-local-martingale.md), by localization on compact space-time sets. Since $Z$ is a [martingale](../../../../../../martingale-split.md), uniqueness of the [continuous semimartingale decomposition](../../../../../../continuous-semimartingale-decomposition.md) makes $\int_0^tg(X_s,s)ds=0$ identically. The integrand is continuous in time along every continuous path, so $g(X_t,t)=0$ for every $t$, outside one common null event.

For each fixed $t>0$, $X_t$ has a [Gaussian distribution](../../../../../../normal-distribution.md) with strictly positive density everywhere on $\mathbb R$. Since $g(\cdot,t)$ is continuous, $g(X_t,t)=0$ almost surely implies $g(x,t)=0$ for every real $x$. Therefore

$$
\boxed{h_t(x,t)+\frac12h_{xx}(x,t)=0\qquad(x\in\mathbb R,\ t>0).}
$$

If the stated smoothness includes time zero, continuity extends the equation there. This is the [backward heat equation](../../../../../../backward-heat-equation.md). The full-support argument is needed to pass from an identity along Brownian paths to an equation at every spatial point.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
