<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A [Brownian excursion in the upper half-plane](../../../../../../brownian-excursion-in-the-upper-half-plane.md) from $0$ to infinity is killed [planar Brownian motion](../../../../../../planar-brownian-motion.md) conditioned to stay in $\mathbb H$, with its entrance law at $0$. Precisely, it is the [Doob h-transform](../../../../../../doob-h-transform.md) for $h(z)=\operatorname{Im}z$, obtained by starting at $i\varepsilon$ and letting $\varepsilon\downarrow0$. Equivalently,

$$
\boxed{\widehat B_t=W_t+iR_t,}
$$

where $W$ is standard [Brownian motion](../../../../../../brownian-motion-split.md) and the independent process $R$ is a dimension-three [Bessel process](../../../../../../bessel-process.md) started at zero. The transformed generator is $\frac12\Delta+y^{-1}\partial_y$, which explains this representation.

First compute avoidance from an interior point $z$. Let $\tau$ be the exit time of ordinary [planar Brownian motion](../../../../../../planar-brownian-motion.md) from $\mathbb H\setminus A$. The harmonic correction

$$
v(z)=\operatorname{Im}\bigl(z-g_A(z)\bigr)
$$

has boundary values $\operatorname{Im}z$ on $A$ and zero on the real axis. The [hydrodynamic normalization at infinity](../../../../../../hydrodynamic-normalization-at-infinity.md) gives $g_A(z)=z+\operatorname{hcap}(A)/z+O(|z|^{-2})$. Together with the [maximum principle for harmonic functions](../../../../../../maximum-principle-for-harmonic-functions.md) this gives the useful bound $0\leq v\leq\sup_{a\in A}\operatorname{Im}a$. Since ordinary [Brownian motion](../../../../../../brownian-motion-split.md) hits the real axis almost surely, the [optional stopping theorem](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) applied to this bounded [harmonic function](../../../../../../harmonic-function.md) gives

$$
v(z)=\mathbb E_z[\operatorname{Im}B_\tau]
=\mathbb E_z[\operatorname{Im}B_\tau\,\mathbf1_{\{B_\tau\in A\}}].
$$

The [Doob h-transform](../../../../../../doob-h-transform.md) weights a stopped path by its final height divided by its initial height. Applying this at the first hit of $A$, with bounded-time localization and then a limit, therefore yields

$$
\mathbb P_z^h(\tau_A<\infty)=\frac{v(z)}{\operatorname{Im}z},\qquad
\mathbb P_z^h(\tau_A=\infty)=\frac{\operatorname{Im}g_A(z)}{\operatorname{Im}z}.
$$

For the entrance law the same result follows by conditioning at a small positive time and letting that time decrease to zero: the avoidance function has the boundary limit computed next, and the excursion is initially in a neighbourhood disjoint from $A$.

Because the closure of the hull avoids $0$, the [Schwarz reflection principle](../../../../../../schwarz-reflection-principle.md) makes $g_A$ analytic in a neighbourhood of zero, with real $g_A(0)$ and positive real $g_A'(0)$. Thus

$$
\lim_{\varepsilon\downarrow0}\frac{\operatorname{Im}g_A(i\varepsilon)}{\varepsilon}=g_A'(0).
$$

In fact, the reflected Taylor expansion gives $\operatorname{Im}g_A(z)/\operatorname{Im}z=g_A'(0)+O(|z|)$ uniformly as $z\to0$ inside the half-plane, so the same limit applies to the entrance process. The map in the question is $\psi_A=g_A-g_A(0)$, so its derivative agrees with $g_A'$. We obtain the [restriction probability of a Brownian half-plane excursion](../../../../../../restriction-probability-of-a-brownian-half-plane-excursion.md):

$$
\boxed{\mathbb P\bigl[\widehat B([0,\infty))\cap A=\varnothing\bigr]=\psi_A'(0).}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 203](../../../paper-203-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
