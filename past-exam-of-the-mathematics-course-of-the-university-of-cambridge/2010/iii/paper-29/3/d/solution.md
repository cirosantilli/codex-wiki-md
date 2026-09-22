<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write $\tau_\varepsilon=T_\varepsilon\wedge T_M$. The stopped [Bessel process](../../../../../../bessel-process.md) has the same law as the weighted stopped [Brownian motion](../../../../../../brownian-motion-split.md), so for every bounded measurable functional $F$ of a continuous path,

$$
\mathbb E F(R^{\tau_\varepsilon})
=\mathbb E_{\mathbb W_x}\left[F(X^{\tau_\varepsilon})
\left(\frac Mx\mathbf1_{\{T_M<T_\varepsilon\}}
+\frac\varepsilon x\mathbf1_{\{T_\varepsilon<T_M\}}\right)\right].
$$

The [Bessel process](../../../../../../bessel-process.md) hits $M$ in finite time and never hits zero. Its minimum before that hitting time is strictly positive. Thus for sufficiently small $\varepsilon$, depending on the path, its stopped path $R^{\tau_\varepsilon}$ equals $R^{T_M}$ exactly. Under [Wiener measure](../../../../../../wiener-measure.md), the events $\{T_M<T_\varepsilon\}$ increase to $\{T_M<T_0\}$, and on that event the stopped paths eventually equal $X^{T_M}$. The remaining term is bounded by $\varepsilon\lVert F\rVert_\infty/x$. The [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) therefore yields the precise limiting identity

$$
\boxed{\mathbb E F(R^{T_M})
=\frac Mx\mathbb E_{\mathbb W_x}\left[
\mathbf1_{\{T_M<T_0\}}F(X^{T_M})\right].}
$$

The bounded stopped [martingale](../../../../../../martingale-split.md) $X_{t\wedge T_0\wedge T_M}$ gives

$$
x=\mathbb E X_{T_0\wedge T_M}=M\mathbb W_x(T_M<T_0),
\qquad \mathbb W_x(T_M<T_0)=x/M.
$$

Hence the limiting identity says

$$
\boxed{\mathcal L(R^{T_M})
=\mathcal L_{\mathbb W_x}(X^{T_M}\mid T_M<T_0).}
$$

This establishes [Brownian conditioning by a stopped Bessel density](../../../../../../brownian-conditioning-by-a-stopped-bessel-density.md).

The displayed density in the question requires a stopping convention. On the full, unstopped path space, the probability measure

$$
\frac{d\widetilde{\mathbb Q}^{M}}{d\mathbb W_x}
=\frac Mx\mathbf1_{\{T_M<T_0\}}
$$

is well-defined, but its paths continue as [Brownian motion](../../../../../../brownian-motion-split.md) after $T_M$. Its pushforward by the stopping map $\omega\mapsto\omega(\cdot\wedge T_M(\omega))$ is the law $\mathbb Q^M$ of the stopped [Bessel process](../../../../../../bessel-process.md). Equivalently, if $\mathbb W_x^{0,M}$ denotes the law of [Brownian motion](../../../../../../brownian-motion-split.md) stopped at $T_0\wedge T_M$, then the actual stopped laws satisfy

$$
\boxed{\frac{d\mathbb Q^M}{d\mathbb W_x^{0,M}}
=\frac Mx\mathbf1_{\{\text{exit at }M\}}.}
$$

Literal absolute continuity of the stopped law with respect to unstopped [Wiener measure](../../../../../../wiener-measure.md) is false: paths that become permanently constant at $M$ have probability one for the stopped law and zero under [Wiener measure](../../../../../../wiener-measure.md). The same density is also valid on the stopped sigma-algebra of the original coordinate space. Thus the corrected stopped-law formulation proves the intended conclusion without equating these different full-path measures.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
