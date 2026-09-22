<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Berezinskii–Kosterlitz–Thouless transition](../../../../../../berezinskii-kosterlitz-thouless-transition.md) is a defect-unbinding transition of a two-dimensional system with a compact continuous phase, such as the short-range [XY model](../../../../../../xy-model.md). At long wavelengths, smooth [spin waves](../../../../../../spin-wave.md) have energy

$$
F_{\rm sw}=\frac{\rho_s}{2}\int d^2x\,|\nabla\theta|^2,
$$

where $\rho_s$ is the [phase stiffness](../../../../../../phase-stiffness.md). Gaussian averaging gives

$$
\langle[\theta(\mathbf r)-\theta(0)]^2\rangle=\frac{k_BT}{\pi\rho_s}\log(r/a)+O(1),\qquad
\langle e^{i[\theta(\mathbf r)-\theta(0)]}\rangle\sim(a/r)^\eta,\quad
\eta=\frac{k_BT}{2\pi\rho_s}.
$$

Thus smooth fluctuations already destroy true nonzero magnetization in an infinite two-dimensional system, in accordance with the [Mermin-Wagner theorem](../../../../../../mermin-wagner-theorem.md). The low-temperature phase instead has [quasi-long-range order](../../../../../../quasi-long-range-order.md), with algebraically decaying correlations. The stiffness in its asymptotic exponent is the renormalized long-distance stiffness, not merely the microscopic coupling.

The phase is periodic modulo $2\pi$, so it also permits [topological defects](../../../../../../topological-defect.md) with integer winding $n$. A [phase vortex](../../../../../../phase-vortex.md) has $|\nabla\theta|=|n|/r$, and integration gives

$$
E_n=\pi\rho_s n^2\log(L/a)+E_{\rm core}.
$$

A singly charged [phase vortex](../../../../../../phase-vortex.md) can be placed in roughly $(L/a)^2$ locations, giving entropy $2k_B\log(L/a)$. This energy-entropy balance suggests that isolated [vortices](../../../../../../phase-vortex.md) become favorable when the effective stiffness falls to $2k_BT/\pi$. Below the transition, [vortex-antivortex binding](../../../../../../vortex-antivortex-binding.md) predominates; above it their unbinding screens the logarithmic interaction and produces a finite [correlation length](../../../../../../correlation-length.md). A single-vortex estimate identifies the mechanism but does not include screening by smaller pairs.

The dilute-vortex [vortex-pair renormalization flow](../../../../../../vortex-pair-renormalization-flow.md) incorporates this screening. With $K=\rho_s/(k_BT)$ and dimensionless core fugacity $y$, one conventional leading-order normalization gives

$$
\boxed{\frac{dK^{-1}}{d\ell}=4\pi^3y^2,\qquad
\frac{dy}{d\ell}=(2-\pi K)y.}
$$

The first equation says polarizable [phase vortex](../../../../../../phase-vortex.md) pairs reduce stiffness. The second compares the [phase vortex](../../../../../../phase-vortex.md)'s position scaling dimension two with its logarithmic energy cost $\pi K$. Numerical coefficients in $y$ depend on its definition, but the zero-fugacity threshold $K=2/\pi$ is invariant. For $K>2/\pi$, sufficiently small fugacity flows to zero, leaving a line of Gaussian spin-wave [renormalization-group fixed points](../../../../../../renormalization-group-fixed-point.md) with varying algebraic exponent. On the other side of the separatrix, fugacity grows and the dilute approximation eventually ceases to apply.

Near the endpoint set $X=2-\pi K$ and $Y=4\pi y$. To leading order $X'=Y^2$ and $Y'=XY$, so $X^2-Y^2$ is invariant. The critical separatrix approaches $(0,0)$. Just on the disordered side this invariant is $-\varepsilon^2$, proportional to the reduced temperature deviation for a generic path through the transition. Hence $X'=X^2+\varepsilon^2$, whose integration gives a time in logarithmic scale of order $1/\varepsilon$. Stopping when the fugacity becomes order one yields

$$
\boxed{\xi\sim a\exp(B/\sqrt\tau),\qquad \tau=(T-T_c)/T_c\downarrow0^+,}
$$

with nonuniversal $B>0$. This derives the essential singularity and explains why assigning a finite ordinary correlation-length exponent is inappropriate.

At the transition the limiting stiffness from below has the [universal stiffness jump](../../../../../../universal-stiffness-jump.md)

$$
\boxed{\rho_s(T_c^-)=\frac{2k_BT_c}{\pi},\qquad \eta(T_c)=1/4.}
$$

Above $T_c$, the thermodynamic long-distance stiffness vanishes and correlations decay exponentially. The singular free-energy contribution is of order $\xi^{-2}$ and is exponentially small in $1/\sqrt\tau$, so this infinite-order transition is unlike a Landau transition with a discontinuous [order parameter](../../../../../../order-parameter.md) or an ordinary power-law heat-capacity singularity. The renormalization mechanism is developed in [Kosterlitz's original vortex analysis](https://doi.org/10.1088/0022-3719/7/6/005). **The transition separates bound [vortices](../../../../../../phase-vortex.md) and algebraic order from unbound [vortices](../../../../../../phase-vortex.md) and short-range order, while neither finite-temperature phase has conventional spontaneous XY magnetization.**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
