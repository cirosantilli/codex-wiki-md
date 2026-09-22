<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Before $T(x)$, the centered image satisfies the [stochastic differential equation](../../../../../../stochastic-differential-equation.md)

$$
dX_t=\frac2{X_t}\,dt-\sqrt\kappa\,d\beta_t,\qquad X_0=x>0.
$$

Changing the sign of the [Brownian motion](../../../../../../brownian-motion-split.md) shows that $X/\sqrt\kappa$ is a [Bessel process](../../../../../../bessel-process.md) of dimension $1+4/\kappa$. Here is a direct proof of the relevant hitting property, including finite lifetime.

Put $p=1-4/\kappa>0$. By the [Itô formula](../../../../../../ito-s-lemma.md), the drift of $X^p$ is

$$
pX^{p-2}\left(2+\frac\kappa2(p-1)\right)=0.
$$

Thus $X^p$ is a [local martingale](../../../../../../local-martingale.md) and a [scale function of a one-dimensional diffusion](../../../../../../scale-function-stochastic-processes.md). Fix $R>x$. The nonnegative function

$$
u_R(v)=\frac{R^{2-p}v^p-v^2}{\kappa+4},\qquad 0\leq v\leq R,
$$

vanishes at both endpoints and satisfies $\mathcal Lu_R=-1$, for $\mathcal L=(\kappa/2)\partial_{vv}+(2/v)\partial_v$. Stop first on $[\epsilon,R]$, and also at a deterministic time. The [Itô formula](../../../../../../ito-s-lemma.md) gives $\mathbb E(t\wedge\tau_{\epsilon,R})\leq u_R(x)$. Let $t\to\infty$ and then $\epsilon\downarrow0$. It follows that the first exit $\tau_{0,R}$ is finite almost surely, not merely that the path approaches a boundary at infinite time.

[Optional stopping](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) applied to $X^p$ on this bounded interval gives

$$
\mathbb P_x(\tau_R<\tau_0)=\left(\frac{x}{R}\right)^p.
$$

On $\{\tau_0=\infty\}$ the process must therefore hit every $R>x$ before zero. Letting $R\to\infty$ makes that probability zero. Consequently

$$
\boxed{\kappa>4\ \Longrightarrow\ T(x)<\infty\quad\text{almost surely}.}
$$

At $\kappa=4$ the dimension is two; zero is not hit from a positive starting point. This endpoint must not be included in the finite-swallowing assertion.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
