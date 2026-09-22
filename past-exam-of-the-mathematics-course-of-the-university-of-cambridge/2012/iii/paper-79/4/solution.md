<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use a [top-hat plume model](../../../../../top-hat-plume-model.md) per unit span. Define volume and kinematic momentum fluxes $Q=bw$ and $J=bw^2$, and set the pure-ice [reduced gravity](../../../../../reduced-gravity-split.md) $g'=g(\rho_0-\rho_s)/\rho_0>0$. The suspension buoyancy is $g'\phi$. The supplied equations express vertical [momentum conservation](../../../../../momentum-conservation.md), conservation of relative enthalpy including latent heat, and conservation of excess salt, respectively. At the release height, prescribe compatible source volume/momentum, salt and enthalpy fluxes, or equivalent source width, velocity, composition and ice fraction; impose ambient entrained water at $(T_0,C_0)$ with no vertical momentum. A pure far-field similarity solution may instead be described using a virtual origin, but its singular near-origin values are not physical inlet conditions.

The missing balance is total mass, equivalently volume under the [Boussinesq approximation](../../../../../boussinesq-approximation.md). In a wall plume, only the exposed outer edge entrains, so the [Batchelor entrainment hypothesis](../../../../../batchelor-entrainment-hypothesis.md) $v_e=e\,w$ gives

$$
\boxed{Q'=e\,w.}
$$

If two free edges are intended, replace $e$ by $2e$ everywhere; the numerical coefficient is a geometry convention. The glacier boundary itself has no normal flow. Local phase conversion does not add volume at retained Boussinesq order, and crystals are assumed to share the liquid velocity.

For a box of height $dz$, the upward momentum flux changes by $\rho_0[J(z+dz)-J(z)]$. The ambient hydrostatic pressure has been subtracted; the remaining force is the suspension buoyancy $\rho_0bg'\phi\,dz$. Entrained ambient water carries no vertical momentum, and drag is neglected, giving $J'=bg'\phi$. Salt entering through the exposed edge is $C_0Q'\,dz$, so $(\bar C Q)'=C_0Q'$ and therefore

$$
\boxed{J'=bg'\phi,\qquad[(\bar C-C_0)Q]'=0.}
$$

These control-volume derivations account for entrainment rather than treating $Q$ as constant.

**Thermodynamic elimination.** Let the conserved excess enthalpy and salt fluxes be $E$ and $S$:

$$
E=[c_p(T-T_0)-L\phi]Q,\qquad S=(\bar C-C_0)Q.
$$

The ambient satisfies $T_0=-mC_0$, while equilibrium in the ice-bearing plume gives

$$
\bar C=C_0+S/Q,\qquad T=-m\frac{C_0+S/Q}{1-\phi}.
$$

Substitute this temperature in the enthalpy invariant. Exact rearrangement gives

$$
\boxed{\phi Q[L+c_pmC_0-L\phi]=-E-c_pmS+E\phi.}
$$

Thus, at dilute-crystal order,

$$
\boxed{\phi Q\simeq I_0=\frac{-E-c_pmS}{L+c_pmC_0},\qquad \mathcal F=g'I_0.}
$$

The [ice-bearing wall-plume thermodynamic invariant](../../../../../ice-bearing-wall-plume-thermodynamic-invariant.md) fixes the leading advected ice volume and buoyancy flux from the source deficits. A rising ice-dominated branch requires $I_0>0$. It is not determined from reduced gravity alone. The small-$\phi$ expansion also presumes finite source fluxes and no cancellation making the discarded terms comparable to $-E-c_pmS$.

The three remaining leading equations are $Q'=e w$, $(Qw)'=\mathcal F/w$, and $\phi=I_0/Q$. Seek a similarity form in $Z=z-z_v>0$ with $Q\propto Z^p$, $w\propto Z^q$. Continuity gives $p=q+1$, while momentum gives $p+2q=1$. Therefore $q=0,p=1$. The coefficients obey $e w^3=\mathcal F$, giving the [self-similar ice-bearing wall plume](../../../../../self-similar-ice-bearing-wall-plume.md)

$$
\boxed{b=eZ,\qquad w=\left(\frac{g'I_0}{e}\right)^{1/3},\qquad Q=e\left(\frac{g'I_0}{e}\right)^{1/3}Z,\qquad\phi=\frac{w^2}{g'Z}=\frac{I_0^{2/3}}{e^{2/3}g'^{1/3}Z}.}
$$

The width grows linearly, the speed approaches a constant, and the crystals dilute inversely with height. This is a buoyancy-conserving [wall line plume](../../../../../wall-line-plume.md), with buoyancy supplied mainly by the ice fraction rather than a temperature anomaly. The dilute-crystal regime requires $Z\gg w^2/g'$ and lies away from the formal virtual-origin singularity. If all source flux deficits vanish, $I_0=0$ and this nontrivial rising branch does not exist. The exact thermodynamic invariants above, rather than their truncated version, are needed near a concentrated source.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 79](../../paper-79-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
