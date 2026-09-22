<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Put $r=|\mathbf x|$ and $s=\mathbf F\cdot\mathbf x$. In the [Unscaled Papkovich–Neuber representation](../../../../../unscaled-papkovich-neuber-representation.md), take the harmonic potentials $\boldsymbol\Phi=-\mathbf F/(8\pi\mu r)$ and $\chi=0$. Differentiating $s/r$ gives the [Stokeslet](../../../../../stokeslet.md) [velocity](../../../../../velocity.md) and its [pressure](../../../../../pressure.md):

$$
\boxed{\mathbf u=\frac1{8\pi\mu}\left(\frac{\mathbf F}{r}+\frac{s\mathbf x}{r^3}\right)},\qquad p=\frac{s}{4\pi r^3}.
$$

Indeed, writing $K=1/(8\pi\mu)$,

$$
\partial_j u_i=K\left[-\frac{F_i x_j}{r^3}+\frac{F_j x_i}{r^3}+\frac{s\delta_{ij}}{r^3}-\frac{3s x_i x_j}{r^5}\right].
$$

The antisymmetric first two terms cancel in the [rate-of-strain tensor](../../../../../strain-rate-tensor.md), whereas their [curl](../../../../../curl.md) supplies the [vorticity](../../../../../vorticity.md). Thus

$$
\boxed{e_{ij}=\frac{s}{8\pi\mu r^3}\left(\delta_{ij}-\frac{3x_i x_j}{r^2}\right),\qquad \boldsymbol\omega=\frac{\mathbf F\times\mathbf x}{4\pi\mu r^3}}.
$$

The [rate-of-strain tensor](../../../../../strain-rate-tensor.md) has zero trace, as required by [incompressibility](../../../../../incompressible-flow.md). The stress is $\sigma_{ij}=-3s x_i x_j/(4\pi r^5)$; integrating its traction with normal $\mathbf x/r$ over a [sphere](../../../../../sphere.md) gives $-\mathbf F$. This fixes the [force](../../../../../force.md) normalization of the [Stokeslet](../../../../../stokeslet.md).

For a [sphere in a uniform straining Stokes flow](../../../../../sphere-in-a-uniform-straining-stokes-flow.md), write the ambient [velocity](../../../../../velocity.md) as $\mathbf E\mathbf x$, where $\mathbf E$ is symmetric and trace-free, and set $q=\mathbf x\cdot\mathbf E\mathbf x$. Symmetry gives zero translation and rotation of the centred [force-free](../../../../../force-free.md), [torque-free](../../../../../torque-free.md) [sphere](../../../../../sphere.md). Seek a decaying disturbance using the [Unscaled Papkovich–Neuber representation](../../../../../unscaled-papkovich-neuber-representation.md) with

$$
\boldsymbol\Phi=C a^3\frac{\mathbf E\mathbf x}{r^3},\qquad \chi=D a^5\frac{q}{r^5}.
$$

