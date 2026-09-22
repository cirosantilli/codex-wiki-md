<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

In the periodic cube, $H_0=|\mathbf v|^2/2=(2\pi/L)^2|\mathbf J|^2/2$, so $\boldsymbol\Omega=(2\pi/L)\mathbf v$. The supplied [action-angle variables](../../../../action-angle-variables.md) are canonical: $d^3\theta\,d^3J=d^3x\,d^3v$. For $\mathbf k=2\pi\mathbf n/L$,

$$
\mathbf n\cdot\boldsymbol\Omega=\mathbf k\cdot\mathbf v,\qquad \mathbf n\cdot\partial_{\mathbf J}f_0=\mathbf k\cdot\partial_{\mathbf v}f_0.
$$

Consequently [c](../c.md) becomes

$$
\widetilde{\delta f}_{\mathbf k}(\mathbf v,\omega)=\frac{\mathbf k\cdot\partial_{\mathbf v}f_0}{\mathbf k\cdot\mathbf v-\omega}\widetilde{\delta\Phi}_{\mathbf k}^{\mathrm{tot}}(\omega).
$$

For each nonzero [wavenumber](../../../../wavenumber.md), the [Poisson equation for Newtonian gravity](../../../../poisson-equation-for-newtonian-gravity.md) gives

$$
-k^2\widetilde{\delta\Phi}_{\mathbf k}=4\pi G\int\widetilde{\delta f}_{\mathbf k}\,d^3v.
$$

Substitute the preceding response and add the externally imposed [Newtonian gravitational potential](../../../../newtonian-gravitational-potential.md):

$$
\widetilde{\delta\Phi}_{\mathbf k}^{\mathrm{tot}}=\widetilde{\delta\Phi}_{\mathbf k}^{\mathrm{ext}}-\frac{4\pi G}{k^2}\widetilde{\delta\Phi}_{\mathbf k}^{\mathrm{tot}}\int d^3v\,\frac{\mathbf k\cdot\partial_{\mathbf v}f_0}{\mathbf k\cdot\mathbf v-\omega}.
$$

Therefore

$$
\boxed{\widetilde{\delta\Phi}_{\mathbf k}^{\mathrm{tot}}=\frac{\widetilde{\delta\Phi}_{\mathbf k}^{\mathrm{ext}}}{\epsilon_{\mathbf k}(\omega)},\qquad \epsilon_{\mathbf k}(\omega)=1+\frac{4\pi G}{k^2}\int d^3v\,\frac{\mathbf k\cdot\partial_{\mathbf v}f_0}{\mathbf k\cdot\mathbf v-\omega}.}
$$

This [gravitational dielectric function](../../../../gravitational-dielectric-function.md) has the opposite susceptibility sign to the electron [dielectric function](../../../../dielectric-function.md), reflecting attractive rather than repulsive collective interactions. The homogeneous mean field is explicitly subtracted in this fictitious periodic model: the [Poisson equation for Newtonian gravity](../../../../poisson-equation-for-newtonian-gravity.md) acts on density fluctuations, and the $\mathbf k=0$ mode is omitted. Otherwise a nonzero uniform positive [mass density](../../../../density.md) would be incompatible with a periodic potential. This is the convention often called the [Jeans swindle](../../../../jeans-swindle.md).

For [analytic continuation](../../../../analytic-continuation.md), resolve [velocity](../../../../velocity.md) parallel to $\mathbf k$: let $u=\widehat{\mathbf k}\cdot\mathbf v$ and $F(u)=\int f_0(u,\mathbf v_\perp)\,d^2v_\perp$. Then

$$
\epsilon_{\mathbf k}(\omega)=1+\frac{4\pi G}{k^2}\int\frac{F'(u)}{u-\omega/k}\,du,\qquad k=|\mathbf k|.
$$

Start at $\operatorname{Im}\omega>0$ and deform the [Landau contour](../../../../landau-contour.md) continuously below the moving pole. At real $\omega$, the integral is

$$
\operatorname{PV}\int\frac{F'(u)}{u-\omega/k}\,du+i\pi F'(\omega/k).
$$

For $\operatorname{Im}\omega<0$, this causal continuation equals the undeformed real-axis integral plus $2\pi iF'(\omega/k)$ wherever $F'$ has the necessary analytic extension. It must not be replaced by the undeformed integral alone.

Zeros of $\epsilon_{\mathbf k}$ are self-consistent collective [Landau modes](../../../../landau-mode.md): with no external forcing, a nonzero [Newtonian gravitational potential](../../../../newtonian-gravitational-potential.md) is possible at such a root. For time dependence $e^{-i\omega t}$, upper-half-plane roots grow, lower-half-plane roots describe [Landau damping](../../../../landau-damping.md), and real roots are neutral. Damped [Landau modes](../../../../landau-mode.md) are poles of the continued response; they need not be regular discrete eigenfunctions of the original collisionless operator.

**Regularity qualification.** Continuation throughout the complex plane presupposes suitable analytic $F$. Arbitrary smooth $F$ need not allow it. For example, $F(u)=C\exp[-1/(1-u^2)]$ for $|u|<1$ and zero elsewhere is smooth but not analytic at $u=\pm1$; its Cauchy integral cannot be holomorphically continued across those endpoints. The [Landau contour](../../../../landau-contour.md) gives the standard causal continuation on the domains where the equilibrium permits it, with possible singularities retained.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [2024](../../../2024-split.md)
4. [Past exam of the kinetic theory course of the University of Oxford](../../../split.md)
5. [Kinetic theory course of the University of Oxford](../../../../kinetic-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
