<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $\pi$ be pressure divided by the reference density and $b$ the buoyancy perturbation. The linear, inviscid [Boussinesq equations](../../../../../../boussinesq-equations.md) about $U(z)$ are

$$
u_t+Uu_x+U'w=-\pi_x,\quad
w_t+Uw_x=-\pi_z+b,\quad
b_t+Ub_x+N^2w=0,\quad
u_x+w_z=0.
$$

For a stationary Fourier component $e^{ikx}$, [incompressibility](../../../../../../incompressible-flow.md) gives $u=iw'/k$. The horizontal momentum equation then gives $\pi=i(U'w-Uw')/k$, while buoyancy conservation gives $b=iN^2w/(kU)$. Substitute these into the vertical momentum equation to obtain the stationary [Taylor–Goldstein equation](../../../../../../taylor-goldstein-equation.md):

$$
w''+\left(\frac{N^2}{U^2}-\frac{U''}{U}-k^2\right)w=0.
$$

Hence its local [WKB approximation](../../../../../../wkb-approximation.md) is

$$
\boxed{m^2=\left(\frac{N^2}{k^2U^2}-\frac{U''}{k^2U}-1\right)k^2.}
$$

For $U''$ negligible, an outgoing upward wave has $mU/k>0$. In particular $m>0$ for $k,U>0$. In an upper evanescent region choose the branch with $\operatorname{Im}m>0$ in $e^{i\int m\,dz}$ so the solution decays upward. These choices express the [radiation condition](../../../../../../radiation-condition.md); a reflected wave has the opposite real branch and downward [group velocity](../../../../../../group-velocity.md).

There are two different limiting levels. A [critical layer in a shear flow](../../../../../../critical-layer-in-a-shear-flow.md) occurs at $U=0$, where the intrinsic frequency vanishes, $|m|\to\infty$, and upward propagation slows while the vertical wavelength contracts. Dissipation or nonlinear effects can absorb the wave and transfer its momentum to the mean flow. For a stable, slowly varying critical layer with [Richardson number](../../../../../../richardson-number.md) $\operatorname{Ri}=N_0^2/(U')^2>1/4$, the usual causal inviscid continuation suppresses transmission; it is not the same as reflection at $m=0$. When the Richardson number is small, a general absorption-only conclusion needs extra stability assumptions.

Reflection instead occurs at the [turning level of a stationary internal wave](../../../../../../turning-level-of-a-stationary-internal-wave.md) $k|U|=N_0$, beyond which $m^2<0$. It is sometimes called a critical reflection height, but the wind there is nonzero. Assuming $0<kU_0<N_0$, the specified profiles give

$$
\boxed{\begin{array}{ll}
U=U_0(1+z/H):&\text{reflection at }\displaystyle\zeta=H\left(\frac{N_0L}{2\pi U_0}-1\right),\\
U=U_0(1-z/H):&\text{critical-layer absorption at }\zeta=H.
\end{array}}
$$

The decreasing-wind profile never encounters $m=0$ before its zero-wind layer. Both profiles have $U''=0$; a well-separated WKB description requires $N_0H/U_0\gg1$, and a turning-layer transition is still required for the increasing profile.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 71](../../../paper-71-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