The components of $\mathbf E\mathbf x/r^3$ are derivatives of $1/r$, and $q/r^5$ is a trace-free harmonic quadrupole, so both potentials satisfy [Laplace's equation](../../../../../laplace-equation.md) outside the [sphere](../../../../../sphere.md). Direct differentiation yields

$$
\mathbf u'=-3Ca^3\frac{q\mathbf x}{r^5}+2Da^5\frac{\mathbf E\mathbf x}{r^5}-5Da^5\frac{q\mathbf x}{r^7}.
$$

The [no-slip boundary condition](../../../../../no-slip-boundary-condition.md) at $r=a$ requires the coefficient of $\mathbf E\mathbf x$ to be $-1$ and that of $q\mathbf x$ to vanish: $2D=-1$, $-3C-5D=0$. Hence $D=-1/2$, $C=5/6$, and

$$
\boxed{\mathbf u'=-\frac{a^5}{r^5}\mathbf E\mathbf x-\frac{5a^3}{2r^5}\left(1-\frac{a^2}{r^2}\right)q\mathbf x},\qquad p'=-\frac{5\mu a^3q}{r^5}.
$$

This disturbance cancels the ambient [velocity](../../../../../velocity.md) at $r=a$, decays at infinity, and has a leading [stresslet](../../../../../force-dipole-flow.md) proportional to $a^3\mathbf E$.

For the two-sphere [hydrodynamic interaction](../../../../../hydrodynamic-interaction.md), let $\mathbf R=R\mathbf n$ point from the forced [sphere](../../../../../sphere.md) to the second [sphere](../../../../../sphere.md). The first [sphere](../../../../../sphere.md)'s leading far field is the [Stokeslet](../../../../../stokeslet.md) with $\mathbf F=6\pi\mu a\mathbf U_0$. Its incident [rate-of-strain tensor](../../../../../strain-rate-tensor.md) at the second [sphere](../../../../../sphere.md) is

$$
\mathbf E_2=\frac{3a}{4R^3}(\mathbf U_0\cdot\mathbf R)(\mathbf I-3\mathbf n\mathbf n),\qquad \mathbf E_2:\mathbf R\mathbf R=-\frac{3a}{2R}(\mathbf U_0\cdot\mathbf R).
$$

The [force-free](../../../../../force-free.md) [sphere](../../../../../sphere.md) translates with the local uniform incident flow, and the [torque-free](../../../../../torque-free.md) [sphere](../../../../../sphere.md) rotates with half the incident [vorticity](../../../../../vorticity.md). Those parts cause no leading [Stokeslet](../../../../../stokeslet.md) or [rotlet](../../../../../rotlet.md) disturbance. The remaining incident strain produces the [stresslet](../../../../../force-dipole-flow.md) just calculated. At displacement $-\mathbf R$ from the second [sphere](../../../../../sphere.md) its [velocity](../../../../../velocity.md) is

$$
\Delta\mathbf U=\frac{5a^3}{2R^5}(\mathbf E_2:\mathbf R\mathbf R)\mathbf R=-\frac{15a^4}{4R^6}(\mathbf U_0\cdot\mathbf R)\mathbf R.
$$

The first [sphere](../../../../../sphere.md) translates in this returned incident flow. Finite-size sampling and higher incident multipoles enter only beyond the retained reflection order. Thus the [stresslet reflection between two force-free and forced spheres](../../../../../stresslet-reflection-between-two-force-free-and-forced-spheres.md) gives

$$
\boxed{\mathbf U=\mathbf U_0-\frac{15a^4}{4R^6}(\mathbf U_0\cdot\mathbf R)\mathbf R+O\!\left(|\mathbf U_0|(a/R)^5\right)}.
$$

The factor $|\mathbf U_0|$ makes explicit the [velocity](../../../../../velocity.md) scale implicit in the printed remainder.

The resulting input power, equal to the [viscous dissipation](../../../../../viscous-dissipation.md), is

$$
\mathbf F\cdot\mathbf U=6\pi\mu a\left[|\mathbf U_0|^2-\frac{15a^4}{4R^6}(\mathbf U_0\cdot\mathbf R)^2\right]+\text{higher orders}.
$$

It decreases at fixed [force](../../../../../force.md). The [Minimum-dissipation theorem for Stokes flow](../../../../../minimum-dissipation-theorem-for-stokes-flow.md) instead compares admissible fields at fixed first-sphere [velocity](../../../../../velocity.md): extending a two-sphere field rigidly into the second [sphere](../../../../../sphere.md) gives an admissible one-sphere field, so the extra rigid inclusion can only increase the minimum resistance. Allowing the second [sphere](../../../../../sphere.md) to choose its translation and rotation minimizes over its rigid motions, producing zero [force](../../../../../force.md) and couple there. An increase of this effective [hydrodynamic resistance matrix](../../../../../hydrodynamic-resistance-matrix.md) decreases its inverse [hydrodynamic mobility matrix](../../../../../hydrodynamic-mobility-matrix.md), and hence decreases fixed-force power. **The negative mobility correction is therefore consistent with minimum dissipation.**

If the second [sphere](../../../../../sphere.md) is prevented from rotating, its [angular velocity](../../../../../angular-velocity.md) relative to the incident fluid becomes

$$
\boldsymbol\Omega_{\mathrm{rel}}=-\frac12\boldsymbol\omega_1(\mathbf R)=-\frac{3a}{4R^3}\mathbf U_0\times\mathbf R.
$$

Use the [rotating sphere in Stokes flow](../../../../../rotating-sphere-in-stokes-flow.md) at $-\mathbf R$. The additional reflected [rotlet](../../../../../rotlet.md) gives

$$
\Delta\mathbf U_{\mathrm{rot}}=\frac{3a^4}{4R^6}(\mathbf U_0\times\mathbf R)\times\mathbf R=-\frac{3a^4}{4R^4}\left[\mathbf U_0-(\mathbf U_0\cdot\mathbf n)\mathbf n\right].
$$

Adding this [rotation-clamped reflection between two spheres](../../../../../rotation-clamped-reflection-between-two-spheres.md) to the strain reflection,

$$
\boxed{\mathbf U=\mathbf U_0-\frac{a^4}{R^4}\left[\frac{15}{4}(\mathbf U_0\cdot\mathbf n)\mathbf n+\frac34\left(\mathbf U_0-(\mathbf U_0\cdot\mathbf n)\mathbf n\right)\right]+O\!\left(|\mathbf U_0|(a/R)^5\right)}.
$$

The holding couple supplies no power because the held [sphere](../../../../../sphere.md)'s [angular velocity](../../../../../angular-velocity.md) is zero.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 74](../../paper-74-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
