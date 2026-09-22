<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $w\ne0$ in $\mathbb R^3$, the radial function $r(w)=\lVert w\rVert$ has

$$
\partial_i r=\frac{w_i}{r},\qquad
\partial_{ij}r=\frac{\delta_{ij}}{r}-\frac{w_iw_j}{r^3},\qquad
\Delta r=\frac2r.
$$

The multidimensional [Itô formula](../../../../../../ito-s-lemma.md), initially stopped away from zero, gives

$$
dR_t=\sum_{i=1}^3\frac{W_t^i}{R_t}\,dW_t^i+\frac{dt}{R_t}.
$$

The martingale term has [quadratic variation](../../../../../../quadratic-variation.md) $dt$, since $\sum_i(W_t^i/R_t)^2=1$. The [Lévy characterization of Brownian motion](../../../../../../levy-characterization-of-brownian-motion.md) says that a continuous [local martingale](../../../../../../local-martingale.md) starting at zero with [quadratic variation](../../../../../../quadratic-variation.md) $t$ is a standard [Brownian motion](../../../../../../brownian-motion-split.md). Consequently the radial equation is

$$
\boxed{dR_t=dB_t+\frac{dt}{R_t}.}
$$

On $[\varepsilon,M]$ the drift $1/r$ is [Lipschitz continuous](../../../../../../lipschitz-continuity.md). Extend it to a bounded globally [Lipschitz function](../../../../../../lipschitz-continuity.md) on the real line. The standard existence and pathwise uniqueness theorem for [stochastic differential equations](../../../../../../stochastic-differential-equation.md) with globally Lipschitz coefficients applies to this extension, and gives uniqueness in law up to the first exit from $[\varepsilon,M]$. Both this radial process and the process in part (a) solve the same equation from $x$. Thus

$$
\boxed{\mathcal L(R_{\cdot\wedge\tau_R})
=\mathcal L_{\mathbb Q^{M,\varepsilon}}(X_{\cdot\wedge\tau_X}),}
$$

where each exit time is computed from its own coordinate path.

For completeness, the radial equation is valid globally: the [three-dimensional Bessel process](../../../../../../three-dimensional-bessel-process.md) does not hit zero. Apply the [Itô formula](../../../../../../ito-s-lemma.md) to $1/R$ on the annulus. Its drift is zero, and the stopped process is a bounded [martingale](../../../../../../martingale-split.md). At the first exit,

$$
\frac1x=\frac1\varepsilon\mathbb P(T_\varepsilon<T_M)
+\frac1M\mathbb P(T_M<T_\varepsilon),
$$

so

$$
\mathbb P(T_\varepsilon<T_M)=\frac{\varepsilon(M-x)}{x(M-\varepsilon)}\longrightarrow0.
$$

The exit time is finite because one coordinate of the underlying [Brownian motion](../../../../../../brownian-motion-split.md) reaches $M$ in finite time. Letting $\varepsilon\downarrow0$ and then considering arbitrarily large $M$ proves that zero is never reached. The radial martingale therefore has [quadratic variation](../../../../../../quadratic-variation.md) $t$ on the whole time axis, completing the [Lévy characterization of Brownian motion](../../../../../../levy-characterization-of-brownian-motion.md) argument.

## ↑ Ancestors (11)

1. [B](../b.md)
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
