<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use [Planck units](../../../../../planck-units.md) for the following formulas. The [black-hole area theorem](../../../../../hawking-s-area-theorem.md) is a classical statement with hypotheses. Assume the [Einstein field equations](../../../../../einstein-field-equations.md), the [null energy condition](../../../../../null-energy-condition.md) and appropriate global future regularity/predictability. For a clean version of the focusing sketch, take the future horizon generators to remain on a regular horizon and to be future complete in affine parameter. The usual [strong asymptotic predictability](../../../../../strong-asymptotic-predictability.md) formulation supplies the global causal control needed to exclude the same focusing pathology; an arbitrary spacetime with naked future breakdown is not covered by the theorem.

Let $\ell^a$ be an affinely parametrized generator of a smooth portion of the [event horizon](../../../../../event-horizon.md), and let $\theta=d\log dA/d\lambda$ be its [null expansion](../../../../../null-expansion.md). The horizon is a null hypersurface, so its generators have zero [null twist](../../../../../null-twist.md). In four dimensions the [Null Raychaudhuri equation](../../../../../null-raychaudhuri-equation.md) is

$$
\frac{d\theta}{d\lambda}=-\frac12\theta^2-\sigma_{ab}\sigma^{ab}-R_{ab}\ell^a\ell^b.
$$

The [Einstein field equations](../../../../../einstein-field-equations.md) give $R_{ab}\ell^a\ell^b=8\pi T_{ab}\ell^a\ell^b\ge0$, since the metric terms vanish when contracted with a null vector. The screen-space [null shear](../../../../../null-shear.md) term is also nonnegative, so $\theta'\le-\theta^2/2$. If $\theta_0<0$ at $\lambda_0$, integrating this inequality while the congruence remains regular gives

$$
\theta(\lambda)\le\frac{\theta_0}{1+\tfrac12\theta_0(\lambda-\lambda_0)}.
$$

It focuses within affine distance at most $2/|\theta_0|$. The vanishing area element is a focal point to an earlier spacelike horizon cut. Past such a point the [null geodesic](../../../../../null-geodesic.md) can no longer generate an [achronal boundary](../../../../../achronal-boundary.md), but the [event horizon](../../../../../event-horizon.md) is precisely such a boundary. Future completeness and the global hypotheses exclude its escaping this contradiction by ending prematurely at a pathology. Therefore $\theta\ge0$ everywhere the smooth horizon description applies.

Integrate $d(dA)/d\lambda=\theta\,dA$ between ordered horizon cuts. Every continuing generator contributes a nondecreasing area element. New generators can enter at past endpoints or merger crease sets, adding area; generators cannot leave a regular future horizon through future endpoints under these hypotheses. Thus, including the total area of disconnected components,

$$
\boxed{A_{\rm later}\ge A_{\rm earlier}.}
$$

This is the [future-complete horizon focusing proof of the area theorem](../../../../../future-complete-horizon-focusing-proof-of-the-area-theorem.md). A smooth elementary congruence proof requires the stated regularity; the general theorem also treats the horizon's nonsmooth joining set rather than assuming mergers have a globally smooth horizon.

[Hawking radiation](../../../../../hawking-radiation.md) changes the situation because the quantum field state in a collapsing geometry is not a classical positive-energy fluid. For a large isolated [Schwarzschild black hole](../../../../../schwarzschild-spacetime.md),

$$
T_H=\frac1{8\pi M},\qquad r_H\simeq2M,\qquad A\simeq16\pi M^2
$$

