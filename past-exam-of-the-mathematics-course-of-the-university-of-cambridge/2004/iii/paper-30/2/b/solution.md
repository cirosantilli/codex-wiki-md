<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $X_t=x+W_t+\mu t$ with $W$ a zero-starting [Brownian motion](../../../../../../brownian-motion-split.md). A unit-time increment exceeds $2b$ with probability

$$
p=\mathbb P(N(\mu,1)>2b)>0.
$$

If the process has not exited before an integer time $k$, it is in $(-b,b)$; an increment exceeding $2b$ forces it outside at time $k+1$ and hence forces an exit by then. Independence of [Brownian increments](../../../../../../brownian-increment.md) gives $\mathbb P(T>k)\le(1-p)^k$. Thus the [geometric tail bound from a uniform escape probability](../../../../../../geometric-tail-bound-from-a-uniform-escape-probability.md) yields

$$
\mathbb E T^2=\int_0^\infty2s\,\mathbb P(T>s)ds
\le\sum_{k=0}^\infty(2k+1)(1-p)^k=\frac{2-p}{p^2}<\infty.
$$

In particular $T$ is finite almost surely.

The [diffusion generator](../../../../../../diffusion-generator.md) is $\mathcal L=\tfrac12\partial_{xx}+\mu\partial_x$. The function $f(z)=e^{-2\mu z}$ satisfies $\mathcal Lf=0$, so the [Itô formula](../../../../../../ito-s-lemma.md) gives $df(X_t)=-2\mu f(X_t)dW_t$. It is a true [martingale](../../../../../../martingale-split.md), since it is $e^{-2\mu x}$ times the Gaussian exponential [martingale](../../../../../../martingale-split.md) $e^{-2\mu W_t-2\mu^2t}$. The stopped values $f(X_{t\wedge T})$ are uniformly bounded because the stopped path stays in $[-b,b]$. Optional sampling and bounded convergence give

$$
e^{-2\mu x}=p_-e^{2\mu b}+(1-p_-)e^{-2\mu b},
$$

where continuity ensures that $X_T$ is exactly one of the two endpoints. Solving,

$$
\boxed{\mathbb P(T_-<T_+)=\frac{e^{-2\mu x}-e^{-2\mu b}}{e^{2\mu b}-e^{-2\mu b}}.}
$$

This [drifted Brownian interval-exit probability](../../../../../../drifted-brownian-interval-exit-probability.md) tends to $(b-x)/(2b)$ as $\mu\to0$, as expected.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
