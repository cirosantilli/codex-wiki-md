<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $d_1=\rho_0-\rho_1>0$, $d_2=\rho_2-\rho_0>0$, and choose the common undisturbed interface pressure $P$. The [hydrostatic pressure](../../../../../../hydrostatic-pressure.md) is $p_1=P-\rho_1gz$ in the upper fluid and $p_2=P-\rho_2gz$ in the lower fluid. Continuity of [hydrostatic pressure](../../../../../../hydrostatic-pressure.md) across both current interfaces gives

$$
p_0=P-\rho_0gz+d_1gh_1=P-\rho_0gz-d_2gh_2,\qquad \boxed{d_1h_1=-d_2h_2.}
$$

Thus $h_1=d_2h/(d_1+d_2)$ and $h_2=-d_1h/(d_1+d_2)$. This [isostatic depth partition of an interfacial current](../../../../../../isostatic-depth-partition-of-an-interfacial-current.md) expresses local vertical buoyancy balance: a displaced column with an imbalance would move vertically until the partition was restored. With the [hydrostatic pressure](../../../../../../hydrostatic-pressure.md) $P-\rho_0gz$ subtracted, the pressure within the current is $\Delta\rho gh$, where

$$
\boxed{\Delta\rho=\frac{(\rho_0-\rho_1)(\rho_2-\rho_0)}{\rho_2-\rho_1},\qquad\mathbf f=-\Delta\rho g h_r\mathbf e_r.}
$$

The equivalent [body force](../../../../../../body-force.md) is outward for a profile decreasing with $r$. Its magnitude is $\Delta\rho g|h_r|$; the derivative without an absolute value is a signed quantity.

For an [ambient-controlled interfacial plug current](../../../../../../ambient-controlled-interfacial-plug-current.md), integrating the [body force](../../../../../../body-force.md) through depth gives radial force per area $O(\Delta\rho gH^2/R)$. The ambient [Stokes flow](../../../../../../stokes-flow-split.md) varies over distance $R$, exerting [traction](../../../../../../traction.md) $O(\mu u/R)$, so **$u\sim\Delta\rho gH^2/\mu$**. The current's internal shear supports the ambient [traction](../../../../../../traction.md) with a velocity difference $\Delta u\sim(\mu u/R)H/(\lambda\mu)$; $\Delta u/u\sim H/(\lambda R)\ll1$ requires $\lambda\gg H/R$. The force per area from its in-plane viscous extension is $O(\lambda\mu uH/R^2)$, negligible against ambient [traction](../../../../../../traction.md) when $\lambda\ll R/H$. Together these give the [viscosity window for an interfacial plug current](../../../../../../viscosity-window-for-an-interfacial-plug-current.md)

$$
\boxed{H/R\ll\lambda\ll R/H.}
$$

Fixed volume gives $V\sim HR^2$, and the spreading velocity has the scale $\dot R$. Thus $\dot R\sim\Delta\rho gV^2/(\mu R^4)$ and

$$
\boxed{R\sim At^{1/5},\qquad A\sim(\Delta\rho gV^2/\mu)^{1/5}.}
$$

Choosing $A$ so that $R=At^{1/5}$ exactly, the [similarity solution](../../../../../../similarity-solution.md) has $h=(V/A^2)t^{-2/5}F(\eta)$, $\eta=r/(At^{1/5})$, and $u=At^{-4/5}U(\eta)$. In radial conservation $h_t+r^{-1}(rhu)_r=0$, substitution gives $(\eta FU)'=(\eta^2F)'/5$. Regularity and no source at the centre remove the integration constant. Therefore **the radial plug velocity is linear**:

$$
\boxed{U(\eta)=\eta/5,\qquad u=r/(5t).}
$$

For the [disc-traction analogy for an interfacial current](../../../../../../disc-traction-analogy-for-an-interfacial-current.md), subtract the imposed straining flow from the stationary-disc solution. The perturbation has velocity $-Er\mathbf e_r$ on the disc and zero far-field velocity. Reverse its sign: the resulting [Stokes flow](../../../../../../stokes-flow-split.md) is driven by a radially expanding disc with velocity $Er\mathbf e_r$ in otherwise quiescent fluid. The background straining flow contributes no radial shear [traction](../../../../../../traction.md) on $z=0$, so the given disc [traction](../../../../../../traction.md) changes sign. This step uses [Linearity of Stokes flow](../../../../../../linearity-of-stokes-flow.md), [Uniqueness of Stokes flow](../../../../../../uniqueness-of-stokes-flow.md), and the [no-slip boundary condition](../../../../../../no-slip-boundary-condition.md). The thin plug current has the same leading boundary velocity and hence the same ambient resistance. Each face contributes $-8\mu Er/[\pi\sqrt{R^2-r^2}]$; both faces must be counted. With $E=1/(5t)$, radial force balance is

$$
-\Delta\rho g h h_r=\frac{16\mu Er}{\pi\sqrt{R^2-r^2}},\qquad\boxed{h h_r=-\frac{16\mu r}{5\pi\Delta\rho gt\sqrt{R^2-r^2}}.}
$$

Integrate with $h(R,t)=0$. The [interfacial plug-current similarity profile](../../../../../../interfacial-plug-current-similarity-profile.md) is

$$
\boxed{h^2=\frac{32\mu\sqrt{R^2-r^2}}{5\pi\Delta\rho gt},\qquad h=H(1-r^2/R^2)^{1/4},\quad H^2=\frac{32\mu R}{5\pi\Delta\rho gt}.}
$$

Volume integration gives $V=2\pi\int_0^Rrh\,dr=4\pi HR^2/5$. Eliminating $H$ gives the full prefactor:

$$
\boxed{R(t)=\left(\frac{125\Delta\rho gV^2t}{512\pi\mu}\right)^{1/5}.}
$$

The formal edge slope diverges, so a narrow edge region lies outside the thin-current approximation. Its [traction](../../../../../../traction.md) and volume contributions are integrable, and this is a leading thin-current solution rather than a uniformly valid edge description.

For a [diffusion-controlled solute gravity current](../../../../../../diffusion-controlled-solute-gravity-current.md), excess solute mass, not enriched-fluid volume, is conserved. At late times the effective [mass density](../../../../../../density.md) excess is proportional to solute concentration, so $\Delta\rho(t)R^2H\sim\Delta\rho_0V_0$, and $H\sim(Dt)^{1/2}$. The same ambient resistance scaling gives

$$
\dot R\sim\frac{\Delta\rho_0gV_0}{\mu}\frac{(Dt)^{1/2}}{R^2},\qquad\boxed{R(t)\sim\left(\frac{\Delta\rho_0gV_0}{\mu}\right)^{1/3}D^{1/6}t^{1/2}.}
$$

This scaling does not determine a universal numerical prefactor. The [mass diffusivity](../../../../../../mass-diffusivity.md) $D$ controls the growing depth, while dilution weakens buoyancy; assuming a fixed current volume would incorrectly retain the $t^{1/5}$ law. The thin-layer requirement becomes $(\mu D/(\Delta\rho_0gV_0))^{1/3}\ll1$; when only dissolved solute changes the upper fluid, its [viscosity](../../../../../../dynamic-viscosity.md) is of order the ambient [viscosity](../../../../../../dynamic-viscosity.md), consistent with the plug-current window.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 329](../../../paper-329-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
