<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Apply the [moving-interface conservation jump identity](../../../../../../../moving-interface-conservation-jump-identity.md) first to mass, then to each momentum component. Write $j_i=\rho u_i$ and $\Pi_{ij}=\rho u_iu_j+p\delta_{ij}-\sigma_{ij}$, with all quantities understood piecewise on the two sides. Define the jumps of flux relative to the moving [shock wave](../../../../../../../shock-wave.md) by

$$
Q=[\rho(\mathbf u-\mathbf v)\cdot\mathbf n],\qquad L_i=[\rho u_i(\mathbf u-\mathbf v)\cdot\mathbf n+p n_i-\sigma_{ij}n_j].
$$

The global distributional conservation equations are

$$
\partial_t\rho+\partial_ij_i=Q\delta_s,\qquad\partial_tj_i+\partial_j\Pi_{ij}=L_i\delta_s.
$$

Differentiate the first in time and subtract the divergence of the second. With $\rho'=\rho-\rho_0$ and the piecewise [Lighthill stress tensor](../../../../../../../lighthill-stress-tensor.md) $T_{ij}=\rho u_iu_j+(p'-c_0^2\rho')\delta_{ij}-\sigma_{ij}$, this gives

$$
\boxed{(\partial_t^2-c_0^2\nabla^2)\rho'=\partial_i\partial_jT_{ij}+\partial_t(Q\delta_s)-\partial_i(L_i\delta_s).}
$$

Derivatives act on the complete distributions, including their moving support. The [acoustic quadrupole](../../../../../../../acoustic-quadrupole.md) term represents momentum-stress fluctuations throughout the volume. The time derivative of the surface mass-flux defect is an [acoustic monopole](../../../../../../../acoustic-monopole.md), representing injection or removal of mass/volume. The divergence of the surface momentum-flux defect is an [acoustic dipole](../../../../../../../acoustic-dipole.md), representing a force sheet. This is the [distributional acoustic analogy across a moving interface](../../../../../../../distributional-acoustic-analogy-across-a-moving-interface.md).

For an actual freely propagating fluid [shock wave](../../../../../../../shock-wave.md) with no singular mass or momentum supply, the [Rankine-Hugoniot conditions](../../../../../../../rankine-hugoniot-conditions.md) give **$Q=0$ and $L_i=0$**. Such a shock does not acquire independent monopole and force-sheet sources merely because it is discontinuous. Its effects remain in the distributional derivatives of $T_{ij}$, including singular derivatives of its jump. Nonzero surface sources are appropriate for an interface with exchange/forcing or for a formulation that omits one side of the fluid.

**A shock does not, by itself, justify retaining the $m^4$ scaling.** That estimate required a low-[Mach number](../../../../../../../mach-number.md) stress $O(\rho_0U^2)$ varying on the slow time $\ell/U$. Fast shock motion, short time scales, or thermodynamic deviations can invalidate that estimate. If these same compact, slow-source assumptions remain valid for the integrated [Lighthill stress tensor](../../../../../../../lighthill-stress-tensor.md), its quadrupole estimate still follows, even distributionally. There is no universal replacement power deducible from the mere presence of a shock; nor should vanished physical flux defects be treated as additional independent radiation sources.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 77](../../../../paper-77-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
