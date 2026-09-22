<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a nonrotating inviscid [Boussinesq](../../../../../../boussinesq-approximation.md) fluid, start from $\nabla\cdot\mathbf u=0$, $D\rho/Dt=0$ and

$$
\frac{D\mathbf u}{Dt}=-\frac1{\rho_0}\nabla p-\frac{g\rho}{\rho_0}\hat{\mathbf z}.
$$

The resting background has $\bar p_z=-g\bar\rho$ and $N^2=-g\bar\rho_z/\rho_0>0$. Write $\rho=\bar\rho(z)+\rho'$, $p=\bar p+p'$ and $\sigma=-g\rho'/\rho_0$. Keeping first-order terms gives

$$
\boxed{\nabla\cdot\mathbf u'=0,\qquad \mathbf u'_t=-\nabla p'/\rho_0+\sigma\hat{\mathbf z},\qquad \sigma_t=-N^2w'}.
$$

The PDF has a genuine sign error: its momentum equation uses a minus sign before $\sigma\hat{\mathbf z}$ despite defining $\sigma=-g\rho'/\rho_0$. A lighter parcel has $\sigma>0$ and accelerates upward, so the plus sign is necessary. Retaining both printed signs would yield negative squared wave frequency and exponential growth in a supposedly stable fluid; no oscillatory stable-wave [dispersion relation](../../../../../../dispersion-relation.md) follows from that inconsistent system. Alternatively one can define a downward density variable $\widetilde\sigma=g\rho'/\rho_0$, but then its density equation must have $\widetilde\sigma_t=+N^2w'$.

For the consistent system, take a [plane internal gravity wave](../../../../../../plane-internal-gravity-wave.md) proportional to $e^{i(kx+mz-\omega t)}$, with $k\ne0$. [Incompressibility](../../../../../../incompressible-flow.md) gives $ku+mw=0$. Project the [momentum](../../../../../../momentum.md) equation perpendicular to the [wavevector](../../../../../../wavevector.md), eliminating pressure: $-i\omega w=k^2\sigma/(k^2+m^2)$. Combining with $-i\omega\sigma=-N^2w$ gives

$$
\boxed{\omega^2=\frac{N^2k^2}{k^2+m^2}}.
$$

On a smooth signed-frequency branch, the [phase velocity](../../../../../../phase-velocity.md) and [group velocity](../../../../../../group-velocity.md) are

$$
\mathbf c_p=\frac{\omega(k,m)}{k^2+m^2},\qquad \mathbf c_g=\left(\frac{\omega m^2}{k(k^2+m^2)},-\frac{\omega m}{k^2+m^2}\right).
$$

Their scalar product is zero. Equivalently, the [dispersion relation](../../../../../../dispersion-relation.md) is homogeneous of degree zero in $(k,m)$, so [Euler homogeneous function theorem](../../../../../../euler-theorem-for-homogeneous-functions.md) gives $(k,m)\cdot\nabla_{(k,m)}\omega=0$. The [phase velocity](../../../../../../phase-velocity.md) moves crests normal to their phase lines; the [group velocity](../../../../../../group-velocity.md) moves wave packets and [energy](../../../../../../energy.md) along those lines. Their perpendicularity explains why following individual crests does not reveal the direction of [energy](../../../../../../energy.md) propagation.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
