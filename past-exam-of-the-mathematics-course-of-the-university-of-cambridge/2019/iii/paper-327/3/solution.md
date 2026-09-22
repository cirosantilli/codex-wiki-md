<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [Paley–Wiener–Schwartz theorem](../../../../../paley-wiener-schwartz-theorem.md) in its closed-ball form says that a [tempered distribution](../../../../../tempered-distribution.md) $u$ is supported in $\overline B_R(0)$ if and only if its [Fourier transform](../../../../../fourier-transform.md) is the real restriction of an [entire function](../../../../../entire-function.md) $F$ on $\mathbb C^n$ satisfying, for some $C>0$ and integer $N\geq0$,

$$
\boxed{|F(\zeta)|\leq C(1+|\zeta|)^N e^{R|\operatorname{Im}\zeta|}.}
$$

The distribution is unique by [Fourier inversion](../../../../../fourier-inversion-theorem.md). More generally a compact convex support set $K$ replaces $R|\operatorname{Im}\zeta|$ by its [support function](../../../../../support-function.md) $H_K(\operatorname{Im}\zeta)$.

For the forward implication, a [compactly supported distribution](../../../../../compactly-supported-distribution.md) has finite [order of a distribution](../../../../../order-of-a-distribution.md), say $m$, on a fixed neighborhood of its support. Define

$$
F(\zeta)=\langle u,e^{-ix\cdot\zeta}\rangle,
$$

using a cutoff equal to one near the support. Differentiation with respect to each complex coordinate is allowed in this pairing and gives $\partial_{\zeta_j}F=\langle u,-ix_je^{-ix\cdot\zeta}\rangle$, so $F$ is entire.

To obtain the exact radius $R$, rather than an enlarged radius, choose a [cutoff function](../../../../../cutoff-function.md) $\chi_\varepsilon$ equal to one near $\overline B_R$ and supported in $B_{R+\varepsilon}$, with derivatives through order $m$ bounded by $C_\gamma\varepsilon^{-|\gamma|}$. Set $\varepsilon=(1+|\zeta|)^{-1}$. The finite-order bound and the [Leibniz rule](../../../../../leibniz-rule.md) give

$$
|F(\zeta)|\leq C(1+|\zeta|)^m e^{(R+\varepsilon)|\operatorname{Im}\zeta|}
\leq Ce(1+|\zeta|)^m e^{R|\operatorname{Im}\zeta|}.
$$

This proves the required growth estimate.

For the converse, $F$ has at most [polynomial growth](../../../../../polynomial-growth.md) on real frequencies, so define its inverse [tempered distribution](../../../../../tempered-distribution.md) by

$$
\langle u,\varphi\rangle=(2\pi)^{-n}\int_{\mathbb R^n}F(\xi)\widehat\varphi(-\xi)\,d\xi.
$$

Let a compactly supported test function lie in a half-space $x\cdot\omega\geq R+\eta$, with $|\omega|=1$ and $\eta>0$. By [contour shifting](../../../../../contour-shifting.md),

$$
\langle u,\varphi\rangle=(2\pi)^{-n}\int_{\mathbb R^n}
F(\xi+it\omega)\widehat\varphi(-\xi-it\omega)\,d\xi,\qquad t\geq0.
$$

Here is the decay needed to justify the shift and then let $t$ grow. Repeated [integration by parts](../../../../../integration-by-parts.md), applying $1-\Delta_x$ to $e^{-t x\cdot\omega}\varphi(x)$, gives for every integer $M$,

$$
|\widehat\varphi(-\xi-it\omega)|
\leq C_M(1+t)^{2M}e^{-(R+\eta)t}(1+|\xi|^2)^{-M}.
$$

Choose $2M>N+n$. For each fixed $t$, this decay makes the vertical sides of a large rectangle vanish in the one complex coordinate parallel to $\omega$; [Cauchy integral theorem](../../../../../cauchy-s-integral-theorem.md) then supplies the contour identity. Combining the two bounds yields

$$
|\langle u,\varphi\rangle|
\leq C'(1+t)^{N+2M}e^{-\eta t}\longrightarrow0.
$$

Thus $u$ vanishes on such test functions. Every point outside $\overline B_R$ has a neighborhood of this form. A [partition of unity](../../../../../partition-of-unity.md) therefore proves $\operatorname{supp}u\subseteq\overline B_R$, completing the converse. The same argument with separating half-spaces proves the compact-convex-set form. This is the [contour-shift proof of the Paley–Wiener–Schwartz theorem](../../../../../contour-shift-proof-of-the-paley-wiener-schwartz-theorem.md).

For a regular function $u$, the [change of variables](../../../../../change-of-variables-formula.md) $y=tx$ gives

$$
\int u(tx)\varphi(x)\,dx=t^{-n}\int u(y)\varphi(y/t)\,dy.
$$

The map $\varphi\mapsto\varphi(\mathord\cdot/t)$ is continuous on the [Schwartz space](../../../../../schwartz-space.md), so duality extends the [dilation of a distribution](../../../../../dilation-of-a-distribution.md) to

$$
\boxed{\langle\delta_tu,\varphi\rangle=t^{-n}\langle u,\delta_{1/t}\varphi\rangle.}
$$

Its Fourier transform obeys $\widehat{\delta_tu}(\zeta)=t^{-n}F(\zeta/t)$. If the original support is in the unit ball, the theorem bounds $F$ by $C(1+|\zeta|)^Ne^{|\operatorname{Im}\zeta|}$. Hence

$$
|\widehat{\delta_tu}(\zeta)|\leq C_t(1+|\zeta|)^N e^{|\operatorname{Im}\zeta|/t}.
$$

The converse theorem gives the [support law for distributional dilation](../../../../../support-law-for-distributional-dilation.md)

$$
\boxed{\operatorname{supp}(\delta_tu)\subseteq\{x:|x|\leq1/t\}=\{x:|tx|\leq1\}.}
$$

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 327](../../paper-327-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