in natural units. Outgoing quantum modes at [future null infinity](../../../../../future-null-infinity.md) have a nearly thermal occupation, modified by [greybody factors](../../../../../greybody-factor.md); an accompanying negative [Killing energy](../../../../../killing-energy.md) flux near the horizon reduces the hole's mass. On timescales short compared with the evaporation time but long compared with $M$, its geometry is approximately [Schwarzschild spacetime](../../../../../schwarzschild-spacetime.md) with slowly decreasing $M(t)$. It is not an exactly stationary vacuum solution with a parameter changed by hand: the radiation's [stress-energy tensor](../../../../../stress-energy-tensor.md) sources the time dependence through the [semiclassical Einstein equation](../../../../../semiclassical-einstein-equation.md). The distant luminosity is carried by the outgoing radiation, while the horizon-area decrease accompanies the inward negative-energy contribution.

As the [black hole](../../../../../black-hole.md) loses mass, its horizon scale and [Bekenstein-Hawking entropy](../../../../../bekenstein-hawking-entropy.md) shrink, its temperature rises and its luminosity increases. This is the [negative heat capacity of a Schwarzschild black hole](../../../../../negative-heat-capacity-of-a-schwarzschild-black-hole.md). Large astrophysical holes evaporate extremely slowly in isolation; small holes evaporate more rapidly, and increasingly massive particle species become accessible as the temperature rises. An incoming radiation bath or accretion can instead offset the loss, so the pure evaporation law assumes negligible incoming energy. A formal complete evaporation also raises the [black hole information paradox](../../../../../black-hole-information-paradox.md); the low-curvature calculation alone does not determine how information or the final state is resolved.

For an elementary luminosity estimate, treat the horizon as emitting photon [blackbody radiation](../../../../../black-body-radiation.md). In natural units the [Stefan–Boltzmann law](../../../../../stefan-boltzmann-law.md) has $\sigma=\pi^2/60$, giving

$$
P=A\sigma T_H^4=\frac1{15360\pi M^2}.
$$

The horizon area used here is an estimate of emitting area, not the exact frequency-dependent absorption cross-section. More generally write $P=\alpha/M^2$, where $\alpha>0$ includes the [greybody factors](../../../../../greybody-factor.md) and the active particle species. For constant effective $\alpha$, energy balance and direct integration give

$$
\frac{dM}{dt}=-\frac{\alpha}{M^2},\qquad \frac{d(M^3)}{dt}=-3\alpha,
\qquad\boxed{M(t)=\bigl(M_0^3-3\alpha t\bigr)^{1/3}.}
$$

Here $t$ is time measured at infinity. The formal evaporation timescale is $M_0^3/(3\alpha)$; with the photon blackbody estimate it is $5120\pi M_0^3$. Restoring constants gives

$$
\boxed{t_{\rm evap}\simeq\frac{5120\pi G^2M_0^3}{\hbar c^4}}
$$

for that specified estimate. If particle thresholds make $\alpha$ mass dependent, the precise leading law is instead $t=\int_{M(t)}^{M_0}m^2\,dm/\alpha(m)$. The robust result is the inverse-square mass-loss rate for a fixed species regime and the cubic mass scaling of its lifetime. This is the [semiclassical cubic mass law for Schwarzschild evaporation](../../../../../semiclassical-cubic-mass-law-for-schwarzschild-evaporation.md). Extrapolating its zero to a definite end state is unjustified once $M$ approaches the [Planck mass](../../../../../planck-mass.md) and curvature requires [quantum gravity](../../../../../quantum-gravity.md).

There is **no contradiction with the classical area theorem**: the renormalized quantum [stress-energy tensor](../../../../../stress-energy-tensor.md) can violate the [null energy condition](../../../../../null-energy-condition.md) used in the focusing inequality. In the evaporation regime,

$$
\frac{dA}{dt}\simeq32\pi M\frac{dM}{dt}=-\frac{32\pi\alpha}{M}<0,
$$

which is permitted when that hypothesis fails. The thermodynamic replacement is the [generalized second law](../../../../../generalized-second-law.md), concerning $S_{\rm outside}+A/(4G\hbar)$ rather than horizon area alone. Outside radiation can carry entropy while the hole's [Bekenstein-Hawking entropy](../../../../../bekenstein-hawking-entropy.md) decreases.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 62](../../paper-62-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
